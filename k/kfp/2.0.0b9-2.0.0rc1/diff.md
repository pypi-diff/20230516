# Comparing `tmp/kfp-2.0.0b9.tar.gz` & `tmp/kfp-2.0.0-rc.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.fOlpoJia/kfp-2.0.0b9.tar", last modified: Wed Dec 21 02:26:58 2022, max compression
+gzip compressed data, was "/var/folders/s4/q287k45x17x_j2mlv1lc_43r00xv1g/T/tmp.PWxKLpYf/kfp-2.0.0rc1.tar", last modified: Tue May 16 18:50:52 2023, max compression
```

## Comparing `kfp-2.0.0b9.tar` & `kfp-2.0.0-rc.1.tar`

### file list

```diff
@@ -1,247 +1,250 @@
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2022-12-21 00:57:23.000000 kfp-2.0.0b9/MANIFEST.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3890 2022-12-21 02:26:58.000000 kfp-2.0.0b9/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2155 2022-12-21 00:57:23.000000 kfp-2.0.0b9/README.md
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      869 2022-12-21 02:23:10.000000 kfp-2.0.0b9/kfp/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/cli_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5391 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/compile_.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/compile_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15375 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19857 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2022-06-02 23:27:30.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3155 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1500 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/dsl.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5347 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8261 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8152 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9066 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8286 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/cli/utils/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/aliased_plurals_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/aliased_plurals_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/deprecated_alias_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/deprecated_alias_group_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/parsing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/cli/utils/parsing_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/client/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    62973 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12327 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/client_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/set_volume_credentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/set_volume_credentials_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/token_credentials_base.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/client/token_credentials_base_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3414 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    84159 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/compiler/compiler_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20834 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/compiler/compiler_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    75610 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/compiler/pipeline_spec_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11250 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/compiler/pipeline_spec_builder_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8163 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/compiler/read_write_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1321 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4851 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/base_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5441 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/base_component_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5995 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5507 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21063 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/component_factory.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6109 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/component_factory_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/constants.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1459 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/container_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1997 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/container_component_artifact_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1831 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/container_component_artifact_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1905 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/container_component_decorator.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2707 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/container_component_decorator_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15216 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/executor.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3649 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/executor_main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    43375 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/executor_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9775 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6428 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/for_loop_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2975 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1015 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/importer_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5510 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/importer_node.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7662 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/importer_node_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/kfp_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12848 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/pipeline_channel.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5657 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/pipeline_channel_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6352 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/pipeline_context.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20812 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/pipeline_task.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9602 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/pipeline_task_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14193 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/placeholders.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18122 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/placeholders_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1466 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/python_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    41899 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    32584 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/structures_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/task_final_status.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7705 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/tasks_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2851 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/tasks_group_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/components/types/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2415 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8059 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/custom_artifact_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16140 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/custom_artifact_types_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7405 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/type_annotations.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7717 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/type_annotations_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14982 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13813 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/types/type_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3859 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3679 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1740 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/v1_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/v1_modelbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27893 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/v1_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4194 2022-12-21 02:25:42.000000 kfp-2.0.0b9/kfp/components/yaml_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4324 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/components/yaml_component_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/__main__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/_auth.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63449 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/_config.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/_local_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/_runners.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/auth/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/auth/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/auth/_satvolumecredentials.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/auth/_tokencredentialsbase.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/aws.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/azure.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/cli/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/components_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/dev_env.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/dev_env_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/gcp.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/gcp_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/utility.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/utility_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me_cli.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/experiment.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/output.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/recurring_run.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/cli/run.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/compiler/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/_data_passing_rewriter.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/_data_passing_using_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/_default_transformers.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/_k8s_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/_op_to_template.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/main.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/v2_compat.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/compiler/v2_compatible_compiler_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/components/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_airflow_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_component_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_data_passing.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_dynamic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_key_value_store.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_naming.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_python_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_python_to_graph_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_structures.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/_yaml_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/modelbase.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/components/structures/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/structures/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/type_annotation_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/components/type_annotation_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/containers/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_build_image_api.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_cache.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_component_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_container_builder.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_gcs_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/_k8s_job_helper.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/entrypoint.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/containers/entrypoint_utils.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_component.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_component_bridge.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_container_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_container_op_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_for_loop.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_metadata.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_ops_group.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline_param.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline_volume.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_resource_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_volume_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/_volume_snapshot_op.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/artifact.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/artifact_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/component_spec.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/component_spec_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/data_passing_methods.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/dsl_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/dsl_utils_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/dsl/extensions/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/extensions/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/extensions/kubernetes.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/io_types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/metrics_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/metrics_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/serialization_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/serialization_utils_test.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/type_utils.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/dsl/types.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/gcp.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/deprecated/notebook/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/notebook/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/notebook/_magic.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/deprecated/onprem.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/dsl/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7143 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/dsl/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/registry/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/__init__.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/registry/context/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/context/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/context/default_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/context/kfp_pkg_dev.json
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/registry_client.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/registry/registry_client_test.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp/v2/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/v2/__init__.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/v2/compiler.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/v2/components.py
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2022-12-21 00:57:23.000000 kfp-2.0.0b9/kfp/v2/dsl.py
-drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3890 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/PKG-INFO
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7594 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/SOURCES.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/dependency_links.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/entry_points.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      556 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/requires.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2022-12-21 02:26:58.000000 kfp-2.0.0b9/kfp.egg-info/top_level.txt
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1418 2022-12-21 00:57:23.000000 kfp-2.0.0b9/requirements.in
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2022-12-21 02:26:58.000000 kfp-2.0.0b9/setup.cfg
--rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3613 2022-12-21 00:57:23.000000 kfp-2.0.0b9/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       60 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/MANIFEST.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2155 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/README.md
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      887 2023-05-16 18:47:57.000000 kfp-2.0.0rc1/kfp/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      878 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4024 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7072 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/cli_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5391 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/compile_.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2304 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/compile_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16072 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    23333 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-03-14 22:48:17.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2460 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2694 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6098 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3786 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4495 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3280 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3040 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2714 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      744 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/dsl.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5369 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7225 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8364 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9395 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7291 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/cli/utils/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1434 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1684 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2439 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1595 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2568 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/parsing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4169 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/cli/utils/parsing_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/client/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      998 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20239 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    66676 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/client/client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17294 2023-05-12 20:36:23.000000 kfp-2.0.0rc1/kfp/client/client_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3269 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/set_volume_credentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1926 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/set_volume_credentials_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1765 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/token_credentials_base.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2390 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/client/token_credentials_base_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      749 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3443 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)   152313 2023-05-12 17:28:57.000000 kfp-2.0.0rc1/kfp/compiler/compiler_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    32534 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1965 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/compiler_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    85354 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16862 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8163 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/compiler/read_write_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1321 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6055 2023-05-09 18:23:54.000000 kfp-2.0.0rc1/kfp/components/base_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5432 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/base_component_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5995 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5489 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_decorator_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25321 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/component_factory.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6726 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/component_factory_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1079 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/constants.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1516 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1997 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_artifact_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1888 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_artifact_channel_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1905 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/container_component_decorator.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4574 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/container_component_decorator_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15493 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3649 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor_main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    43760 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/executor_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    11014 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6428 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/for_loop_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3399 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1015 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5510 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_node.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7662 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/importer_node_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4012 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/kfp_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13634 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/pipeline_channel.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5981 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/pipeline_channel_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6436 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_context.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27154 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_task.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12295 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/pipeline_task_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16441 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/placeholders.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    22066 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/placeholders_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1523 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/python_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    44307 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/components/structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    38004 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/structures_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2372 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/task_final_status.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7711 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/tasks_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2851 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/tasks_group_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/components/types/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18756 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2415 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/artifact_types_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8059 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/custom_artifact_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16140 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/custom_artifact_types_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7647 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_annotations.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7717 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_annotations_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    19843 2023-05-13 00:03:12.000000 kfp-2.0.0rc1/kfp/components/types/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    26536 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/types/type_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3905 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/kfp/components/utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3679 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1740 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16240 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_modelbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    27893 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/v1_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4214 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/yaml_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4324 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/components/yaml_component_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      811 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      767 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/__main__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9693 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_auth.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63369 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      799 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_config.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    20892 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_local_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3829 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/_runners.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/auth/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      859 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2594 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/_satvolumecredentials.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1551 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/auth/_tokencredentialsbase.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2561 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/aws.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2272 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/azure.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/cli/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      584 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3038 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    15615 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17870 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/components_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      603 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2489 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2734 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6151 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3826 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4547 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3320 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3169 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1529 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3729 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me_cli.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4548 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/experiment.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2156 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/output.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9207 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7544 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/recurring_run.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7476 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/cli/run.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      761 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    24589 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_rewriter.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    12032 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_using_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3480 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_default_transformers.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3168 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_k8s_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    14459 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/_op_to_template.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    58420 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5028 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/main.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6946 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compat.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7033 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compatible_compiler_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/components/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      740 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6680 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_airflow_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    16145 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_component_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25925 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8214 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_data_passing.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3572 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_dynamic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2552 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_key_value_store.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4189 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_naming.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    52469 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_python_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9535 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_python_to_graph_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    29100 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_structures.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2757 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/_yaml_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17572 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/modelbase.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/components/structures/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       28 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/structures/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1917 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2809 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/containers/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      581 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7468 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_build_image_api.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2527 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_cache.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17356 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_component_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10904 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_container_builder.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3603 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_gcs_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7344 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/_k8s_job_helper.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8735 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7158 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint_utils.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1665 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6364 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_component.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    30557 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_component_bridge.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    63751 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1865 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    10053 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_for_loop.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3857 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_metadata.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8123 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_ops_group.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    13111 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     9125 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_param.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4483 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_volume.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     8409 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_resource_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6057 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4771 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_snapshot_op.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7871 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/artifact.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3439 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/artifact_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    18942 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    25290 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1210 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/data_passing_methods.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5155 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2119 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3511 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/kubernetes.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1311 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/io_types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     6121 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2330 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1367 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1221 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils_test.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3750 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/type_utils.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7886 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/dsl/types.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     5984 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/gcp.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      607 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/notebook/_magic.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     4757 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/deprecated/onprem.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/dsl/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7618 2023-05-16 00:14:24.000000 kfp-2.0.0rc1/kfp/dsl/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/registry/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      837 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/__init__.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/registry/context/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      585 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1060 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/default_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     2381 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/context/kfp_pkg_dev.json
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    21147 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/registry_client.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)    17404 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/registry/registry_client_test.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp/v2/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      921 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/__init__.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      621 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/compiler.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      623 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/components.py
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      616 2023-05-04 22:04:58.000000 kfp-2.0.0rc1/kfp/v2/dsl.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3977 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/PKG-INFO
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     7648 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/SOURCES.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        1 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/dependency_links.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      142 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/entry_points.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      449 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/requires.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)        4 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/kfp.egg-info/top_level.txt
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     1276 2023-05-16 18:47:57.000000 kfp-2.0.0rc1/requirements.in
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)       38 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/setup.cfg
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)     3769 2023-05-11 16:02:47.000000 kfp-2.0.0rc1/setup.py
+drwxr-xr-x   0 cjmccarthy (977967) primarygroup (89939)        0 2023-05-16 18:50:52.000000 kfp-2.0.0rc1/tests/
+-rw-r--r--   0 cjmccarthy (977967) primarygroup (89939)      158 2023-03-14 22:48:17.000000 kfp-2.0.0rc1/tests/test_kfp.py
```

### Comparing `kfp-2.0.0b9/PKG-INFO` & `kfp-2.0.0rc1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.0b9
+Version: 2.0.0rc1
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
@@ -65,15 +65,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.7.0,<3.12.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: kubernetes
```

### Comparing `kfp-2.0.0b9/README.md` & `kfp-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/__init__.py` & `kfp-2.0.0rc1/kfp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,12 +12,13 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # `kfp` is a namespace package.
 # https://packaging.python.org/guides/packaging-namespace-packages/#pkgutil-style-namespace-packages
 __path__ = __import__('pkgutil').extend_path(__path__, __name__)
 
-__version__ = '2.0.0-beta.9'
+__version__ = '2.0.0-rc.1'
 
 TYPE_CHECK = True
 
+from kfp import dsl
 from kfp.client import Client
```

### Comparing `kfp-2.0.0b9/kfp/cli/__init__.py` & `kfp-2.0.0rc1/kfp/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/__main__.py` & `kfp-2.0.0rc1/kfp/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/cli.py` & `kfp-2.0.0rc1/kfp/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/cli_test.py` & `kfp-2.0.0rc1/kfp/cli/cli_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/compile_.py` & `kfp-2.0.0rc1/kfp/cli/compile_.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/compile_test.py` & `kfp-2.0.0rc1/kfp/cli/compile_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/component.py` & `kfp-2.0.0rc1/kfp/cli/component.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,17 +42,17 @@
 # TODO: merge kfp_package_path into runtime-requirements.txt, once we have
 # kfp_runtime package that is dependency-free.
 _DOCKERFILE_TEMPLATE = '''
 FROM {base_image}
 
 WORKDIR {component_root_dir}
 COPY {requirements_file} {requirements_file}
-RUN pip install --no-cache-dir -r {requirements_file}
+RUN pip install {index_urls}--no-cache-dir -r {requirements_file}
 {maybe_copy_kfp_package}
-RUN pip install --no-cache-dir {kfp_package_path}
+RUN pip install {index_urls}--no-cache-dir {kfp_package_path}
 COPY . .
 '''
 
 _DOCKERIGNORE = '.dockerignore'
 
 # Location in which to write out shareable YAML for components.
 _COMPONENT_METADATA_DIR = 'component_metadata'
@@ -152,14 +152,15 @@
         self._component_files = [
             file for file in self._context_directory.glob(
                 self._component_filepattern) if file.is_file()
         ]
 
         self._base_image = None
         self._target_image = None
+        self._pip_index_urls = None
         self._load_components()
 
     def _load_components(self):
         if not self._component_files:
             logging.error(
                 f'No component files found matching pattern `{self._component_filepattern}` in directory {self._context_directory}'
             )
@@ -210,14 +211,21 @@
             logging.error(
                 'Did not find a target_image specified in any of the'
                 ' components. A target_image must be specified in order'
                 ' to build the component.')
             raise sys.exit(1)
         logging.info(f'Using target image: {self._target_image}')
 
+        pip_index_urls = []
+        for comp in self._components:
+            if comp.pip_index_urls is not None:
+                pip_index_urls.extend(comp.pip_index_urls)
+        if pip_index_urls:
+            self._pip_index_urls = list(dict.fromkeys(pip_index_urls))
+
     def _maybe_write_file(self,
                           filename: str,
                           contents: str,
                           overwrite: bool = False):
         if filename in self._context_directory_files:
             logging.info(
                 f'Found existing file {filename} under {self._context_directory}.'
@@ -266,38 +274,42 @@
             relative_path = component_info.module_path.relative_to(
                 self._context_directory)
             config.add_component(
                 function_name=component_info.function_name, path=relative_path)
         config.save()
 
     def maybe_generate_dockerfile(self, overwrite_dockerfile: bool = False):
+        index_urls_options = component_factory.make_index_url_options(
+            self._pip_index_urls)
         dockerfile_contents = _DOCKERFILE_TEMPLATE.format(
             base_image=self._base_image,
             maybe_copy_kfp_package=self._maybe_copy_kfp_package,
             component_root_dir=_COMPONENT_ROOT_DIR,
             kfp_package_path=self._kfp_package_path,
             requirements_file=_REQUIREMENTS_TXT,
+            index_urls=index_urls_options,
         )
 
         self._maybe_write_file(_DOCKERFILE, dockerfile_contents,
                                overwrite_dockerfile)
 
-    def build_image(self, push_image: bool):
+    def build_image(self, platform: str, push_image: bool):
         logging.info(f'Building image {self._target_image} using Docker...')
         client = docker.from_env()
 
         docker_log_prefix = 'Docker'
 
         try:
             context = str(self._context_directory)
             logs = client.api.build(
                 path=context,
                 dockerfile='Dockerfile',
                 tag=self._target_image,
                 decode=True,
+                platform=platform,
             )
             for log in logs:
                 message = log.get('stream', '').rstrip('\n')
                 if message:
                     logging.info(f'{docker_log_prefix}: {message}')
 
         except docker.errors.BuildError as e:
@@ -364,22 +376,27 @@
 @click.option(
     '--build-image/--no-build-image',
     type=bool,
     is_flag=True,
     default=True,
     help='Build the container image.')
 @click.option(
+    '--platform',
+    type=str,
+    default='linux/amd64',
+    help='The platform to build the container image for.')
+@click.option(
     '--push-image/--no-push-image',
     type=bool,
     is_flag=True,
     default=True,
     help='Push the built image to its remote repository.')
 def build(components_directory: str, component_filepattern: str, engine: str,
           kfp_package_path: Optional[str], overwrite_dockerfile: bool,
-          build_image: bool, push_image: bool):
+          build_image: bool, platform: str, push_image: bool):
     """Builds containers for KFP v2 Python-based components."""
 
     if build_image and engine != 'docker':
         warnings.warn(
             'The --engine option is deprecated and does not need to be passed. Only Docker engine is supported and will be used by default.',
             DeprecationWarning,
             stacklevel=2)
@@ -413,8 +430,8 @@
     builder.write_component_files()
     builder.generate_kfp_config()
 
     builder.generate_requirements_txt()
     builder.maybe_generate_dockerignore()
     builder.maybe_generate_dockerfile(overwrite_dockerfile=overwrite_dockerfile)
     if build_image:
-        builder.build_image(push_image=push_image)
+        builder.build_image(platform=platform, push_image=push_image)
```

### Comparing `kfp-2.0.0b9/kfp/cli/component_test.py` & `kfp-2.0.0rc1/kfp/cli/component_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,34 +26,39 @@
 import docker
 
 docker = mock.Mock()
 
 from kfp.cli import component
 
 
-def _make_component(func_name: str,
-                    base_image: Optional[str] = None,
-                    target_image: Optional[str] = None,
-                    packages_to_install: Optional[List[str]] = None,
-                    output_component_file: Optional[str] = None) -> str:
+def _make_component(
+    func_name: str,
+    base_image: Optional[str] = None,
+    target_image: Optional[str] = None,
+    packages_to_install: Optional[List[str]] = None,
+    output_component_file: Optional[str] = None,
+    pip_index_urls: Optional[List[str]] = None,
+) -> str:
     return textwrap.dedent('''
     from kfp.dsl import *
 
     @component(
         base_image={base_image},
         target_image={target_image},
         packages_to_install={packages_to_install},
-        output_component_file={output_component_file})
+        output_component_file={output_component_file},
+        pip_index_urls={pip_index_urls})
     def {func_name}():
         pass
     ''').format(
         base_image=repr(base_image),
         target_image=repr(target_image),
         packages_to_install=repr(packages_to_install),
         output_component_file=repr(output_component_file),
+        pip_index_urls=repr(pip_index_urls),
         func_name=func_name)
 
 
 def _write_file(filename: str, file_contents: str):
     filepath = pathlib.Path(filename)
     filepath.parent.mkdir(exist_ok=True, parents=True)
     filepath.write_text(file_contents)
@@ -256,14 +261,32 @@
             'kfp_config.ini',
             textwrap.dedent('''\
             [Components]
             train = train/train_component.py
 
             '''))
 
+    def test_nested_module_imports(self):
+        module_two = 'two = 2'
+        _write_file('module_two.py', module_two)
+
+        module_one = 'from module_two import two\none = 1'
+        _write_file('module_one.py', module_one)
+
+        component = _make_component(
+            func_name='comp', target_image='custom-image')
+        component = 'from module_one import one\n' + component
+        _write_components('component.py', component)
+
+        result = self.runner.invoke(
+            self.cli,
+            ['build', str(self._working_dir)],
+        )
+        self.assertEqual(result.exit_code, 0)
+
     def test_emptry_requirements_txt_file_is_generated(self):
         component = _make_component(
             func_name='train', target_image='custom-image')
         _write_components('components.py', component)
 
         result = self.runner.invoke(self.cli, ['build', str(self._working_dir)])
         self.assertEqual(result.exit_code, 0)
@@ -380,15 +403,21 @@
 
         result = self.runner.invoke(
             self.cli,
             ['build', str(self._working_dir)],
         )
         self.assertEqual(result.exit_code, 0)
 
-        self._docker_client.api.build.assert_called_once()
+        self._docker_client.api.build.assert_called_once_with(
+            path=mock.ANY,
+            dockerfile='Dockerfile',
+            tag=mock.ANY,
+            decode=True,
+            platform='linux/amd64',
+        )
         self._docker_client.images.push.assert_called_once_with(
             'custom-image', stream=True, decode=True)
 
     def test_docker_client_is_not_called_to_build_or_push(self):
         component = _make_component(
             func_name='train', target_image='custom-image')
         _write_components('components.py', component)
@@ -439,14 +468,74 @@
                 COPY runtime-requirements.txt runtime-requirements.txt
                 RUN pip install --no-cache-dir -r runtime-requirements.txt
 
                 RUN pip install --no-cache-dir kfp==1.2.3
                 COPY . .
                 '''))
 
+    @mock.patch('kfp.__version__', '1.2.3')
+    def test_docker_file_is_created_correctly_with_one_url(self):
+        component = _make_component(
+            func_name='train',
+            target_image='custom-image',
+            pip_index_urls=['https://pypi.org/simple'])
+        _write_components('components.py', component)
+
+        result = self.runner.invoke(
+            self.cli,
+            ['build', str(self._working_dir)],
+        )
+        self.assertEqual(result.exit_code, 0)
+        self._docker_client.api.build.assert_called_once()
+        self.assert_file_exists_and_contains(
+            'Dockerfile',
+            textwrap.dedent('''\
+                # Generated by KFP.
+
+                FROM python:3.7
+
+                WORKDIR /usr/local/src/kfp/components
+                COPY runtime-requirements.txt runtime-requirements.txt
+                RUN pip install --index-url https://pypi.org/simple --trusted-host https://pypi.org/simple --no-cache-dir -r runtime-requirements.txt
+
+                RUN pip install --index-url https://pypi.org/simple --trusted-host https://pypi.org/simple --no-cache-dir kfp==1.2.3
+                COPY . .
+                '''))
+
+    @mock.patch('kfp.__version__', '1.2.3')
+    def test_docker_file_is_created_correctly_with_two_urls(self):
+        component = _make_component(
+            func_name='train',
+            target_image='custom-image',
+            pip_index_urls=[
+                'https://pypi.org/simple', 'https://example.com/pypi/simple'
+            ])
+        _write_components('components.py', component)
+
+        result = self.runner.invoke(
+            self.cli,
+            ['build', str(self._working_dir)],
+        )
+        self.assertEqual(result.exit_code, 0)
+        self._docker_client.api.build.assert_called_once()
+        self.assert_file_exists_and_contains(
+            'Dockerfile',
+            textwrap.dedent('''\
+                # Generated by KFP.
+
+                FROM python:3.7
+
+                WORKDIR /usr/local/src/kfp/components
+                COPY runtime-requirements.txt runtime-requirements.txt
+                RUN pip install --index-url https://pypi.org/simple --trusted-host https://pypi.org/simple --extra-index-url https://example.com/pypi/simple --trusted-host https://example.com/pypi/simple --no-cache-dir -r runtime-requirements.txt
+
+                RUN pip install --index-url https://pypi.org/simple --trusted-host https://pypi.org/simple --extra-index-url https://example.com/pypi/simple --trusted-host https://example.com/pypi/simple --no-cache-dir kfp==1.2.3
+                COPY . .
+                '''))
+
     def test_existing_dockerfile_is_unchanged_by_default(self):
         component = _make_component(
             func_name='train', target_image='custom-image')
         _write_components('components.py', component)
         _write_file('Dockerfile', 'Existing Dockerfile contents')
 
         result = self.runner.invoke(
```

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/__init__.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/dev_env.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/dev_env_test.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/gcp.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/gcp_test.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/utility.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Lint as: python3
 # Copyright 2019 The Kubeflow Authors. All Rights Reserved.
 #
 # Licensed under the Apache License,Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -50,15 +51,15 @@
             process = subprocess.Popen(
                 command_list, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
             stdout, stderr = process.communicate()
             self._stdout = stdout.decode('utf-8')
             self._stderr = stderr.decode('utf-8')
             self._returncode = process.returncode
         except OSError as e:
-            self._stderr = str(e)
+            self._stderr = e
             self._stdout = ''
             self._returncode = e.errno
         self._parse_raw_input()
         return self
 
     def _parse_raw_input(self):
         """Parses the raw input and popluates _json and _parsed properies."""
```

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me/utility_test.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/utility_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# Lint as: python3
 # Copyright 2019 The Kubeflow Authors. All Rights Reserved.
 #
 # Licensed under the Apache License,Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,16 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND,either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for diagnose_me.utility."""
 
 import unittest
-
-from kfp.cli.diagnose_me import utility
+from kfp.deprecated.cli.diagnose_me import utility
 
 
 class UtilityTest(unittest.TestCase):
 
     def test_parse_raw_input_json(self):
         """Testing json stdout is correctly parsed."""
         response = utility.ExecutorResponse()
```

### Comparing `kfp-2.0.0b9/kfp/cli/diagnose_me_cli.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/dsl.py` & `kfp-2.0.0rc1/kfp/cli/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/experiment.py` & `kfp-2.0.0rc1/kfp/cli/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     output_format = ctx.obj['output']
 
     if (experiment_id is None) == (experiment_name is None):
         raise ValueError(either_option_required)
 
     if not experiment_id:
         experiment = client_obj.get_experiment(experiment_name=experiment_name)
-        experiment_id = experiment.id
+        experiment_id = experiment.experiment_id
 
     client_obj.archive_experiment(experiment_id=experiment_id)
     if experiment_id:
         experiment = client_obj.get_experiment(experiment_id=experiment_id)
     else:
         experiment = client_obj.get_experiment(experiment_name=experiment_name)
     output.print_output(
@@ -158,15 +158,15 @@
     output_format = ctx.obj['output']
 
     if (experiment_id is None) == (experiment_name is None):
         raise ValueError(either_option_required)
 
     if not experiment_id:
         experiment = client_obj.get_experiment(experiment_name=experiment_name)
-        experiment_id = experiment.id
+        experiment_id = experiment.experiment_id
 
     client_obj.unarchive_experiment(experiment_id=experiment_id)
     if experiment_id:
         experiment = client_obj.get_experiment(experiment_id=experiment_id)
     else:
         experiment = client_obj.get_experiment(experiment_name=experiment_name)
     output.print_output(
```

### Comparing `kfp-2.0.0b9/kfp/cli/output.py` & `kfp-2.0.0rc1/kfp/cli/output.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import dataclasses
 import datetime
 import enum
 import json
-from typing import Any, Dict, Union
+from typing import Any, Dict
 
 import click
 import kfp_server_api
 import tabulate
 
 KFP_TABLE_FORMAT = 'custom-simple'
 
@@ -41,25 +41,14 @@
 @enum.unique
 class OutputFormat(enum.Enum):
     """Enumerated class with the allowed output format constants."""
     table = 'table'
     json = 'json'
 
 
-RUN_STORAGE_STATE_MAP = {
-    kfp_server_api.ApiRunStorageState.AVAILABLE: 'Available',
-    kfp_server_api.ApiRunStorageState.ARCHIVED: 'Archived',
-}
-EXPERIMENT_STORAGE_STATE_MAP = {
-    kfp_server_api.ApiExperimentStorageState.AVAILABLE: 'Available',
-    kfp_server_api.ApiExperimentStorageState.ARCHIVED: 'Archived',
-    kfp_server_api.ApiExperimentStorageState.UNSPECIFIED: 'Unspecified',
-}
-
-
 def snake_to_header(string: str) -> str:
     """Converts a snake case string to a table header by replacing underscores
     with spaces and making uppercase.
 
     Args:
         string (str): The snake case string.
 
@@ -70,140 +59,127 @@
 
 
 @dataclasses.dataclass
 class ExperimentData:
     id: str
     name: str
     created_at: str
-    state: str
+    storage_state: str
 
 
-def transform_experiment(exp: kfp_server_api.ApiExperiment) -> Dict[str, Any]:
+def transform_experiment(
+        exp: kfp_server_api.V2beta1Experiment) -> Dict[str, Any]:
     return dataclasses.asdict(
         ExperimentData(
-            id=exp.id,
-            name=exp.name,
+            id=exp.experiment_id,
+            name=exp.display_name,
             created_at=exp.created_at.isoformat(),
-            state=EXPERIMENT_STORAGE_STATE_MAP.get(
-                exp.storage_state, EXPERIMENT_STORAGE_STATE_MAP[
-                    kfp_server_api.ApiExperimentStorageState.AVAILABLE])))
+            storage_state=exp.storage_state))
 
 
 @dataclasses.dataclass
 class PipelineData:
     id: str
     name: str
     created_at: str
-    default_version: str
 
 
-def transform_pipeline(pipeline: kfp_server_api.ApiPipeline) -> Dict[str, Any]:
-    default_version_id = pipeline.default_version.id if hasattr(
-        pipeline,
-        'default_version') and pipeline.default_version is not None and hasattr(
-            pipeline.default_version, 'id') else None
+def transform_pipeline(
+        pipeline: kfp_server_api.V2beta1Pipeline) -> Dict[str, Any]:
     return dataclasses.asdict(
         PipelineData(
-            id=pipeline.id,
-            name=pipeline.name,
+            id=pipeline.pipeline_id,
+            name=pipeline.display_name,
             created_at=pipeline.created_at.isoformat(),
-            default_version=default_version_id))
+        ))
 
 
 @dataclasses.dataclass
 class PipelineVersionData:
     id: str
     name: str
     created_at: str
     parent_id: str
 
 
 def transform_pipeline_version(
-        pipeline_version: kfp_server_api.ApiPipelineVersion) -> Dict[str, Any]:
-    parent_id = next(
-        rr for rr in pipeline_version.resource_references
-        if rr.relationship == kfp_server_api.ApiRelationship.OWNER).key.id
+        pipeline_version: kfp_server_api.V2beta1PipelineVersion
+) -> Dict[str, Any]:
     return dataclasses.asdict(
         PipelineVersionData(
-            id=pipeline_version.id,
-            name=pipeline_version.name,
+            id=pipeline_version.pipeline_version_id,
+            name=pipeline_version.display_name,
             created_at=pipeline_version.created_at.isoformat(),
-            parent_id=parent_id,
+            parent_id=pipeline_version.pipeline_id,
         ))
 
 
 @dataclasses.dataclass
 class RunData:
     id: str
     name: str
     created_at: str
-    status: str
     state: str
+    storage_state: str
 
 
-def transform_run(
-    run: Union[kfp_server_api.ApiRun, kfp_server_api.ApiRunDetail]
-) -> Dict[str, Any]:
+def transform_run(run: kfp_server_api.V2beta1Run) -> Dict[str, Any]:
     return dataclasses.asdict((RunData(
-        id=run.id,
-        name=run.name,
+        id=run.run_id,
+        name=run.display_name,
         created_at=run.created_at.isoformat(),
-        status=run.status,
-        state=RUN_STORAGE_STATE_MAP.get(
-            run.storage_state,
-            RUN_STORAGE_STATE_MAP[kfp_server_api.ApiRunStorageState.AVAILABLE]))
-                              ))
+        state=run.state,
+        storage_state=run.storage_state,
+    )))
 
 
 @dataclasses.dataclass
-class JobData:
+class RecurringRunData:
     id: str
     name: str
     created_at: str
     experiment_id: str
     status: str
 
 
-def transform_job(recurring_run: kfp_server_api.ApiJob) -> Dict[str, Any]:
-    experiment_id = next(
-        rr for rr in recurring_run.resource_references
-        if rr.key.type == kfp_server_api.ApiResourceType.EXPERIMENT).key.id
+def transform_recurring_run(
+        recurring_run: kfp_server_api.V2beta1RecurringRun) -> Dict[str, Any]:
     return dataclasses.asdict(
-        JobData(
-            id=recurring_run.id,
-            name=recurring_run.name,
+        RecurringRunData(
+            id=recurring_run.recurring_run_id,
+            name=recurring_run.display_name,
             created_at=recurring_run.created_at.isoformat(),
-            experiment_id=experiment_id,
+            experiment_id=recurring_run.experiment_id,
             status=recurring_run.status))
 
 
 @enum.unique
 class ModelType(enum.Enum):
     """Enumerated class with the allowed output format constants."""
     EXPERIMENT = 'EXPERIMENT'
     PIPELINE = 'PIPELINE'
     PIPELINE_VERSION = 'PIPELINE_VERSION'
     RUN = 'RUN'
-    JOB = 'JOB'
+    RECURRING_RUN = 'RECURRING_RUN'
 
 
 transformer_map = {
     ModelType.EXPERIMENT: transform_experiment,
     ModelType.PIPELINE: transform_pipeline,
     ModelType.PIPELINE_VERSION: transform_pipeline_version,
     ModelType.RUN: transform_run,
-    ModelType.JOB: transform_job,
+    ModelType.RECURRING_RUN: transform_recurring_run,
 }
 
 dataclass_map = {
     ModelType.EXPERIMENT: ExperimentData,
     ModelType.PIPELINE: PipelineData,
     ModelType.PIPELINE_VERSION: PipelineVersionData,
     ModelType.RUN: RunData,
-    ModelType.JOB: JobData,
+    ModelType.RECURRING_RUN: RecurringRunData,
 }
 
 
 class DatetimeEncoder(json.JSONEncoder):
     """JSON encoder for serializing datetime objects."""
 
     def default(self, obj: Any) -> Any:
```

### Comparing `kfp-2.0.0b9/kfp/cli/pipeline.py` & `kfp-2.0.0rc1/kfp/cli/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -187,33 +187,35 @@
     response = client_obj.list_pipeline_versions(
         pipeline_id,
         page_token=page_token,
         page_size=max_size,
         sort_by=sort_by,
         filter=filter)
     output.print_output(
-        response.versions or [],
-        output.ModelType.PIPELINE,
+        response.pipeline_versions or [],
+        output.ModelType.PIPELINE_VERSION,
         output_format,
     )
 
 
 @pipeline.command()
+@click.argument('pipeline-id')
 @click.argument('version-id')
 @click.pass_context
-def delete_version(ctx: click.Context, version_id: str):
+def delete_version(ctx: click.Context, pipeline_id: str, version_id: str):
     """Delete a version of a pipeline."""
     confirmation = f'Are you sure you want to delete pipeline version {version_id}?'
     if not click.confirm(confirmation):
         return
 
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
-    client_obj.delete_pipeline_version(version_id)
+    client_obj.delete_pipeline_version(
+        pipeline_id=pipeline_id, pipeline_version_id=version_id)
     output.print_deleted_text('pipeline version', version_id, output_format)
 
 
 @pipeline.command()
 @click.argument('pipeline-id')
 @click.pass_context
 def get(ctx: click.Context, pipeline_id: str):
@@ -226,22 +228,24 @@
         pipeline,
         output.ModelType.PIPELINE,
         output_format,
     )
 
 
 @pipeline.command()
+@click.argument('pipeline-id')
 @click.argument('version-id')
 @click.pass_context
-def get_version(ctx: click.Context, version_id: str):
+def get_version(ctx: click.Context, pipeline_id: str, version_id: str):
     """Get information about a version of a pipeline."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
-    version = client_obj.get_pipeline_version(version_id=version_id)
+    version = client_obj.get_pipeline_version(
+        pipeline_id=pipeline_id, pipeline_version_id=version_id)
     output.print_output(
         version,
         output.ModelType.PIPELINE,
         output_format,
     )
```

### Comparing `kfp-2.0.0b9/kfp/cli/recurring_run.py` & `kfp-2.0.0rc1/kfp/cli/recurring_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -131,15 +131,15 @@
             'Either of --interval-second or --cron-expression options is required.'
         )
 
     if (experiment_id is None) == (experiment_name is None):
         raise ValueError(either_option_required)
     if not experiment_id:
         experiment = client_obj.create_experiment(experiment_name)
-        experiment_id = experiment.id
+        experiment_id = experiment.experiment_id
 
     # Ensure we only split on the first equals char so the value can contain
     # equals signs too.
     split_args: List = [arg.split('=', 1) for arg in args or []]
     params: Dict[str, Any] = dict(split_args)
     recurring_run = client_obj.create_recurring_run(
         cron_expression=cron_expression,
@@ -155,15 +155,15 @@
         params=params,
         pipeline_package_path=pipeline_package_path,
         pipeline_id=pipeline_id,
         start_time=start_time,
         version_id=version_id)
     output.print_output(
         recurring_run,
-        output.ModelType.JOB,
+        output.ModelType.RECURRING_RUN,
         output_format,
     )
 
 
 @recurring_run.command()
 @click.option(
     '-e',
@@ -198,77 +198,79 @@
     response = client_obj.list_recurring_runs(
         experiment_id=experiment_id,
         page_token=page_token,
         page_size=max_size,
         sort_by=sort_by,
         filter=filter)
     output.print_output(
-        response.jobs or [],
-        output.ModelType.JOB,
+        response.recurring_runs or [],
+        output.ModelType.RECURRING_RUN,
         output_format,
     )
 
 
 @recurring_run.command()
-@click.argument('job-id')
+@click.argument('recurring-run-id')
 @click.pass_context
-def get(ctx: click.Context, job_id: str):
+def get(ctx: click.Context, recurring_run_id: str):
     """Get information about a recurring run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
-    recurring_run = client_obj.get_recurring_run(job_id)
+    recurring_run = client_obj.get_recurring_run(recurring_run_id)
     output.print_output(
         recurring_run,
-        output.ModelType.JOB,
+        output.ModelType.RECURRING_RUN,
         output_format,
     )
 
 
 @recurring_run.command()
-@click.argument('job-id')
+@click.argument('recurring-run-id')
 @click.pass_context
-def delete(ctx: click.Context, job_id: str):
+def delete(ctx: click.Context, recurring_run_id: str):
     """Delete a recurring run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
-    confirmation = f'Are you sure you want to delete job {job_id}?'
+    confirmation = f'Are you sure you want to delete job {recurring_run_id}?'
     if not click.confirm(confirmation):
         return
-    client_obj.delete_job(job_id)
-    output.print_deleted_text('job', job_id, output_format)
+    client_obj.delete_recurring_run(recurring_run_id)
+    output.print_deleted_text('recurring_run', recurring_run_id, output_format)
 
 
 @recurring_run.command()
-@click.argument('job-id')
+@click.argument('recurring-run-id')
 @click.pass_context
-def enable(ctx: click.Context, job_id: str):
+def enable(ctx: click.Context, recurring_run_id: str):
     """Enable a recurring run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
-    client_obj.enable_job(job_id=job_id)
+    client_obj.enable_recurring_run(recurring_run_id=recurring_run_id)
     # TODO: add wait option, since enable takes time to complete
-    recurring_run = client_obj.get_recurring_run(job_id=job_id)
+    recurring_run = client_obj.get_recurring_run(
+        recurring_run_id=recurring_run_id)
     output.print_output(
         recurring_run,
-        output.ModelType.JOB,
+        output.ModelType.RECURRING_RUN,
         output_format,
     )
 
 
 @recurring_run.command()
-@click.argument('job-id')
+@click.argument('recurring-run-id')
 @click.pass_context
-def disable(ctx: click.Context, job_id: str):
+def disable(ctx: click.Context, recurring_run_id: str):
     """Disable a recurring run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
-    client_obj.disable_job(job_id=job_id)
+    client_obj.disable_recurring_run(recurring_run_id=recurring_run_id)
     # TODO: add wait option, since disable takes time to complete
-    recurring_run = client_obj.get_recurring_run(job_id=job_id)
+    recurring_run = client_obj.get_recurring_run(
+        recurring_run_id=recurring_run_id)
     output.print_output(
         recurring_run,
-        output.ModelType.JOB,
+        output.ModelType.RECURRING_RUN,
         output_format,
     )
```

### Comparing `kfp-2.0.0b9/kfp/cli/run.py` & `kfp-2.0.0rc1/kfp/cli/run.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-import json
-import shutil
-import subprocess
 import sys
 import time
 from typing import List
 
 import click
 from kfp import client
 from kfp.cli import output
@@ -129,29 +126,29 @@
             err=True)
         sys.exit(1)
 
     arg_dict = dict(arg.split('=', maxsplit=1) for arg in args)
 
     experiment = client_obj.create_experiment(experiment_name)
     run = client_obj.run_pipeline(
-        experiment_id=experiment.id,
+        experiment_id=experiment.experiment_id,
         job_name=run_name,
         pipeline_package_path=package_file,
         params=arg_dict,
         pipeline_id=pipeline_id,
         version_id=version)
     if timeout > 0:
-        run_detail = client_obj.wait_for_run_completion(run.id, timeout)
+        run_detail = client_obj.wait_for_run_completion(run.run_id, timeout)
         output.print_output(
-            run_detail.run,
+            run_detail,
             output.ModelType.RUN,
             output_format,
         )
     else:
-        display_run(client_obj, namespace, run.id, watch, output_format)
+        display_run(client_obj, run.run_id, watch, output_format)
 
 
 @run.command()
 @click.option(
     '-w',
     '--watch',
     is_flag=True,
@@ -171,29 +168,29 @@
     namespace = ctx.obj['namespace']
     output_format = ctx.obj['output']
     if detail:
         output_format = 'json'
         click.echo(
             'The --detail/-d flag is deprecated. Please use --output=json instead.',
             err=True)
-    display_run(client_obj, namespace, run_id, watch, output_format)
+    display_run(client_obj, run_id, watch, output_format)
 
 
 @run.command()
 @click.argument('run-id')
 @click.pass_context
 def archive(ctx: click.Context, run_id: str):
     """Archive a pipeline run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
     client_obj.archive_run(run_id=run_id)
     run = client_obj.get_run(run_id=run_id)
     output.print_output(
-        run.run,
+        run,
         output.ModelType.RUN,
         output_format,
     )
 
 
 @run.command()
 @click.argument('run-id')
@@ -201,15 +198,15 @@
 def unarchive(ctx: click.Context, run_id: str):
     """Unarchive a pipeline run."""
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
     client_obj.unarchive_run(run_id=run_id)
     run = client_obj.get_run(run_id=run_id)
     output.print_output(
-        run.run,
+        run,
         output.ModelType.RUN,
         output_format,
     )
 
 
 @run.command()
 @click.argument('run-id')
@@ -224,47 +221,27 @@
     client_obj: client.Client = ctx.obj['client']
     output_format = ctx.obj['output']
 
     client_obj.delete_run(run_id=run_id)
     output.print_deleted_text('run', run_id, output_format)
 
 
-def display_run(client: client.Client, namespace: str, run_id: str, watch: bool,
+def display_run(client: client.Client, run_id: str, watch: bool,
                 output_format: str):
-    run = client.get_run(run_id).run
+    run = client.get_run(run_id)
 
     output.print_output(
         run,
         output.ModelType.RUN,
         output_format,
     )
     if not watch:
         return
-    argo_path = shutil.which('argo')
-    if not argo_path:
-        raise RuntimeError(
-            "argo isn't found in $PATH. It's necessary for watch. "
-            "Please make sure it's installed and available. "
-            'Installation instructions be found here - '
-            'https://github.com/argoproj/argo-workflows/releases')
-
-    argo_workflow_name = None
     while True:
         time.sleep(1)
         run_detail = client.get_run(run_id)
-        run = run_detail.run
-        if run_detail.pipeline_runtime and run_detail.pipeline_runtime.workflow_manifest:
-            manifest = json.loads(run_detail.pipeline_runtime.workflow_manifest)
-            if manifest['metadata'] and manifest['metadata']['name']:
-                argo_workflow_name = manifest['metadata']['name']
-                break
-        if run_detail.run.status in ['Succeeded', 'Skipped', 'Failed', 'Error']:
-            click.echo(f'Run is finished with status {run_detail.run.status}.')
+        run = run_detail
+        if run_detail.state in [
+                'SUCCEEDED', 'SKIPPED', 'FAILED', 'CANCELED', 'PAUSED'
+        ]:
+            click.echo(f'Run is finished with state {run_detail.state}.')
             return
-    if argo_workflow_name:
-        subprocess.run(
-            [argo_path, 'watch', argo_workflow_name, '-n', namespace])
-        output.print_output(
-            run,
-            output.ModelType.RUN,
-            output_format,
-        )
```

### Comparing `kfp-2.0.0b9/kfp/cli/utils/__init__.py` & `kfp-2.0.0rc1/kfp/cli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/aliased_plurals_group.py` & `kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/aliased_plurals_group_test.py` & `kfp-2.0.0rc1/kfp/cli/utils/aliased_plurals_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/deprecated_alias_group.py` & `kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/deprecated_alias_group_test.py` & `kfp-2.0.0rc1/kfp/cli/utils/deprecated_alias_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/parsing.py` & `kfp-2.0.0rc1/kfp/cli/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/cli/utils/parsing_test.py` & `kfp-2.0.0rc1/kfp/cli/utils/parsing_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/__init__.py` & `kfp-2.0.0rc1/kfp/client/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/auth.py` & `kfp-2.0.0rc1/kfp/client/auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/client.py` & `kfp-2.0.0rc1/kfp/deprecated/_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,152 +1,158 @@
-# Copyright 2022 The Kubeflow Authors
+# Copyright 2018 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""The SDK client for Kubeflow Pipelines API."""
 
-import copy
-import datetime
-import json
+import time
 import logging
+import json
 import os
 import re
 import tarfile
 import tempfile
-import time
-from types import ModuleType
-from typing import Any, Callable, Dict, List, Optional, Union
 import warnings
+import yaml
 import zipfile
+import datetime
+import copy
+from typing import Mapping, Callable, Optional
 
-from kfp import compiler
-from kfp.client import auth
-from kfp.client import set_volume_credentials
-from kfp.components import base_component
 import kfp_server_api
-import yaml
+
+from kfp.deprecated import dsl
+from kfp.deprecated.compiler import compiler
+from kfp.deprecated.compiler._k8s_helper import sanitize_k8s_name
+
+from kfp.deprecated._auth import get_auth_token, get_gcp_access_token
+from kfp_server_api import ApiException
 
 # Operators on scalar values. Only applies to one of |int_value|,
 # |long_value|, |string_value| or |timestamp_value|.
 _FILTER_OPERATIONS = {
-    'UNKNOWN': 0,
-    'EQUALS': 1,
-    'NOT_EQUALS': 2,
-    'GREATER_THAN': 3,
-    'GREATER_THAN_EQUALS': 5,
-    'LESS_THAN': 6,
-    'LESS_THAN_EQUALS': 7
+    "UNKNOWN": 0,
+    "EQUALS": 1,
+    "NOT_EQUALS": 2,
+    "GREATER_THAN": 3,
+    "GREATER_THAN_EQUALS": 5,
+    "LESS_THAN": 6,
+    "LESS_THAN_EQUALS": 7
 }
 
-KF_PIPELINES_ENDPOINT_ENV = 'KF_PIPELINES_ENDPOINT'
-KF_PIPELINES_UI_ENDPOINT_ENV = 'KF_PIPELINES_UI_ENDPOINT'
-KF_PIPELINES_DEFAULT_EXPERIMENT_NAME = 'KF_PIPELINES_DEFAULT_EXPERIMENT_NAME'
-KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME = 'KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME'
-KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_IAP_OAUTH2_CLIENT_ID'
-KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_ID'
-KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET'
 
+def _add_generated_apis(target_struct, api_module, api_client):
+    """Initializes a hierarchical API object based on the generated API module.
 
-class JobConfig:
+    PipelineServiceApi.create_pipeline becomes
+    target_struct.pipelines.create_pipeline
+    """
+    Struct = type('Struct', (), {})
 
-    def __init__(
-            self, spec: kfp_server_api.ApiPipelineSpec,
-            resource_references: kfp_server_api.ApiResourceReference) -> None:
-        self.spec = spec
-        self.resource_references = resource_references
+    def camel_case_to_snake_case(name):
+        import re
+        return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
 
+    for api_name in dir(api_module):
+        if not api_name.endswith('ServiceApi'):
+            continue
 
-class RunPipelineResult:
+        short_api_name = camel_case_to_snake_case(
+            api_name[0:-len('ServiceApi')]) + 's'
+        api_struct = Struct()
+        setattr(target_struct, short_api_name, api_struct)
+        service_api = getattr(api_module.api, api_name)
+        initialized_service_api = service_api(api_client)
+        for member_name in dir(initialized_service_api):
+            if member_name.startswith('_') or member_name.endswith(
+                    '_with_http_info'):
+                continue
 
-    def __init__(self, client: 'Client',
-                 run_info: kfp_server_api.ApiRun) -> None:
-        self._client = client
-        self.run_info = run_info
-        self.run_id = run_info.id
+            bound_member = getattr(initialized_service_api, member_name)
+            setattr(api_struct, member_name, bound_member)
+    models_struct = Struct()
+    for member_name in dir(api_module.models):
+        if not member_name[0].islower():
+            setattr(models_struct, member_name,
+                    getattr(api_module.models, member_name))
+    target_struct.api_models = models_struct
 
-    def wait_for_run_completion(self, timeout=None):
-        timeout = timeout or datetime.timedelta.max
-        return self._client.wait_for_run_completion(self.run_id, timeout)
 
-    def __repr__(self):
-        return f'RunPipelineResult(run_id={self.run_id})'
+KF_PIPELINES_ENDPOINT_ENV = 'KF_PIPELINES_ENDPOINT'
+KF_PIPELINES_UI_ENDPOINT_ENV = 'KF_PIPELINES_UI_ENDPOINT'
+KF_PIPELINES_DEFAULT_EXPERIMENT_NAME = 'KF_PIPELINES_DEFAULT_EXPERIMENT_NAME'
+KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME = 'KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME'
+KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_IAP_OAUTH2_CLIENT_ID'
+KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_ID'
+KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET'
 
 
-class Client:
-    """The KFP SDK client for the Kubeflow Pipelines backend API.
+class Client(object):
+    """API Client for KubeFlow Pipeline.
 
     Args:
-        host: Host name to use to talk to Kubeflow Pipelines. If not set,
-            the in-cluster service DNS name will be used, which only works if
-            the current environment is a pod in the same cluster (such as a
-            Jupyter instance spawned by Kubeflow's JupyterHub). (`More information on connecting. <https://www.kubeflow.org/docs/components/pipelines/sdk/connect-api/>`_)
-        client_id: Client ID used by Identity-Aware Proxy.
-        namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
-        other_client_id: Client ID used to obtain the auth codes and refresh
-            tokens (`reference <https://cloud.google.com/iap/docs/authentication-howto#authenticating_from_a_desktop_app>`_).
-        other_client_secret: Client secret used to obtain the auth codes and
-            refresh tokens.
-        existing_token: Authentication token to pass in directly. Used in cases where the token is
-            generated from outside the SDK.
-        cookies: CookieJar object containing cookies that will be passed to the
-            Pipelines API.
-        proxy: HTTP or HTTPS proxy server.
-        ssl_ca_cert: Certification for proxy.
-        kube_context: kubectl context to use. Must be a context listed in the kubeconfig file. Defaults to the current-context set within kubeconfig.
-        credentials: ``TokenCredentialsBase`` object which provides the logic to
-            populate the requests with credentials to authenticate against the
-            API server.
-        ui_host: Base URL to use to open the Kubeflow Pipelines UI. This is used
-            when running the client from a notebook to generate and print links.
-        verify_ssl: Whether to verify the server's TLS certificate.
+      host: The host name to use to talk to Kubeflow Pipelines. If not set, the in-cluster
+          service DNS name will be used, which only works if the current environment is a pod
+          in the same cluster (such as a Jupyter instance spawned by Kubeflow's
+          JupyterHub).
+          Set the host based on https://www.kubeflow.org/docs/components/pipelines/sdk/connect-api/.
+      client_id: The client ID used by Identity-Aware Proxy.
+      namespace: The namespace where the kubeflow pipeline system is run.
+      other_client_id: The client ID used to obtain the auth codes and refresh tokens.
+          Reference: https://cloud.google.com/iap/docs/authentication-howto#authenticating_from_a_desktop_app.
+      other_client_secret: The client secret used to obtain the auth codes and refresh tokens.
+      existing_token: Pass in token directly, it's used for cases better get token outside of SDK, e.x. GCP Cloud Functions
+          or caller already has a token
+      cookies: CookieJar object containing cookies that will be passed to the pipelines API.
+      proxy: HTTP or HTTPS proxy server
+      ssl_ca_cert: Cert for proxy
+      kube_context: String name of context within kubeconfig to use, defaults to the current-context set within kubeconfig.
+      credentials: A TokenCredentialsBase object which provides the logic to
+          populate the requests with credentials to authenticate against the API
+          server.
+      ui_host: Base url to use to open the Kubeflow Pipelines UI. This is used when running the client from a notebook to generate and
+          print links.
+      verify_ssl: A boolean indication to verify the servers TLS certificate or not.
     """
 
     # in-cluster DNS name of the pipeline service
-    _IN_CLUSTER_DNS_NAME = 'ml-pipeline.{}.svc.cluster.local:8888'
-    _KUBE_PROXY_PATH = 'api/v1/namespaces/{}/services/ml-pipeline:http/proxy/'
+    IN_CLUSTER_DNS_NAME = 'ml-pipeline.{}.svc.cluster.local:8888'
+    KUBE_PROXY_PATH = 'api/v1/namespaces/{}/services/ml-pipeline:http/proxy/'
 
     # Auto populated path in pods
     # https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster/#accessing-the-api-from-a-pod
     # https://kubernetes.io/docs/reference/access-authn-authz/service-accounts-admin/#serviceaccount-admission-controller
-    _NAMESPACE_PATH = '/var/run/secrets/kubernetes.io/serviceaccount/namespace'
+    NAMESPACE_PATH = '/var/run/secrets/kubernetes.io/serviceaccount/namespace'
 
-    _LOCAL_KFP_CONTEXT = os.path.expanduser('~/.config/kfp/context.json')
+    LOCAL_KFP_CONTEXT = os.path.expanduser('~/.config/kfp/context.json')
 
     # TODO: Wrap the configurations for different authentication methods.
-    def __init__(
-        self,
-        host: Optional[str] = None,
-        client_id: Optional[str] = None,
-        namespace: str = 'kubeflow',
-        other_client_id: Optional[str] = None,
-        other_client_secret: Optional[str] = None,
-        existing_token: Optional[str] = None,
-        cookies: Optional[str] = None,
-        proxy: Optional[str] = None,
-        ssl_ca_cert: Optional[str] = None,
-        kube_context: Optional[str] = None,
-        credentials: Optional[str] = None,
-        ui_host: Optional[str] = None,
-        verify_ssl: Optional[bool] = None,
-    ) -> None:
+    def __init__(self,
+                 host=None,
+                 client_id=None,
+                 namespace='kubeflow',
+                 other_client_id=None,
+                 other_client_secret=None,
+                 existing_token=None,
+                 cookies=None,
+                 proxy=None,
+                 ssl_ca_cert=None,
+                 kube_context=None,
+                 credentials=None,
+                 ui_host=None,
+                 verify_ssl=None):
         """Create a new instance of kfp client."""
-        warnings.warn(
-            'This client only works with Kubeflow Pipeline v2.0.0-alpha.0 '
-            'and later versions.',
-            category=FutureWarning)
-
         host = host or os.environ.get(KF_PIPELINES_ENDPOINT_ENV)
         self._uihost = os.environ.get(KF_PIPELINES_UI_ENDPOINT_ENV, ui_host or
                                       host)
         client_id = client_id or os.environ.get(
             KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV)
         other_client_id = other_client_id or os.environ.get(
             KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV)
@@ -164,53 +170,48 @@
         # context settings for current client instance
         if namespace != 'kubeflow':
             self._context_setting['namespace'] = namespace
 
         self._existing_config = config
         if cookies is None:
             cookies = self._context_setting.get('client_authentication_cookie')
-        api_client = kfp_server_api.ApiClient(
+        api_client = kfp_server_api.api_client.ApiClient(
             config,
             cookie=cookies,
             header_name=self._context_setting.get(
                 'client_authentication_header_name'),
             header_value=self._context_setting.get(
                 'client_authentication_header_value'))
         _add_generated_apis(self, kfp_server_api, api_client)
-        self._job_api = kfp_server_api.JobServiceApi(api_client)
-        self._run_api = kfp_server_api.RunServiceApi(api_client)
-        self._experiment_api = kfp_server_api.ExperimentServiceApi(api_client)
-        self._pipelines_api = kfp_server_api.PipelineServiceApi(api_client)
-        self._upload_api = kfp_server_api.PipelineUploadServiceApi(api_client)
-        self._healthz_api = kfp_server_api.HealthzServiceApi(api_client)
+        self._job_api = kfp_server_api.api.job_service_api.JobServiceApi(
+            api_client)
+        self._run_api = kfp_server_api.api.run_service_api.RunServiceApi(
+            api_client)
+        self._experiment_api = kfp_server_api.api.experiment_service_api.ExperimentServiceApi(
+            api_client)
+        self._pipelines_api = kfp_server_api.api.pipeline_service_api.PipelineServiceApi(
+            api_client)
+        self._upload_api = kfp_server_api.api.PipelineUploadServiceApi(
+            api_client)
+        self._healthz_api = kfp_server_api.api.healthz_service_api.HealthzServiceApi(
+            api_client)
         if not self._context_setting['namespace'] and self.get_kfp_healthz(
         ).multi_user is True:
             try:
-                with open(Client._NAMESPACE_PATH, 'r') as f:
+                with open(Client.NAMESPACE_PATH, 'r') as f:
                     current_namespace = f.read()
                     self.set_user_namespace(current_namespace)
             except FileNotFoundError:
                 logging.info(
                     'Failed to automatically set namespace.', exc_info=False)
 
-    def _load_config(
-        self,
-        host: Optional[str],
-        client_id: Optional[str],
-        namespace: str,
-        other_client_id: Optional[str],
-        other_client_secret: Optional[str],
-        existing_token: Optional[str],
-        proxy: Optional[str],
-        ssl_ca_cert: Optional[str],
-        kube_context: Optional[str],
-        credentials: Optional[str],
-        verify_ssl: Optional[bool],
-    ) -> kfp_server_api.Configuration:
-        config = kfp_server_api.Configuration()
+    def _load_config(self, host, client_id, namespace, other_client_id,
+                     other_client_secret, existing_token, proxy, ssl_ca_cert,
+                     kube_context, credentials, verify_ssl):
+        config = kfp_server_api.configuration.Configuration()
 
         if proxy:
             # https://github.com/kubeflow/pipelines/blob/c6ac5e0b1fd991e19e96419f0f508ec0a4217c29/backend/api/python_http_client/kfp_server_api/rest.py#L100
             config.proxy = proxy
         if verify_ssl is not None:
             config.verify_ssl = verify_ssl
 
@@ -218,35 +219,33 @@
             config.ssl_ca_cert = ssl_ca_cert
 
         host = host or ''
 
         # Defaults to 'https' if host does not contain 'http' or 'https' protocol.
         if host and not host.startswith('http'):
             warnings.warn(
-                f'The host {host} does not contain the "http" or "https" protocol. Defaults to "https".'
-            )
+                'The host %s does not contain the "http" or "https" protocol.'
+                ' Defaults to "https".' % host)
             host = 'https://' + host
 
         # Preprocess the host endpoint to prevent some common user mistakes.
         if not client_id:
             # always preserving the protocol (http://localhost requires it)
             host = host.rstrip('/')
 
         if host:
             config.host = host
 
         token = None
 
-        # "existing_token" is designed to accept token generated outside of SDK.
+        # "existing_token" is designed to accept token generated outside of SDK. Here is an example.
         #
         # https://cloud.google.com/functions/docs/securing/function-identity
         # https://cloud.google.com/endpoints/docs/grpc/service-account-authentication
         #
-        # Here is an example.
-        #
         # import requests
         # import kfp
         #
         # def get_access_token():
         #     url = 'http://metadata.google.internal/computeMetadata/v1/instance/service-accounts/default/token'
         #     r = requests.get(url, headers={'Metadata-Flavor': 'Google'})
         #     r.raise_for_status()
@@ -255,596 +254,543 @@
         #
         # client = kfp.Client(host='<KFPHost>', existing_token=get_access_token())
         #
         if existing_token:
             token = existing_token
             self._is_refresh_token = False
         elif client_id:
-            token, self._is_refresh_token = auth.get_auth_token(
-                client_id, other_client_id, other_client_secret)
+            token = get_auth_token(client_id, other_client_id,
+                                   other_client_secret)
+            self._is_refresh_token = True
         elif self._is_inverse_proxy_host(host):
-            token = auth.get_gcp_access_token()
+            token = get_gcp_access_token()
             self._is_refresh_token = False
         elif credentials:
             config.api_key['authorization'] = 'placeholder'
             config.api_key_prefix['authorization'] = 'Bearer'
             config.refresh_api_key_hook = credentials.refresh_api_key_hook
 
         if token:
             config.api_key['authorization'] = token
             config.api_key_prefix['authorization'] = 'Bearer'
             return config
 
         if host:
-            # if host is explicitly set with auth token, it's probably a port
-            # forward address.
+            # if host is explicitly set with auth token, it's probably a port forward address.
             return config
 
         import kubernetes as k8s
         in_cluster = True
         try:
             k8s.config.load_incluster_config()
         except:
             in_cluster = False
 
         if in_cluster:
-            config.host = Client._IN_CLUSTER_DNS_NAME.format(namespace)
+            config.host = Client.IN_CLUSTER_DNS_NAME.format(namespace)
             config = self._get_config_with_default_credentials(config)
             return config
 
         try:
             k8s.config.load_kube_config(
                 client_configuration=config, context=kube_context)
         except:
             print('Failed to load kube config.')
             return config
 
         if config.host:
-            config.host = config.host + '/' + Client._KUBE_PROXY_PATH.format(
+            config.host = config.host + '/' + Client.KUBE_PROXY_PATH.format(
                 namespace)
         return config
 
     def _is_inverse_proxy_host(self, host):
         if host:
             return re.match(r'\S+.googleusercontent.com/{0,1}$', host)
         if re.match(r'\w+', host):
             warnings.warn(
-                f'The received host is {host}, please include the full endpoint'
-                ' address (with ".(pipelines/notebooks).googleusercontent.com")'
-            )
+                'The received host is %s, please include the full endpoint address '
+                '(with ".(pipelines/notebooks).googleusercontent.com")' % host)
         return False
 
-    def _is_ipython(self) -> bool:
+    def _is_ipython(self):
         """Returns whether we are running in notebook."""
         try:
             import IPython
             ipy = IPython.get_ipython()
             if ipy is None:
                 return False
         except ImportError:
             return False
 
         return True
 
-    def _get_url_prefix(self) -> str:
+    def _get_url_prefix(self):
         if self._uihost:
             # User's own connection.
             if self._uihost.startswith('http://') or self._uihost.startswith(
                     'https://'):
                 return self._uihost
             else:
                 return 'http://' + self._uihost
 
         # In-cluster pod. We could use relative URL.
         return '/pipeline'
 
-    def _load_context_setting_or_default(self) -> None:
-        if os.path.exists(Client._LOCAL_KFP_CONTEXT):
-            with open(Client._LOCAL_KFP_CONTEXT, 'r') as f:
+    def _load_context_setting_or_default(self):
+        if os.path.exists(Client.LOCAL_KFP_CONTEXT):
+            with open(Client.LOCAL_KFP_CONTEXT, 'r') as f:
                 self._context_setting = json.load(f)
         else:
             self._context_setting = {
                 'namespace': '',
             }
 
-    def _refresh_api_client_token(self) -> None:
+    def _refresh_api_client_token(self):
         """Refreshes the existing token associated with the kfp_api_client."""
         if getattr(self, '_is_refresh_token', None):
             return
 
-        new_token = auth.get_gcp_access_token()
+        new_token = get_gcp_access_token()
         self._existing_config.api_key['authorization'] = new_token
 
-    def _get_config_with_default_credentials(
-            self, config: kfp_server_api.Configuration
-    ) -> kfp_server_api.Configuration:
+    def _get_config_with_default_credentials(self, config):
         """Apply default credentials to the configuration object.
 
         This method accepts a Configuration object and extends it with
         some default credentials interface.
         """
         # XXX: The default credentials are audience-based service account tokens
         # projected by the kubelet (ServiceAccountTokenVolumeCredentials). As we
         # implement more and more credentials, we can have some heuristic and
         # choose from a number of options.
         # See https://github.com/kubeflow/pipelines/pull/5287#issuecomment-805654121
-        credentials = set_volume_credentials.ServiceAccountTokenVolumeCredentials(
-        )
+        from kfp.deprecated import auth
+        credentials = auth.ServiceAccountTokenVolumeCredentials()
         config_copy = copy.deepcopy(config)
 
         try:
             credentials.refresh_api_key_hook(config_copy)
         except Exception:
-            logging.warning('Failed to set up default credentials. Proceeding'
-                            ' without credentials...')
+            logging.warning("Failed to set up default credentials. Proceeding"
+                            " without credentials...")
             return config
 
         config.refresh_api_key_hook = credentials.refresh_api_key_hook
         config.api_key_prefix['authorization'] = 'Bearer'
         config.refresh_api_key_hook(config)
         return config
 
-    def set_user_namespace(self, namespace: str) -> None:
-        """Sets the namespace in the Kuberenetes cluster to use.
+    def set_user_namespace(self, namespace: str):
+        """Set user namespace into local context setting file.
 
-        This function should only be used when Kubeflow Pipelines is in the
-        multi-user mode.
+        This function should only be used when Kubeflow Pipelines is in the multi-user mode.
 
         Args:
-            namespace: Namespace to use within the Kubernetes cluster (namespace containing the Kubeflow Pipelines deployment).
+          namespace: kubernetes namespace the user has access to.
         """
         self._context_setting['namespace'] = namespace
-        if not os.path.exists(os.path.dirname(Client._LOCAL_KFP_CONTEXT)):
-            os.makedirs(os.path.dirname(Client._LOCAL_KFP_CONTEXT))
-        with open(Client._LOCAL_KFP_CONTEXT, 'w') as f:
+        if not os.path.exists(os.path.dirname(Client.LOCAL_KFP_CONTEXT)):
+            os.makedirs(os.path.dirname(Client.LOCAL_KFP_CONTEXT))
+        with open(Client.LOCAL_KFP_CONTEXT, 'w') as f:
             json.dump(self._context_setting, f)
 
-    def get_kfp_healthz(
-            self,
-            sleep_duration: int = 5) -> kfp_server_api.ApiGetHealthzResponse:
-        """Gets healthz info for KFP deployment.
-
-        Args:
-            sleep_duration: Time in seconds between retries.
+    def get_kfp_healthz(self) -> kfp_server_api.ApiGetHealthzResponse:
+        """Gets healthz info of KFP deployment.
 
         Returns:
-            JSON response from the healthz endpoint.
+          response: json formatted response from the healtz endpoint.
         """
         count = 0
         response = None
         max_attempts = 5
         while not response:
             count += 1
             if count > max_attempts:
                 raise TimeoutError(
-                    f'Failed getting healthz endpoint after {max_attempts} attempts.'
-                )
-
+                    'Failed getting healthz endpoint after {} attempts.'.format(
+                        max_attempts))
             try:
-                return self._healthz_api.get_healthz()
+                response = self._healthz_api.get_healthz()
+                return response
             # ApiException, including network errors, is the only type that may
             # recover after retry.
             except kfp_server_api.ApiException:
                 # logging.exception also logs detailed info about the ApiException
                 logging.exception(
-                    f'Failed to get healthz info attempt {count} of {max_attempts}.'
-                )
-                time.sleep(sleep_duration)
+                    'Failed to get healthz info attempt {} of 5.'.format(count))
+                time.sleep(5)
 
     def get_user_namespace(self) -> str:
-        """Gets user namespace in context config.
+        """Get user namespace in context config.
 
         Returns:
-            Kubernetes namespace from the local context file or empty if it
-            wasn't set.
+          namespace: kubernetes namespace from the local context file or empty if it wasn't set.
         """
         return self._context_setting['namespace']
 
     def create_experiment(
             self,
             name: str,
             description: str = None,
             namespace: str = None) -> kfp_server_api.ApiExperiment:
-        """Creates a new experiment.
+        """Create a new experiment.
 
         Args:
-            name: Name of the experiment.
-            description: Description of the experiment.
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+          name: The name of the experiment.
+          description: Description of the experiment.
+          namespace: Kubernetes namespace where the experiment should be created.
+            For single user deployment, leave it as None;
+            For multi user, input a namespace where the user is authorized.
 
         Returns:
-            ``ApiExperiment`` object.
+          An Experiment object. Most important field is id.
         """
         namespace = namespace or self.get_user_namespace()
         experiment = None
         try:
             experiment = self.get_experiment(
                 experiment_name=name, namespace=namespace)
         except ValueError as error:
             # Ignore error if the experiment does not exist.
             if not str(error).startswith('No experiment is found with name'):
                 raise error
 
         if not experiment:
-            logging.info(f'Creating experiment {name}.')
+            logging.info('Creating experiment {}.'.format(name))
 
             resource_references = []
-            if namespace is not None:
-                key = kfp_server_api.ApiResourceKey(
-                    id=namespace, type=kfp_server_api.ApiResourceType.NAMESPACE)
-                reference = kfp_server_api.ApiResourceReference(
-                    key=key, relationship=kfp_server_api.ApiRelationship.OWNER)
+            if namespace:
+                key = kfp_server_api.models.ApiResourceKey(
+                    id=namespace,
+                    type=kfp_server_api.models.ApiResourceType.NAMESPACE)
+                reference = kfp_server_api.models.ApiResourceReference(
+                    key=key,
+                    relationship=kfp_server_api.models.ApiRelationship.OWNER)
                 resource_references.append(reference)
 
-            experiment = kfp_server_api.ApiExperiment(
+            experiment = kfp_server_api.models.ApiExperiment(
                 name=name,
                 description=description,
                 resource_references=resource_references)
             experiment = self._experiment_api.create_experiment(body=experiment)
 
-        link = f'{self._get_url_prefix()}/#/experiments/details/{experiment.id}'
         if self._is_ipython():
             import IPython
-            html = f'<a href="{link}" target="_blank" >Experiment details</a>.'
+            html = \
+                ('<a href="%s/#/experiments/details/%s" target="_blank" >Experiment details</a>.'
+                % (self._get_url_prefix(), experiment.id))
             IPython.display.display(IPython.display.HTML(html))
-        else:
-            print(f'Experiment details: {link}')
-
         return experiment
 
-    def get_pipeline_id(self, name: str) -> Optional[str]:
-        """Gets the ID of a pipeline by its name.
+    def get_pipeline_id(self, name) -> Optional[str]:
+        """Find the id of a pipeline by name.
 
         Args:
-            name: Pipeline name.
+          name: Pipeline name.
 
         Returns:
-            The pipeline ID if a pipeline with the name exists.
+          Returns the pipeline id if a pipeline with the name exists.
         """
         pipeline_filter = json.dumps({
-            'predicates': [{
-                'op': _FILTER_OPERATIONS['EQUALS'],
-                'key': 'name',
-                'stringValue': name,
+            "predicates": [{
+                "op": _FILTER_OPERATIONS["EQUALS"],
+                "key": "name",
+                "stringValue": name,
             }]
         })
         result = self._pipelines_api.list_pipelines(filter=pipeline_filter)
         if result.pipelines is None:
             return None
         if len(result.pipelines) == 1:
             return result.pipelines[0].id
         elif len(result.pipelines) > 1:
             raise ValueError(
-                f'Multiple pipelines with the name: {name} found, the name needs to be unique'
-            )
+                "Multiple pipelines with the name: {} found, the name needs to be unique"
+                .format(name))
         return None
 
     def list_experiments(
         self,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
         namespace: Optional[str] = None,
         filter: Optional[str] = None
     ) -> kfp_server_api.ApiListExperimentsResponse:
-        """Lists experiments.
+        """List experiments.
 
         Args:
-            page_token: Page token for obtaining page from paginated response.
-            page_size: Size of the page.
-            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'name desc'``.
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
-            filter: A url-encoded, JSON-serialized Filter protocol buffer
-                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/backend/api/filter.proto>`_). For a list of all filter operations ``'op'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
-
-                  ::
-
-                    json.dumps({
-                        "predicates": [{
-                            "op": _FILTER_OPERATIONS["EQUALS"],
-                            "key": "name",
-                            "stringValue": "my-name",
-                        }]
-                    })
+          page_token: Token for starting of the page.
+          page_size: Size of the page.
+          sort_by: Can be '[field_name]', '[field_name] desc'. For example, 'name desc'.
+          namespace: Kubernetes namespace where the experiment was created.
+            For single user deployment, leave it as None;
+            For multi user, input a namespace where the user is authorized.
+          filter: A url-encoded, JSON-serialized Filter protocol buffer
+            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+
+            An example filter string would be:
+
+                # For the list of filter operations please see:
+                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
+                json.dumps({
+                    "predicates": [{
+                        "op": _FILTER_OPERATIONS["EQUALS"],
+                        "key": "name",
+                        "stringValue": "my-name",
+                    }]
+                })
 
         Returns:
-            ``ApiListExperimentsResponse`` object.
+          A response object including a list of experiments and next page token.
         """
         namespace = namespace or self.get_user_namespace()
-        return self._experiment_api.list_experiment(
+        response = self._experiment_api.list_experiment(
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
-            resource_reference_key_type=kfp_server_api.ApiResourceType
-            .NAMESPACE,
+            resource_reference_key_type=kfp_server_api.models.api_resource_type
+            .ApiResourceType.NAMESPACE,
             resource_reference_key_id=namespace,
             filter=filter)
+        return response
 
     def get_experiment(self,
                        experiment_id=None,
                        experiment_name=None,
                        namespace=None) -> kfp_server_api.ApiExperiment:
-        """Gets details of an experiment.
+        """Get details of an experiment.
 
-        Either ``experiment_id`` or ``experiment_name`` is required.
+        Either experiment_id or experiment_name is required
 
         Args:
-            experiment_id: ID of the experiment.
-            experiment_name: Name of the experiment.
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+          experiment_id: Id of the experiment. (Optional)
+          experiment_name: Name of the experiment. (Optional)
+          namespace: Kubernetes namespace where the experiment was created.
+            For single user deployment, leave it as None;
+            For multi user, input the namespace where the user is authorized.
 
         Returns:
-            ``ApiExperiment`` object.
+          A response object including details of a experiment.
+
+        Raises:
+          kfp_server_api.ApiException: If experiment is not found or None of the arguments is provided
         """
         namespace = namespace or self.get_user_namespace()
         if experiment_id is None and experiment_name is None:
             raise ValueError(
                 'Either experiment_id or experiment_name is required')
         if experiment_id is not None:
             return self._experiment_api.get_experiment(id=experiment_id)
         experiment_filter = json.dumps({
-            'predicates': [{
-                'op': _FILTER_OPERATIONS['EQUALS'],
-                'key': 'name',
-                'stringValue': experiment_name,
+            "predicates": [{
+                "op": _FILTER_OPERATIONS["EQUALS"],
+                "key": "name",
+                "stringValue": experiment_name,
             }]
         })
-        if namespace is not None:
+        if namespace:
             result = self._experiment_api.list_experiment(
                 filter=experiment_filter,
-                resource_reference_key_type=kfp_server_api.ApiResourceType
-                .NAMESPACE,
+                resource_reference_key_type=kfp_server_api.models
+                .api_resource_type.ApiResourceType.NAMESPACE,
                 resource_reference_key_id=namespace)
         else:
             result = self._experiment_api.list_experiment(
                 filter=experiment_filter)
         if not result.experiments:
             raise ValueError(
-                f'No experiment is found with name {experiment_name}.')
+                'No experiment is found with name {}.'.format(experiment_name))
         if len(result.experiments) > 1:
             raise ValueError(
-                f'Multiple experiments is found with name {experiment_name}.')
+                'Multiple experiments is found with name {}.'.format(
+                    experiment_name))
         return result.experiments[0]
 
-    def archive_experiment(self, experiment_id: str) -> dict:
-        """Archives an experiment.
+    def archive_experiment(self, experiment_id: str):
+        """Archive experiment.
 
         Args:
-            experiment_id: ID of the experiment.
+          experiment_id: id of the experiment.
 
-        Returns:
-            Empty dictionary.
+        Raises:
+          kfp_server_api.ApiException: If experiment is not found.
         """
-        return self._experiment_api.archive_experiment(id=experiment_id)
-
-    def unarchive_experiment(self, experiment_id: str) -> dict:
-        """Unarchives an experiment.
+        self._experiment_api.archive_experiment(experiment_id)
 
-        Args:
-            experiment_id: ID of the experiment.
-
-        Returns:
-            Empty dictionary.
-        """
-        return self._experiment_api.unarchive_experiment(id=experiment_id)
-
-    def delete_experiment(self, experiment_id: str) -> dict:
+    def delete_experiment(self, experiment_id):
         """Delete experiment.
 
         Args:
-            experiment_id: ID of the experiment.
+          experiment_id: id of the experiment.
 
         Returns:
-            Empty dictionary.
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          kfp_server_api.ApiException: If experiment is not found.
         """
         return self._experiment_api.delete_experiment(id=experiment_id)
 
-    def _extract_pipeline_yaml(self, package_file: str) -> dict:
+    def _extract_pipeline_yaml(self, package_file):
 
-        def _choose_pipeline_file(file_list: List[str]) -> str:
-            pipeline_files = [
-                file for file in file_list if file.endswith('.yaml')
-            ]
-            if not pipeline_files:
+        def _choose_pipeline_yaml_file(file_list) -> str:
+            yaml_files = [file for file in file_list if file.endswith('.yaml')]
+            if len(yaml_files) == 0:
                 raise ValueError(
                     'Invalid package. Missing pipeline yaml file in the package.'
                 )
 
-            if 'pipeline.yaml' in pipeline_files:
+            if 'pipeline.yaml' in yaml_files:
                 return 'pipeline.yaml'
-            elif len(pipeline_files) == 1:
-                return pipeline_files[0]
             else:
+                if len(yaml_files) == 1:
+                    return yaml_files[0]
                 raise ValueError(
-                    'Invalid package. There is no pipeline.json file or there '
-                    'are multiple yaml files.')
+                    'Invalid package. There is no pipeline.yaml file and there are multiple yaml files.'
+                )
 
         if package_file.endswith('.tar.gz') or package_file.endswith('.tgz'):
-            with tarfile.open(package_file, 'r:gz') as tar:
+            with tarfile.open(package_file, "r:gz") as tar:
                 file_names = [member.name for member in tar if member.isfile()]
-                pipeline_file = _choose_pipeline_file(file_names)
-                with tar.extractfile(
-                        tar.getmember(pipeline_file)) as f:  # type: ignore
+                pipeline_yaml_file = _choose_pipeline_yaml_file(file_names)
+                with tar.extractfile(tar.getmember(pipeline_yaml_file)) as f:
                     return yaml.safe_load(f)
         elif package_file.endswith('.zip'):
             with zipfile.ZipFile(package_file, 'r') as zip:
-                pipeline_file = _choose_pipeline_file(zip.namelist())
-                with zip.open(pipeline_file) as f:
+                pipeline_yaml_file = _choose_pipeline_yaml_file(zip.namelist())
+                with zip.open(pipeline_yaml_file) as f:
                     return yaml.safe_load(f)
         elif package_file.endswith('.yaml') or package_file.endswith('.yml'):
             with open(package_file, 'r') as f:
                 return yaml.safe_load(f)
         else:
             raise ValueError(
-                f'The package_file {package_file} should end with one of the '
-                'following formats: [.tar.gz, .tgz, .zip, .yaml, .yml].')
+                'The package_file ' + package_file +
+                ' should end with one of the following formats: [.tar.gz, .tgz, .zip, .yaml, .yml]'
+            )
 
-    def _override_caching_options(self, pipeline_obj: dict,
-                                  enable_caching: bool) -> None:
-        """Overrides caching options.
-
-        Args:
-            pipeline_obj: Dict object parsed from the yaml file.
-            enable_caching: Overrides options, one of 'True', 'False'.
-        """
-        for _, task in pipeline_obj['root']['dag']['tasks'].items():
-            if 'cachingOptions' in task:
-                task['cachingOptions']['enableCache'] = enable_caching
-            else:
-                task['cachingOptions'] = {'enableCache': enable_caching}
+    def _override_caching_options(self, workflow: dict, enable_caching: bool):
+        templates = workflow['spec']['templates']
+        for template in templates:
+            if 'metadata' in template \
+               and 'labels' in template['metadata'] \
+               and 'pipelines.kubeflow.org/enable_caching' in template['metadata']['labels']:
+                template['metadata']['labels'][
+                    'pipelines.kubeflow.org/enable_caching'] = str(
+                        enable_caching).lower()
 
     def list_pipelines(
         self,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
         filter: Optional[str] = None
     ) -> kfp_server_api.ApiListPipelinesResponse:
-        """Lists pipelines.
+        """List pipelines.
 
         Args:
-            page_token: Page token for obtaining page from paginated response.
-            page_size: Size of the page.
-            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'name desc'``.
-            filter: A url-encoded, JSON-serialized Filter protocol buffer
-                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/backend/api/filter.proto>`_). For a list of all filter operations ``'op'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
+          page_token: Token for starting of the page.
+          page_size: Size of the page.
+          sort_by: one of 'field_name', 'field_name desc'. For example, 'name desc'.
+          filter: A url-encoded, JSON-serialized Filter protocol buffer
+            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
 
-                  ::
+            An example filter string would be:
 
-                    json.dumps({
-                        "predicates": [{
-                            "op": _FILTER_OPERATIONS["EQUALS"],
-                            "key": "name",
-                            "stringValue": "my-name",
-                        }]
-                    })
+                # For the list of filter operations please see:
+                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
+                json.dumps({
+                    "predicates": [{
+                        "op": _FILTER_OPERATIONS["EQUALS"],
+                        "key": "name",
+                        "stringValue": "my-name",
+                    }]
+                })
 
         Returns:
-            ``ApiListPipelinesResponse`` object.
+          A response object including a list of pipelines and next page token.
         """
         return self._pipelines_api.list_pipelines(
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
             filter=filter)
 
     # TODO: provide default namespace, similar to kubectl default namespaces.
     def run_pipeline(
         self,
         experiment_id: str,
         job_name: str,
         pipeline_package_path: Optional[str] = None,
-        params: Optional[Dict[str, Any]] = None,
+        params: Optional[dict] = None,
         pipeline_id: Optional[str] = None,
         version_id: Optional[str] = None,
         pipeline_root: Optional[str] = None,
-        enable_caching: Optional[bool] = None,
+        enable_caching: Optional[str] = None,
         service_account: Optional[str] = None,
     ) -> kfp_server_api.ApiRun:
-        """Runs a specified pipeline.
+        """Run a specified pipeline.
 
         Args:
-            experiment_id: ID of an experiment.
-            job_name: Name of the job.
-            pipeline_package_path: Local path of the pipeline package (the
-                filename should end with one of the following .tar.gz, .tgz,
-                .zip, .json).
-            params: Arguments to the pipeline function provided as a dict.
-            pipeline_id: ID of the pipeline.
-            version_id: ID of the pipeline version to run.
-                If both pipeline_id and version_id are specified, version_id
-                will take precendence.
-                If only pipeline_id is specified, the default version of this
-                pipeline is used to create the run.
-            pipeline_root: Root path of the pipeline outputs.
-            enable_caching: Whether or not to enable caching for the
-                run. If not set, defaults to the compile-time settings, which
-                is ``True`` for all tasks by default. If set, the
-                setting applies to all tasks in the pipeline (overrides the
-                compile time settings).
-            service_account: Specifies which Kubernetes service
-                account to use for this run.
+          experiment_id: The id of an experiment.
+          job_name: Name of the job.
+          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
+          params: A dictionary with key (string) as param name and value (string) as as param value.
+          pipeline_id: The id of a pipeline.
+          version_id: The id of a pipeline version.
+            If both pipeline_id and version_id are specified, version_id will take precendence.
+            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
+          pipeline_root: The root path of the pipeline outputs. This argument should
+            be used only for pipeline compiled with
+            dsl.PipelineExecutionMode.V2_COMPATIBLE or
+            dsl.PipelineExecutionMode.V2_ENGINGE mode.
+          enable_caching: Optional. Whether or not to enable caching for the run.
+            This setting affects v2 compatible mode and v2 mode only.
+            If not set, defaults to the compile time settings, which are True for all
+            tasks by default, while users may specify different caching options for
+            individual tasks.
+            If set, the setting applies to all tasks in the pipeline -- overrides
+            the compile time settings.
+          service_account: Optional. Specifies which Kubernetes service account this
+            run uses.
 
         Returns:
-            ``ApiRun`` object.
+          A run object. Most important field is id.
         """
         if params is None:
             params = {}
 
+        if pipeline_root is not None:
+            params[dsl.ROOT_PARAMETER_NAME] = pipeline_root
+
         job_config = self._create_job_config(
             experiment_id=experiment_id,
             params=params,
             pipeline_package_path=pipeline_package_path,
             pipeline_id=pipeline_id,
             version_id=version_id,
             enable_caching=enable_caching,
-            pipeline_root=pipeline_root,
         )
-        run_body = kfp_server_api.ApiRun(
+        run_body = kfp_server_api.models.ApiRun(
             pipeline_spec=job_config.spec,
             resource_references=job_config.resource_references,
             name=job_name,
             service_account=service_account)
 
         response = self._run_api.create_run(body=run_body)
 
-        link = f'{self._get_url_prefix()}/#/runs/details/{response.run.id}'
         if self._is_ipython():
             import IPython
-            html = (f'<a href="{link}" target="_blank" >Run details</a>.')
+            html = (
+                '<a href="%s/#/runs/details/%s" target="_blank" >Run details</a>.'
+                % (self._get_url_prefix(), response.run.id))
             IPython.display.display(IPython.display.HTML(html))
-        else:
-            print(f'Run details: {link}')
-
         return response.run
 
-    def archive_run(self, run_id: str) -> dict:
-        """Archives a run.
-
-        Args:
-            run_id: ID of the run.
-
-        Returns:
-            Empty dictionary.
-        """
-        return self._run_api.archive_run(id=run_id)
-
-    def unarchive_run(self, run_id: str) -> dict:
-        """Restores an archived run.
-
-        Args:
-            run_id: ID of the run.
-
-        Returns:
-            Empty dictionary.
-        """
-        return self._run_api.unarchive_run(id=run_id)
-
-    def delete_run(self, run_id: str) -> dict:
-        """Deletes a run.
-
-        Args:
-            run_id: ID of the run.
-
-        Returns:
-            Empty dictionary.
-        """
-        return self._run_api.delete_run(id=run_id)
-
-    def terminate_run(self, run_id: str) -> dict:
-        """Terminates a run.
-
-        Args:
-            run_id: ID of the run.
-
-        Returns:
-            Empty dictionary.
-        """
-        return self._run_api.terminate_run(run_id=run_id)
-
     def create_recurring_run(
         self,
         experiment_id: str,
         job_name: str,
         description: Optional[str] = None,
         start_time: Optional[str] = None,
         end_time: Optional[str] = None,
@@ -853,224 +799,236 @@
         max_concurrency: Optional[int] = 1,
         no_catchup: Optional[bool] = None,
         params: Optional[dict] = None,
         pipeline_package_path: Optional[str] = None,
         pipeline_id: Optional[str] = None,
         version_id: Optional[str] = None,
         enabled: bool = True,
-        pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
     ) -> kfp_server_api.ApiJob:
-        """Creates a recurring run.
+        """Create a recurring run.
 
         Args:
-            experiment_id: ID of the experiment.
-            job_name: Name of the job.
-            description: Description of the job.
-            start_time: RFC3339 time string of the time when to start the
-                job.
-            end_time: RFC3339 time string of the time when to end the job.
-            interval_second: Integer indicating the seconds between two
-                recurring runs in for a periodic schedule.
-            cron_expression: Cron expression representing a set of times,
-                using 6 space-separated fields (e.g., ``'0 0 9 ? * 2-6'``). See `cron format
-                <https://pkg.go.dev/github.com/robfig/cron#hdr-CRON_Expression_Format>`_.
-            max_concurrency: Integer indicating how many jobs can be run in
-                parallel.
-            no_catchup: Whether the recurring run should catch up if behind
-                schedule. For example, if the recurring run is paused for a
-                while and re-enabled afterwards. If ``no_catchup=False``, the
-                scheduler will catch up on (backfill) each missed interval.
-                Otherwise, it only schedules the latest interval if more than
-                one interval is ready to be scheduled. Usually, if your pipeline
-                handles backfill internally, you should turn catchup off to
-                avoid duplicate backfill.
-            pipeline_package_path: Local path of the pipeline package (the
-                filename should end with one of the following .tar.gz, .tgz,
-                .zip, .json).
-            params: Arguments to the pipeline function provided as a dict.
-            pipeline_id: ID of a pipeline.
-            version_id: ID of a pipeline version.
-                If both ``pipeline_id`` and ``version_id`` are specified, ``version_id``
-                will take precedence.
-                If only ``pipeline_id`` is specified, the default version of this
-                pipeline is used to create the run.
-            enabled: Whether to enable or disable the recurring run.
-            pipeline_root: Root path of the pipeline outputs.
-            enable_caching: Whether or not to enable caching for the
-                run. If not set, defaults to the compile time settings, which
-                is ``True`` for all tasks by default, while users may specify
-                different caching options for individual tasks. If set, the
-                setting applies to all tasks in the pipeline (overrides the
-                compile time settings).
-            service_account: Specifies which Kubernetes service
-                account this recurring run uses.
+          experiment_id: The string id of an experiment.
+          job_name: Name of the job.
+          description: An optional job description.
+          start_time: The RFC3339 time string of the time when to start the job.
+          end_time: The RFC3339 time string of the time when to end the job.
+          interval_second: Integer indicating the seconds between two recurring runs in for a periodic schedule.
+          cron_expression: A cron expression representing a set of times, using 6 space-separated fields, e.g. "0 0 9 ? * 2-6".
+            See `here <https://pkg.go.dev/github.com/robfig/cron#hdr-CRON_Expression_Format>`_ for details of the cron expression format.
+          max_concurrency: Integer indicating how many jobs can be run in parallel.
+          no_catchup: Whether the recurring run should catch up if behind schedule.
+            For example, if the recurring run is paused for a while and re-enabled
+            afterwards. If no_catchup=False, the scheduler will catch up on (backfill) each
+            missed interval. Otherwise, it only schedules the latest interval if more than one interval
+            is ready to be scheduled.
+            Usually, if your pipeline handles backfill internally, you should turn catchup
+            off to avoid duplicate backfill. (default: {False})
+          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
+          params: A dictionary with key (string) as param name and value (string) as param value.
+          pipeline_id: The id of a pipeline.
+          version_id: The id of a pipeline version.
+            If both pipeline_id and version_id are specified, version_id will take precendence.
+            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
+          enabled: A bool indicating whether the recurring run is enabled or disabled.
+          enable_caching: Optional. Whether or not to enable caching for the run.
+            This setting affects v2 compatible mode and v2 mode only.
+            If not set, defaults to the compile time settings, which are True for all
+            tasks by default, while users may specify different caching options for
+            individual tasks.
+            If set, the setting applies to all tasks in the pipeline -- overrides
+            the compile time settings.
+          service_account: Optional. Specifies which Kubernetes service account this
+            recurring run uses.
+
         Returns:
-            ``ApiJob`` object.
+          A Job object. Most important field is id.
+
+        Raises:
+          ValueError: If required parameters are not supplied.
         """
 
         job_config = self._create_job_config(
             experiment_id=experiment_id,
             params=params,
             pipeline_package_path=pipeline_package_path,
             pipeline_id=pipeline_id,
             version_id=version_id,
             enable_caching=enable_caching,
-            pipeline_root=pipeline_root,
         )
 
         if all([interval_second, cron_expression
                ]) or not any([interval_second, cron_expression]):
             raise ValueError(
                 'Either interval_second or cron_expression is required')
         if interval_second is not None:
-            trigger = kfp_server_api.ApiTrigger(
-                periodic_schedule=kfp_server_api.ApiPeriodicSchedule(
+            trigger = kfp_server_api.models.ApiTrigger(
+                periodic_schedule=kfp_server_api.models.ApiPeriodicSchedule(
                     start_time=start_time,
                     end_time=end_time,
                     interval_second=interval_second))
         if cron_expression is not None:
-            trigger = kfp_server_api.ApiTrigger(
-                cron_schedule=kfp_server_api.ApiCronSchedule(
+            trigger = kfp_server_api.models.ApiTrigger(
+                cron_schedule=kfp_server_api.models.ApiCronSchedule(
                     start_time=start_time,
                     end_time=end_time,
                     cron=cron_expression))
 
-        job_body = kfp_server_api.ApiJob(
+        job_body = kfp_server_api.models.ApiJob(
             enabled=enabled,
             pipeline_spec=job_config.spec,
             resource_references=job_config.resource_references,
             name=job_name,
             description=description,
             no_catchup=no_catchup,
             trigger=trigger,
             max_concurrency=max_concurrency,
             service_account=service_account)
         return self._job_api.create_job(body=job_body)
 
     def _create_job_config(
         self,
         experiment_id: str,
-        params: Optional[Dict[str, Any]],
+        params: Optional[dict],
         pipeline_package_path: Optional[str],
         pipeline_id: Optional[str],
         version_id: Optional[str],
         enable_caching: Optional[bool],
-        pipeline_root: Optional[str],
-    ) -> JobConfig:
-        """Creates a JobConfig with spec and resource_references.
-
-        Args:
-            experiment_id: ID of an experiment.
-            pipeline_package_path: Local path of the pipeline package (the
-                filename should end with one of the following .tar.gz, .tgz,
-                .zip, .yaml, .yml).
-            params: A dictionary with key as param name and value as param value.
-            pipeline_id: ID of a pipeline.
-            version_id: ID of a pipeline version.
-                If both pipeline_id and version_id are specified, version_id
-                will take precedence. If only pipeline_id is specified, the
-                default version of this pipeline is used to create the run.
-            enable_caching: Whether or not to enable caching for the
-                run. If not set, defaults to the compile time settings, which
-                is ``True`` for all tasks by default, while users may specify
-                different caching options for individual tasks. If set, the
-                setting applies to all tasks in the pipeline (overrides the
-                compile time settings).
-            pipeline_root: Root path of the pipeline outputs.
+    ):
+        """Create a JobConfig with spec and resource_references.
 
-        Returns:
-            A JobConfig object with attributes .spec and .resource_reference.
-        """
+        Args:
+          experiment_id: The id of an experiment.
+          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
+          params: A dictionary with key (string) as param name and value (string) as param value.
+          pipeline_id: The id of a pipeline.
+          version_id: The id of a pipeline version.
+            If both pipeline_id and version_id are specified, version_id will take precendence.
+            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
+          enable_caching: Whether or not to enable caching for the run.
+            This setting affects v2 compatible mode and v2 mode only.
+            If not set, defaults to the compile time settings, which are True for all
+            tasks by default, while users may specify different caching options for
+            individual tasks.
+            If set, the setting applies to all tasks in the pipeline -- overrides
+            the compile time settings.
+
+        Returns:
+          A JobConfig object with attributes spec and resource_reference.
+        """
+
+        class JobConfig:
+
+            def __init__(self, spec, resource_references):
+                self.spec = spec
+                self.resource_references = resource_references
 
         params = params or {}
-        pipeline_yaml_string = None
+        pipeline_json_string = None
         if pipeline_package_path:
             pipeline_obj = self._extract_pipeline_yaml(pipeline_package_path)
 
-            # Caching option set at submission time overrides the compile time
-            # settings.
+            # Caching option set at submission time overrides the compile time settings.
             if enable_caching is not None:
                 self._override_caching_options(pipeline_obj, enable_caching)
 
-            pipeline_yaml_string = yaml.dump(pipeline_obj, sort_keys=True)
-
-        runtime_config = kfp_server_api.PipelineSpecRuntimeConfig(
-            pipeline_root=pipeline_root,
-            parameters=params,
-        )
+            pipeline_json_string = json.dumps(pipeline_obj)
+        api_params = [
+            kfp_server_api.ApiParameter(
+                name=sanitize_k8s_name(name=k, allow_capital_underscore=True),
+                value=str(v) if type(v) not in (list, dict) else json.dumps(v))
+            for k, v in params.items()
+        ]
         resource_references = []
-        key = kfp_server_api.ApiResourceKey(
-            id=experiment_id, type=kfp_server_api.ApiResourceType.EXPERIMENT)
-        reference = kfp_server_api.ApiResourceReference(
-            key=key, relationship=kfp_server_api.ApiRelationship.OWNER)
+        key = kfp_server_api.models.ApiResourceKey(
+            id=experiment_id,
+            type=kfp_server_api.models.ApiResourceType.EXPERIMENT)
+        reference = kfp_server_api.models.ApiResourceReference(
+            key=key, relationship=kfp_server_api.models.ApiRelationship.OWNER)
         resource_references.append(reference)
 
         if version_id:
-            key = kfp_server_api.ApiResourceKey(
+            key = kfp_server_api.models.ApiResourceKey(
                 id=version_id,
-                type=kfp_server_api.ApiResourceType.PIPELINE_VERSION)
-            reference = kfp_server_api.ApiResourceReference(
-                key=key, relationship=kfp_server_api.ApiRelationship.CREATOR)
+                type=kfp_server_api.models.ApiResourceType.PIPELINE_VERSION)
+            reference = kfp_server_api.models.ApiResourceReference(
+                key=key,
+                relationship=kfp_server_api.models.ApiRelationship.CREATOR)
             resource_references.append(reference)
 
-        spec = kfp_server_api.ApiPipelineSpec(
+        spec = kfp_server_api.models.ApiPipelineSpec(
             pipeline_id=pipeline_id,
-            pipeline_manifest=pipeline_yaml_string,
-            runtime_config=runtime_config,
-        )
+            workflow_manifest=pipeline_json_string,
+            parameters=api_params)
         return JobConfig(spec=spec, resource_references=resource_references)
 
     def create_run_from_pipeline_func(
         self,
-        pipeline_func: Union[Callable[..., Any], base_component.BaseComponent],
-        arguments: Optional[Dict[str, Any]] = None,
+        pipeline_func: Callable,
+        arguments: Mapping[str, str],
         run_name: Optional[str] = None,
         experiment_name: Optional[str] = None,
+        pipeline_conf: Optional[dsl.PipelineConf] = None,
         namespace: Optional[str] = None,
+        mode: dsl.PipelineExecutionMode = dsl.PipelineExecutionMode.V1_LEGACY,
+        launcher_image: Optional[str] = None,
         pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ) -> RunPipelineResult:
+    ):
         """Runs pipeline on KFP-enabled Kubernetes cluster.
 
-        This command compiles the pipeline function, creates or gets an
-        experiment, then submits the pipeline for execution.
+        This command compiles the pipeline function, creates or gets an experiment and submits the pipeline for execution.
 
         Args:
-            pipeline_func: Pipeline function constructed with ``@kfp.dsl.pipeline`` decorator.
-            arguments: Arguments to the pipeline function provided as a dict.
-            run_name: Name of the run to be shown in the UI.
-            experiment_name: Name of the experiment to add the run to.
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
-            pipeline_root: Root path of the pipeline outputs.
-            enable_caching: Whether or not to enable caching for the
-                run. If not set, defaults to the compile time settings, which
-                is ``True`` for all tasks by default, while users may specify
-                different caching options for individual tasks. If set, the
-                setting applies to all tasks in the pipeline (overrides the
-                compile time settings).
-            service_account: Specifies which Kubernetes service
-                account to use for this run.
+          pipeline_func: A function that describes a pipeline by calling components and composing them into execution graph.
+          arguments: Arguments to the pipeline function provided as a dict.
+          run_name: Optional. Name of the run to be shown in the UI.
+          experiment_name: Optional. Name of the experiment to add the run to.
+          pipeline_conf: Optional. Pipeline configuration ops that will be applied
+            to all the ops in the pipeline func.
+          namespace: Kubernetes namespace where the pipeline runs are created.
+            For single user deployment, leave it as None;
+            For multi user, input a namespace where the user is authorized
+          mode: The PipelineExecutionMode to use when compiling and running
+            pipeline_func.
+          launcher_image: The launcher image to use if the mode is specified as
+            PipelineExecutionMode.V2_COMPATIBLE. Should only be needed for tests
+            or custom deployments right now.
+          pipeline_root: The root path of the pipeline outputs. This argument should
+            be used only for pipeline compiled with
+            dsl.PipelineExecutionMode.V2_COMPATIBLE or
+            dsl.PipelineExecutionMode.V2_ENGINGE mode.
+          enable_caching: Optional. Whether or not to enable caching for the run.
+            This setting affects v2 compatible mode and v2 mode only.
+            If not set, defaults to the compile time settings, which are True for all
+            tasks by default, while users may specify different caching options for
+            individual tasks.
+            If set, the setting applies to all tasks in the pipeline -- overrides
+            the compile time settings.
+          service_account: Optional. Specifies which Kubernetes service account this
+            run uses.
+        """
+        if pipeline_root is not None and mode == dsl.PipelineExecutionMode.V1_LEGACY:
+            raise ValueError('`pipeline_root` should not be used with '
+                             'dsl.PipelineExecutionMode.V1_LEGACY mode.')
 
-        Returns:
-            ``RunPipelineResult`` object containing information about the pipeline run.
-        """
         #TODO: Check arguments against the pipeline function
-        pipeline_name = pipeline_func.name
+        pipeline_name = pipeline_func.__name__
         run_name = run_name or pipeline_name + ' ' + datetime.datetime.now(
         ).strftime('%Y-%m-%d %H-%M-%S')
-
         with tempfile.TemporaryDirectory() as tmpdir:
             pipeline_package_path = os.path.join(tmpdir, 'pipeline.yaml')
-            compiler.Compiler().compile(
-                pipeline_func=pipeline_func,
-                package_path=pipeline_package_path,
-            )
+            compiler.Compiler(
+                mode=mode, launcher_image=launcher_image).compile(
+                    pipeline_func=pipeline_func,
+                    package_path=pipeline_package_path,
+                    pipeline_conf=pipeline_conf)
 
             return self.create_run_from_pipeline_package(
                 pipeline_file=pipeline_package_path,
                 arguments=arguments,
                 run_name=run_name,
                 experiment_name=experiment_name,
                 namespace=namespace,
@@ -1078,57 +1036,75 @@
                 enable_caching=enable_caching,
                 service_account=service_account,
             )
 
     def create_run_from_pipeline_package(
         self,
         pipeline_file: str,
-        arguments: Optional[Dict[str, str]] = None,
+        arguments: Mapping[str, str],
         run_name: Optional[str] = None,
         experiment_name: Optional[str] = None,
         namespace: Optional[str] = None,
         pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ) -> RunPipelineResult:
+    ):
         """Runs pipeline on KFP-enabled Kubernetes cluster.
 
-        This command takes a local pipeline package, creates or gets an
-        experiment, then submits the pipeline for execution.
+        This command takes a local pipeline package, creates or gets an experiment
+        and submits the pipeline for execution.
 
         Args:
-            pipeline_file: A compiled pipeline package file.
-            arguments: Arguments to the pipeline function provided as a dict.
-            run_name:  Name of the run to be shown in the UI.
-            experiment_name: Name of the experiment to add the run to.
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
-            pipeline_root: Root path of the pipeline outputs.
-            enable_caching: Whether or not to enable caching for the
-                run. If not set, defaults to the compile time settings, which
-                is ``True`` for all tasks by default, while users may specify
-                different caching options for individual tasks. If set, the
-                setting applies to all tasks in the pipeline (overrides the
-                compile time settings).
-            service_account: Specifies which Kubernetes service
-                account to use for this run.
+          pipeline_file: A compiled pipeline package file.
+          arguments: Arguments to the pipeline function provided as a dict.
+          run_name: Optional. Name of the run to be shown in the UI.
+          experiment_name: Optional. Name of the experiment to add the run to.
+          namespace: Kubernetes namespace where the pipeline runs are created.
+            For single user deployment, leave it as None;
+            For multi user, input a namespace where the user is authorized
+          pipeline_root: The root path of the pipeline outputs. This argument should
+            be used only for pipeline compiled with
+            dsl.PipelineExecutionMode.V2_COMPATIBLE or
+            dsl.PipelineExecutionMode.V2_ENGINGE mode.
+          enable_caching: Optional. Whether or not to enable caching for the run.
+            This setting affects v2 compatible mode and v2 mode only.
+            If not set, defaults to the compile time settings, which are True for all
+            tasks by default, while users may specify different caching options for
+            individual tasks.
+            If set, the setting applies to all tasks in the pipeline -- overrides
+            the compile time settings.
+          service_account: Optional. Specifies which Kubernetes service account this
+            run uses.
+        """
+
+        class RunPipelineResult:
+
+            def __init__(self, client, run_info):
+                self._client = client
+                self.run_info = run_info
+                self.run_id = run_info.id
+
+            def wait_for_run_completion(self, timeout=None):
+                timeout = timeout or datetime.timedelta.max
+                return self._client.wait_for_run_completion(
+                    self.run_id, timeout)
 
-        Returns:
-            ``RunPipelineResult`` object containing information about the pipeline run.
-        """
+            def __repr__(self):
+                return 'RunPipelineResult(run_id={})'.format(self.run_id)
 
         #TODO: Check arguments against the pipeline function
         pipeline_name = os.path.basename(pipeline_file)
         experiment_name = experiment_name or os.environ.get(
             KF_PIPELINES_DEFAULT_EXPERIMENT_NAME, None)
         overridden_experiment_name = os.environ.get(
             KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME, experiment_name)
         if overridden_experiment_name != experiment_name:
-            warnings.warn(
-                f'Changing experiment name from "{experiment_name}" to "{overridden_experiment_name}".'
-            )
+            import warnings
+            warnings.warn('Changing experiment name from "{}" to "{}".'.format(
+                experiment_name, overridden_experiment_name))
         experiment_name = overridden_experiment_name or 'Default'
         run_name = run_name or (
             pipeline_name + ' ' +
             datetime.datetime.now().strftime('%Y-%m-%d %H-%M-%S'))
         experiment = self.create_experiment(
             name=experiment_name, namespace=namespace)
         run_info = self.run_pipeline(
@@ -1138,286 +1114,301 @@
             params=arguments,
             pipeline_root=pipeline_root,
             enable_caching=enable_caching,
             service_account=service_account,
         )
         return RunPipelineResult(self, run_info)
 
-    def delete_job(self, job_id: str) -> dict:
-        """Deletes a job (recurring run).
+    def delete_job(self, job_id: str):
+        """Deletes a job.
 
         Args:
-            job_id: ID of the job.
+          job_id: id of the job.
 
         Returns:
-            Empty dictionary.
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          kfp_server_api.ApiException: If the job is not found.
         """
         return self._job_api.delete_job(id=job_id)
 
-    def disable_job(self, job_id: str) -> dict:
-        """Disables a job (recurring run).
+    def disable_job(self, job_id: str):
+        """Disables a job.
 
         Args:
-            job_id: ID of the job.
+          job_id: id of the job.
 
         Returns:
-            Empty dictionary.
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          ApiException: If the job is not found.
         """
         return self._job_api.disable_job(id=job_id)
 
-    def enable_job(self, job_id: str) -> dict:
-        """Enables a job (recurring run).
+    def enable_job(self, job_id: str):
+        """Enables a job.
 
         Args:
-            job_id: ID of the job.
+          job_id: id of the job.
 
         Returns:
-            Empty dictionary.
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          ApiException: If the job is not found.
         """
         return self._job_api.enable_job(id=job_id)
 
     def list_runs(
             self,
             page_token: str = '',
             page_size: int = 10,
             sort_by: str = '',
             experiment_id: Optional[str] = None,
             namespace: Optional[str] = None,
             filter: Optional[str] = None) -> kfp_server_api.ApiListRunsResponse:
-        """List runs.
+        """List runs, optionally can be filtered by experiment or namespace.
 
         Args:
-            page_token: Page token for obtaining page from paginated response.
-            page_size: Size of the page.
-            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'name desc'``.
-            experiment_id: Experiment ID to filter upon
-            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
-            filter: A url-encoded, JSON-serialized Filter protocol buffer
-                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/backend/api/filter.proto>`_). For a list of all filter operations ``'op'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
-
-                  ::
-
-                    json.dumps({
-                        "predicates": [{
-                            "op": _FILTER_OPERATIONS["EQUALS"],
-                            "key": "name",
-                            "stringValue": "my-name",
-                        }]
-                    })
+          page_token: Token for starting of the page.
+          page_size: Size of the page.
+          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
+          experiment_id: Experiment id to filter upon
+          namespace: Kubernetes namespace to filter upon.
+            For single user deployment, leave it as None;
+            For multi user, input a namespace where the user is authorized.
+          filter: A url-encoded, JSON-serialized Filter protocol buffer
+            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+
+            An example filter string would be:
+
+                # For the list of filter operations please see:
+                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
+                json.dumps({
+                    "predicates": [{
+                        "op": _FILTER_OPERATIONS["EQUALS"],
+                        "key": "name",
+                        "stringValue": "my-name",
+                    }]
+                })
 
-          Returns:
-            ``ApiListRunsResponse`` object.
+        Returns:
+          A response object including a list of experiments and next page token.
         """
         namespace = namespace or self.get_user_namespace()
         if experiment_id is not None:
-            return self._run_api.list_runs(
+            response = self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.ApiResourceType
-                .EXPERIMENT,
+                resource_reference_key_type=kfp_server_api.models
+                .api_resource_type.ApiResourceType.EXPERIMENT,
                 resource_reference_key_id=experiment_id,
                 filter=filter)
-
-        elif namespace is not None:
-            return self._run_api.list_runs(
+        elif namespace:
+            response = self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.ApiResourceType
-                .NAMESPACE,
+                resource_reference_key_type=kfp_server_api.models
+                .api_resource_type.ApiResourceType.NAMESPACE,
                 resource_reference_key_id=namespace,
                 filter=filter)
-
         else:
-            return self._run_api.list_runs(
+            response = self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
                 filter=filter)
+        return response
 
     def list_recurring_runs(
             self,
             page_token: str = '',
             page_size: int = 10,
             sort_by: str = '',
             experiment_id: Optional[str] = None,
             filter: Optional[str] = None) -> kfp_server_api.ApiListJobsResponse:
-        """Lists recurring runs.
+        """List recurring runs.
 
         Args:
-            page_token: Page token for obtaining page from paginated response.
-            page_size: Size of the page.
-            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'name desc'``.
-            experiment_id: Experiment ID to filter upon.
-            filter: A url-encoded, JSON-serialized Filter protocol buffer
-                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/backend/api/filter.proto>`_). For a list of all filter operations ``'op'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
-
-                  ::
-
-                    json.dumps({
-                        "predicates": [{
-                            "op": _FILTER_OPERATIONS["EQUALS"],
-                            "key": "name",
-                            "stringValue": "my-name",
-                        }]
-                    })
+          page_token: Token for starting of the page.
+          page_size: Size of the page.
+          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
+          experiment_id: Experiment id to filter upon.
+          filter: A url-encoded, JSON-serialized Filter protocol buffer
+            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+
+            An example filter string would be:
+
+                # For the list of filter operations please see:
+                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
+                json.dumps({
+                    "predicates": [{
+                        "op": _FILTER_OPERATIONS["EQUALS"],
+                        "key": "name",
+                        "stringValue": "my-name",
+                    }]
+                })
 
         Returns:
-            ``ApiListJobsResponse`` object.
+          A response object including a list of recurring_runs and next page token.
         """
         if experiment_id is not None:
-            return self._job_api.list_jobs(
+            response = self._job_api.list_jobs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.ApiResourceType
-                .EXPERIMENT,
+                resource_reference_key_type=kfp_server_api.models
+                .api_resource_type.ApiResourceType.EXPERIMENT,
                 resource_reference_key_id=experiment_id,
                 filter=filter)
-
         else:
-            return self._job_api.list_jobs(
+            response = self._job_api.list_jobs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
                 filter=filter)
+        return response
 
     def get_recurring_run(self, job_id: str) -> kfp_server_api.ApiJob:
-        """Gets recurring run (job) details.
+        """Get recurring_run details.
 
         Args:
-            job_id: ID of the recurring run (job).
+          job_id: id of the recurring_run.
 
         Returns:
-            ``ApiJob`` object.
+          A response object including details of a recurring_run.
+
+        Raises:
+          kfp_server_api.ApiException: If recurring_run is not found.
         """
         return self._job_api.get_job(id=job_id)
 
     def get_run(self, run_id: str) -> kfp_server_api.ApiRun:
-        """Gets run details.
+        """Get run details.
 
         Args:
-            run_id: ID of the run.
+          run_id: id of the run.
 
         Returns:
-            ``ApiRun`` object.
+          A response object including details of a run.
+
+        Raises:
+          kfp_server_api.ApiException: If run is not found.
         """
         return self._run_api.get_run(run_id=run_id)
 
-    def wait_for_run_completion(
-            self,
-            run_id: str,
-            timeout: int,
-            sleep_duration: int = 5) -> kfp_server_api.ApiRun:
+    def wait_for_run_completion(self, run_id: str, timeout: int):
         """Waits for a run to complete.
 
         Args:
-            run_id: ID of the run.
-            timeout: Timeout after which the client should stop waiting for run completion (seconds).
-            sleep_duration: Time in seconds between retries.
+          run_id: Run id, returned from run_pipeline.
+          timeout: Timeout in seconds.
 
         Returns:
-            ``ApiRun`` object.
+          A run detail object: Most important fields are run and pipeline_runtime.
+
+        Raises:
+          TimeoutError: if the pipeline run failed to finish before the specified timeout.
         """
         status = 'Running:'
         start_time = datetime.datetime.now()
         if isinstance(timeout, datetime.timedelta):
             timeout = timeout.total_seconds()
         is_valid_token = False
         while (status is None or status.lower()
                not in ['succeeded', 'failed', 'skipped', 'error']):
             try:
                 get_run_response = self._run_api.get_run(run_id=run_id)
                 is_valid_token = True
-            except kfp_server_api.ApiException as api_ex:
+            except ApiException as api_ex:
                 # if the token is valid but receiving 401 Unauthorized error
                 # then refresh the token
                 if is_valid_token and api_ex.status == 401:
                     logging.info('Access token has expired !!! Refreshing ...')
                     self._refresh_api_client_token()
                     continue
                 else:
                     raise api_ex
             status = get_run_response.run.status
             elapsed_time = (datetime.datetime.now() -
                             start_time).total_seconds()
             logging.info('Waiting for the job to complete...')
             if elapsed_time > timeout:
                 raise TimeoutError('Run timeout')
-            time.sleep(sleep_duration)
+            time.sleep(5)
         return get_run_response
 
-    def _get_workflow_json(self, run_id: str) -> dict:
-        """Gets the workflow json.
+    def _get_workflow_json(self, run_id):
+        """Get the workflow json.
 
         Args:
-            run_id: run id, returned from run_pipeline.
+          run_id: run id, returned from run_pipeline.
 
         Returns:
-            Workflow JSON.
+          workflow: Json workflow
         """
         get_run_response = self._run_api.get_run(run_id=run_id)
         workflow = get_run_response.pipeline_runtime.workflow_manifest
-        return json.loads(workflow)
+        workflow_json = json.loads(workflow)
+        return workflow_json
 
     def upload_pipeline(
         self,
         pipeline_package_path: str = None,
         pipeline_name: str = None,
         description: str = None,
     ) -> kfp_server_api.ApiPipeline:
-        """Uploads a pipeline.
+        """Uploads the pipeline to the Kubeflow Pipelines cluster.
 
         Args:
-            pipeline_package_path: Local path to the pipeline package.
-            pipeline_name: Name of the pipeline to be shown in the UI.
-            description: Description of the pipeline to be shown in
-                the UI.
+          pipeline_package_path: Local path to the pipeline package.
+          pipeline_name: Optional. Name of the pipeline to be shown in the UI.
+          description: Optional. Description of the pipeline to be shown in the UI.
 
         Returns:
-            ``ApiPipeline`` object.
+          Server response object containing pipleine id and other information.
         """
-        if pipeline_name is None:
-            pipeline_name = os.path.splitext(
-                os.path.basename('something/file.txt'))[0]
 
-        validate_pipeline_resource_name(pipeline_name)
         response = self._upload_api.upload_pipeline(
             pipeline_package_path, name=pipeline_name, description=description)
-        link = f'{self._get_url_prefix()}/#/pipelines/details/{response.id}'
         if self._is_ipython():
             import IPython
-            html = f'<a href="{link}" target="_blank" >Pipeline details</a>.'
+            html = '<a href=%s/#/pipelines/details/%s>Pipeline details</a>.' % (
+                self._get_url_prefix(), response.id)
             IPython.display.display(IPython.display.HTML(html))
-        else:
-            print(f'Pipeline details: {link}')
-
         return response
 
     def upload_pipeline_version(
         self,
-        pipeline_package_path: str,
+        pipeline_package_path,
         pipeline_version_name: str,
         pipeline_id: Optional[str] = None,
         pipeline_name: Optional[str] = None,
         description: Optional[str] = None,
     ) -> kfp_server_api.ApiPipelineVersion:
-        """Uploads a new version of the pipeline.
+        """Uploads a new version of the pipeline to the Kubeflow Pipelines
+        cluster.
 
         Args:
-            pipeline_package_path: Local path to the pipeline package.
-            pipeline_version_name:  Name of the pipeline version to be shown in
-                the UI.
-            pipeline_id: ID of the pipeline.
-            pipeline_name: Name of the pipeline.
-            description: Description of the pipeline version to show in the UI.
+          pipeline_package_path: Local path to the pipeline package.
+          pipeline_version_name:  Name of the pipeline version to be shown in the UI.
+          pipeline_id: Optional. Id of the pipeline.
+          pipeline_name: Optional. Name of the pipeline.
+          description: Optional. Description of the pipeline version to be shown in the UI.
 
         Returns:
-            ``ApiPipelineVersion`` object.
+          Server response object containing pipleine id and other information.
+
+        Raises:
+          ValueError when none or both of pipeline_id or pipeline_name are specified
+          kfp_server_api.ApiException: If pipeline id is not found.
         """
 
         if all([pipeline_id, pipeline_name
                ]) or not any([pipeline_id, pipeline_name]):
             raise ValueError('Either pipeline_id or pipeline_name is required')
 
         if pipeline_name:
@@ -1425,152 +1416,114 @@
         kwargs = dict(
             name=pipeline_version_name,
             pipelineid=pipeline_id,
         )
 
         if description:
             kwargs['description'] = description
+        try:
+            response = self._upload_api.upload_pipeline_version(
+                pipeline_package_path, **kwargs)
+        except kfp_server_api.exceptions.ApiTypeError as e:
+            # ToDo: Remove this once we drop support for kfp_server_api < 1.7.1
+            if 'description' in e.message and 'unexpected keyword argument' in e.message:
+                raise NotImplementedError(
+                    'Pipeline version description is not supported in current kfp-server-api pypi package. Upgrade to 1.7.1 or above'
+                )
+            else:
+                raise e
 
-        response = self._upload_api.upload_pipeline_version(
-            pipeline_package_path, **kwargs)
-
-        link = f'{self._get_url_prefix()}/#/pipelines/details/{response.id}'
         if self._is_ipython():
             import IPython
-            html = f'<a href="{link}" target="_blank" >Pipeline details</a>.'
+            html = '<a href=%s/#/pipelines/details/%s>Pipeline details</a>.' % (
+                self._get_url_prefix(), response.id)
             IPython.display.display(IPython.display.HTML(html))
-        else:
-            print(f'Pipeline details: {link}')
-
         return response
 
     def get_pipeline(self, pipeline_id: str) -> kfp_server_api.ApiPipeline:
-        """Gets pipeline details.
+        """Get pipeline details.
 
         Args:
-            pipeline_id: ID of the pipeline.
+          pipeline_id: id of the pipeline.
 
         Returns:
-            ``ApiPipeline`` object.
+          A response object including details of a pipeline.
+
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
         """
         return self._pipelines_api.get_pipeline(id=pipeline_id)
 
-    def delete_pipeline(self, pipeline_id: str) -> dict:
-        """Deletes a pipeline.
+    def delete_pipeline(self, pipeline_id):
+        """Delete pipeline.
 
         Args:
-            pipeline_id: ID of the pipeline.
+          pipeline_id: id of the pipeline.
 
         Returns:
-            Empty dictionary.
+          Object. If the method is called asynchronously, returns the request thread.
+
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
         """
         return self._pipelines_api.delete_pipeline(id=pipeline_id)
 
     def list_pipeline_versions(
         self,
         pipeline_id: str,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
         filter: Optional[str] = None
     ) -> kfp_server_api.ApiListPipelineVersionsResponse:
         """Lists pipeline versions.
 
         Args:
-            pipeline_id: ID of the pipeline for which to list versions.
-            page_token: Page token for obtaining page from paginated response.
-            page_size: Size of the page.
-            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'name desc'``.
-            filter: A url-encoded, JSON-serialized Filter protocol buffer
-                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/backend/api/filter.proto>`_). For a list of all filter operations ``'op'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
-
-                  ::
-
-                    json.dumps({
-                        "predicates": [{
-                            "op": _FILTER_OPERATIONS["EQUALS"],
-                            "key": "name",
-                            "stringValue": "my-name",
-                        }]
-                    })
+          pipeline_id: Id of the pipeline to list versions
+          page_token: Token for starting of the page.
+          page_size: Size of the page.
+          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
+          filter: A url-encoded, JSON-serialized Filter protocol buffer
+            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+
+            An example filter string would be:
+
+                # For the list of filter operations please see:
+                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
+                json.dumps({
+                    "predicates": [{
+                        "op": _FILTER_OPERATIONS["EQUALS"],
+                        "key": "name",
+                        "stringValue": "my-name",
+                    }]
+                })
 
         Returns:
-            ``ApiListPipelineVersionsResponse`` object.
+          A response object including a list of versions and next page token.
+
+        Raises:
+          kfp_server_api.ApiException: If pipeline is not found.
         """
 
         return self._pipelines_api.list_pipeline_versions(
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
-            resource_key_type=kfp_server_api.ApiResourceType.PIPELINE,
+            resource_key_type=kfp_server_api.models.api_resource_type
+            .ApiResourceType.PIPELINE,
             resource_key_id=pipeline_id,
             filter=filter)
 
-    def get_pipeline_version(
-            self, version_id: str) -> kfp_server_api.ApiPipelineVersion:
-        """Gets a pipeline version.
+    def delete_pipeline_version(self, version_id: str):
+        """Delete pipeline version.
 
         Args:
-            version_id: ID of the pipeline version.
+          version_id: id of the pipeline version.
 
         Returns:
-            ``ApiPipelineVersion`` object.
-        """
-        return self._pipelines_api.get_pipeline_version(version_id=version_id)
-
-    def delete_pipeline_version(self, version_id: str) -> dict:
-        """Deletes a pipeline version.
+          Object. If the method is called asynchronously, returns the request thread.
 
-        Args:
-            version_id: ID of the pipeline version.
-
-        Returns:
-            Empty dictionary.
+        Raises:
+          Exception if pipeline version is not found.
         """
         return self._pipelines_api.delete_pipeline_version(
             version_id=version_id)
-
-
-def _add_generated_apis(target_struct: Any, api_module: ModuleType,
-                        api_client: kfp_server_api.ApiClient):
-    """Initializes a hierarchical API object based on the generated API module.
-
-    PipelineServiceApi.create_pipeline becomes
-    target_struct.pipelines.create_pipeline
-    """
-    Struct = type('Struct', (), {})
-
-    def camel_case_to_snake_case(name: str) -> str:
-        return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
-
-    for api_name in dir(api_module):
-        if not api_name.endswith('ServiceApi'):
-            continue
-
-        short_api_name = camel_case_to_snake_case(
-            api_name[0:-len('ServiceApi')]) + 's'
-        api_struct = Struct()
-        setattr(target_struct, short_api_name, api_struct)
-        service_api = getattr(api_module.api, api_name)
-        initialized_service_api = service_api(api_client)
-        for member_name in dir(initialized_service_api):
-            if member_name.startswith('_') or member_name.endswith(
-                    '_with_http_info'):
-                continue
-
-            bound_member = getattr(initialized_service_api, member_name)
-            setattr(api_struct, member_name, bound_member)
-    models_struct = Struct()
-    for member_name in dir(api_module.models):
-        if not member_name[0].islower():
-            setattr(models_struct, member_name,
-                    getattr(api_module.models, member_name))
-    target_struct.api_models = models_struct
-
-
-def validate_pipeline_resource_name(name: str) -> None:
-    REGEX = r'[a-z0-9]([-a-z0-9]*[a-z0-9])?(\\.[a-z0-9]([-a-z0-9]*[a-z0-9])?)*'
-
-    if re.fullmatch(REGEX, name) is None:
-        raise ValueError(
-            f'Invalid pipeline name: "{name}". Pipeline name must conform to the regex: "{REGEX}".'
-        )
```

### Comparing `kfp-2.0.0b9/kfp/client/client_test.py` & `kfp-2.0.0rc1/kfp/client/client_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,24 +11,27 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import json
 import os
 import tempfile
+import textwrap
 import unittest
 from unittest.mock import MagicMock
 from unittest.mock import Mock
 from unittest.mock import patch
 
 from absl.testing import parameterized
+from google.protobuf import json_format
 from kfp.client import client
 from kfp.compiler import Compiler
 from kfp.dsl import component
 from kfp.dsl import pipeline
+from kfp.pipeline_spec import pipeline_spec_pb2
 import kfp_server_api
 import yaml
 
 
 class TestValidatePipelineName(parameterized.TestCase):
 
     @parameterized.parameters([
@@ -50,39 +53,14 @@
     def test_invalid(self, name: str):
         with self.assertRaisesRegex(ValueError, r'Invalid pipeline name:'):
             client.validate_pipeline_resource_name(name)
 
 
 class TestOverrideCachingOptions(parameterized.TestCase):
 
-    def test_override_caching_from_pipeline(self):
-
-        @component
-        def hello_world(text: str) -> str:
-            """Hello world component."""
-            return text
-
-        @pipeline(name='hello-world', description='A simple intro pipeline')
-        def pipeline_hello_world(text: str = 'hi there'):
-            """Hello world pipeline."""
-
-            hello_world(text=text).set_caching_options(True)
-
-        with tempfile.TemporaryDirectory() as tempdir:
-            temp_filepath = os.path.join(tempdir, 'hello_world_pipeline.yaml')
-            Compiler().compile(
-                pipeline_func=pipeline_hello_world, package_path=temp_filepath)
-
-            with open(temp_filepath, 'r') as f:
-                pipeline_obj = yaml.safe_load(f)
-                test_client = client.Client(namespace='foo')
-                test_client._override_caching_options(pipeline_obj, False)
-                for _, task in pipeline_obj['root']['dag']['tasks'].items():
-                    self.assertFalse(task['cachingOptions']['enableCache'])
-
     def test_override_caching_of_multiple_components(self):
 
         @component
         def hello_word(text: str) -> str:
             return text
 
         @component
@@ -92,37 +70,131 @@
         @pipeline(
             name='sample two-step pipeline',
             description='a minimal two-step pipeline')
         def pipeline_with_two_component(text: str = 'hi there'):
 
             component_1 = hello_word(text=text).set_caching_options(True)
             component_2 = to_lower(
-                text=component_1.output).set_caching_options(True)
+                text=component_1.output).set_caching_options(False)
 
         with tempfile.TemporaryDirectory() as tempdir:
             temp_filepath = os.path.join(tempdir, 'hello_world_pipeline.yaml')
             Compiler().compile(
                 pipeline_func=pipeline_with_two_component,
                 package_path=temp_filepath)
 
             with open(temp_filepath, 'r') as f:
                 pipeline_obj = yaml.safe_load(f)
-                test_client = client.Client(namespace='foo')
-                test_client._override_caching_options(pipeline_obj, False)
-                self.assertFalse(
-                    pipeline_obj['root']['dag']['tasks']['hello-word']
-                    ['cachingOptions']['enableCache'])
-                self.assertFalse(pipeline_obj['root']['dag']['tasks']
-                                 ['to-lower']['cachingOptions']['enableCache'])
+                pipeline_spec = json_format.ParseDict(
+                    pipeline_obj, pipeline_spec_pb2.PipelineSpec())
+                client._override_caching_options(pipeline_spec, True)
+                pipeline_obj = json_format.MessageToDict(pipeline_spec)
+                self.assertTrue(pipeline_obj['root']['dag']['tasks']
+                                ['hello-word']['cachingOptions']['enableCache'])
+                self.assertTrue(pipeline_obj['root']['dag']['tasks']['to-lower']
+                                ['cachingOptions']['enableCache'])
+
+
+class TestExtractPipelineYAML(parameterized.TestCase):
+
+    def test_extract_pipeline_yaml_single_doc(self):
+
+        with tempfile.TemporaryDirectory() as tempdir:
+            temp_filepath = os.path.join(tempdir, 'single_doc_pipeline.yaml')
+            with open(temp_filepath, 'w') as f:
+                f.write(
+                    textwrap.dedent('''
+                        components:
+                          comp-foo:
+                            executorLabel: exec-foo
+                        deploymentSpec:
+                          executors:
+                            exec-foo:
+                              container:
+                                command:
+                                - sh
+                                - -c
+                                - cat /data/file.txt
+                                image: alpine
+                        pipelineInfo:
+                          name: my-pipeline
+                        root:
+                          dag:
+                            tasks:
+                              foo:
+                                componentRef:
+                                  name: comp-foo
+                                taskInfo:
+                                  name: foo
+                        schemaVersion: 2.1.0
+                        sdkVersion: kfp-2.0.0-beta.13
+                        '''))
+
+            pipeline_dict = client._extract_pipeline_yaml(
+                temp_filepath).to_dict()
+            self.assertEqual('my-pipeline',
+                             pipeline_dict['pipelineInfo']['name'])
+
+    def test_extract_pipeline_yaml_multiple_docs(self):
+
+        with tempfile.TemporaryDirectory() as tempdir:
+            temp_filepath = os.path.join(tempdir, 'multi_docs_pipeline.yaml')
+            with open(temp_filepath, 'w') as f:
+                f.write(
+                    textwrap.dedent('''
+                        components:
+                          comp-foo:
+                            executorLabel: exec-foo
+                        deploymentSpec:
+                          executors:
+                            exec-foo:
+                              container:
+                                command:
+                                - sh
+                                - -c
+                                - cat /data/file.txt
+                                image: alpine
+                        pipelineInfo:
+                          name: my-pipeline
+                        root:
+                          dag:
+                            tasks:
+                              foo:
+                                componentRef:
+                                  name: comp-foo
+                                taskInfo:
+                                  name: foo
+                        schemaVersion: 2.1.0
+                        sdkVersion: kfp-2.0.0-beta.13
+                        ---
+                        platforms:
+                          kubernetes:
+                            deploymentSpec:
+                              executors:
+                                exec-foo:
+                                  pvcMount:
+                                  - mountPath: /data
+                                    constant: my-pvc
+                        '''))
+
+            pipeline_dict = client._extract_pipeline_yaml(
+                temp_filepath).to_dict()
+            self.assertEqual(
+                'my-pipeline',
+                pipeline_dict['pipeline_spec']['pipelineInfo']['name'])
+            self.assertEqual(
+                'my-pvc', pipeline_dict['platform_spec']['platforms']
+                ['kubernetes']['deploymentSpec']['executors']['exec-foo']
+                ['pvcMount'][0]['constant'])
 
 
 class TestClient(unittest.TestCase):
 
     def setUp(self):
-        self.client = client.Client(namespace='foo')
+        self.client = client.Client(namespace='ns1')
 
     def test__is_ipython_return_false(self):
         mock = MagicMock()
         with patch.dict('sys.modules', IPython=mock):
             mock.get_ipython.return_value = None
             self.assertFalse(self.client._is_ipython())
 
@@ -148,29 +220,29 @@
                     run_id='foo', timeout=1, sleep_duration=0)
                 mock_get_run.assert_called_once()
 
     def test_wait_for_run_completion_expired_access_token(self):
         with patch.object(self.client._run_api, 'get_run') as mock_get_run:
             # We need to iterate through multiple side effects in order to test this logic.
             mock_get_run.side_effect = [
-                Mock(run=Mock(status='foo')),
+                Mock(state='unknown state'),
                 kfp_server_api.ApiException(status=401),
-                Mock(run=Mock(status='succeeded')),
+                Mock(state='succeeded'),
             ]
 
             with patch.object(self.client, '_refresh_api_client_token'
                              ) as mock_refresh_api_client_token:
                 self.client.wait_for_run_completion(
                     run_id='foo', timeout=1, sleep_duration=0)
                 mock_get_run.assert_called_with(run_id='foo')
                 mock_refresh_api_client_token.assert_called_once()
 
     def test_wait_for_run_completion_valid_token(self):
         with patch.object(self.client._run_api, 'get_run') as mock_get_run:
-            mock_get_run.return_value = Mock(run=Mock(status='succeeded'))
+            mock_get_run.return_value = Mock(state='succeeded')
             response = self.client.wait_for_run_completion(
                 run_id='foo', timeout=1, sleep_duration=0)
             mock_get_run.assert_called_once_with(run_id='foo')
             assert response == mock_get_run.return_value
 
     def test_wait_for_run_completion_run_timeout_should_raise_error(self):
         with self.assertRaises(TimeoutError):
@@ -180,97 +252,98 @@
                     run_id='foo', timeout=1, sleep_duration=0)
                 mock_get_run.assert_called_once_with(run_id='foo')
 
     @patch('kfp.Client.get_experiment', side_effect=ValueError)
     def test_create_experiment_no_experiment_should_raise_error(
             self, mock_get_experiment):
         with self.assertRaises(ValueError):
-            self.client.create_experiment(name='foo', namespace='foo')
+            self.client.create_experiment(name='foo', namespace='ns1')
             mock_get_experiment.assert_called_once_with(
-                name='foo', namespace='foo')
+                name='foo', namespace='ns1')
 
     @patch('kfp.Client.get_experiment', return_value=Mock(id='foo'))
     @patch('kfp.Client._get_url_prefix', return_value='/pipeline')
     def test_create_experiment_existing_experiment(self, mock_get_url_prefix,
                                                    mock_get_experiment):
         self.client.create_experiment(name='foo')
         mock_get_experiment.assert_called_once_with(
-            experiment_name='foo', namespace='foo')
+            experiment_name='foo', namespace='ns1')
         mock_get_url_prefix.assert_called_once()
 
-    @patch('kfp_server_api.ApiExperiment')
+    @patch('kfp_server_api.V2beta1Experiment')
     @patch(
         'kfp.Client.get_experiment',
         side_effect=ValueError('No experiment is found with name'))
     @patch('kfp.Client._get_url_prefix', return_value='/pipeline')
     def test__create_experiment_name_not_found(self, mock_get_url_prefix,
                                                mock_get_experiment,
                                                mock_api_experiment):
         # experiment with the specified name is not found, so a new experiment
         # is created.
         with patch.object(
                 self.client._experiment_api,
                 'create_experiment',
-                return_value=Mock(id='foo')) as mock_create_experiment:
+                return_value=Mock(
+                    experiment_id='foo')) as mock_create_experiment:
             self.client.create_experiment(name='foo')
             mock_get_experiment.assert_called_once_with(
-                experiment_name='foo', namespace='foo')
+                experiment_name='foo', namespace='ns1')
             mock_api_experiment.assert_called_once()
             mock_create_experiment.assert_called_once()
             mock_get_url_prefix.assert_called_once()
 
     def test_get_experiment_no_experiment_id_or_name_should_raise_error(self):
         with self.assertRaises(ValueError):
             self.client.get_experiment()
 
     @patch('kfp.Client.get_user_namespace', return_value=None)
     def test_get_experiment_does_not_exist_should_raise_error(
             self, mock_get_user_namespace):
         with self.assertRaises(ValueError):
             with patch.object(
                     self.client._experiment_api,
-                    'list_experiment',
+                    'list_experiments',
                     return_value=Mock(
-                        experiments=None)) as mock_list_experiment:
+                        experiments=None)) as mock_list_experiments:
                 self.client.get_experiment(experiment_name='foo')
-                mock_list_experiment.assert_called_once()
+                mock_list_experiments.assert_called_once()
                 mock_get_user_namespace.assert_called_once()
 
     @patch('kfp.Client.get_user_namespace', return_value=None)
     def test_get_experiment_multiple_experiments_with_name_should_raise_error(
             self, mock_get_user_namespace):
         with self.assertRaises(ValueError):
             with patch.object(
                     self.client._experiment_api,
-                    'list_experiment',
+                    'list_experiments',
                     return_value=Mock(
-                        experiments=['foo', 'foo'])) as mock_list_experiment:
+                        experiments=['foo', 'foo'])) as mock_list_experiments:
                 self.client.get_experiment(experiment_name='foo')
-                mock_list_experiment.assert_called_once()
+                mock_list_experiments.assert_called_once()
                 mock_get_user_namespace.assert_called_once()
 
     def test_get_experiment_with_experiment_id(self):
         with patch.object(self.client._experiment_api,
                           'get_experiment') as mock_get_experiment:
             self.client.get_experiment(experiment_id='foo')
-            mock_get_experiment.assert_called_once_with(id='foo')
+            mock_get_experiment.assert_called_once_with(experiment_id='foo')
 
     def test_get_experiment_with_experiment_name_and_namespace(self):
         with patch.object(self.client._experiment_api,
-                          'list_experiment') as mock_list_experiment:
-            self.client.get_experiment(experiment_name='foo', namespace='foo')
-            mock_list_experiment.assert_called_once()
+                          'list_experiments') as mock_list_experiments:
+            self.client.get_experiment(experiment_name='foo', namespace='ns1')
+            mock_list_experiments.assert_called_once()
 
     @patch('kfp.Client.get_user_namespace', return_value=None)
     def test_get_experiment_with_experiment_name_and_no_namespace(
             self, mock_get_user_namespace):
         with patch.object(self.client._experiment_api,
-                          'list_experiment') as mock_list_experiment:
+                          'list_experiments') as mock_list_experiments:
             self.client.get_experiment(experiment_name='foo')
-            mock_list_experiment.assert_called_once()
+            mock_list_experiments.assert_called_once()
             mock_get_user_namespace.assert_called_once()
 
     @patch('kfp_server_api.HealthzServiceApi.get_healthz')
     def test_get_kfp_healthz(self, mock_get_kfp_healthz):
         mock_get_kfp_healthz.return_value = json.dumps([{'foo': 'bar'}])
         response = self.client.get_kfp_healthz()
         mock_get_kfp_healthz.assert_called_once()
@@ -280,10 +353,53 @@
         'kfp_server_api.HealthzServiceApi.get_healthz',
         side_effect=kfp_server_api.ApiException)
     def test_get_kfp_healthz_should_raise_error(self, mock_get_kfp_healthz):
         with self.assertRaises(TimeoutError):
             self.client.get_kfp_healthz(sleep_duration=0)
             mock_get_kfp_healthz.assert_called()
 
+    def test_upload_pipeline_without_name(self):
+
+        @component
+        def return_bool(boolean: bool) -> bool:
+            return boolean
+
+        @pipeline(name='test-upload-without-name', description='description')
+        def pipeline_test_upload_without_name(boolean: bool = True):
+            return_bool(boolean=boolean)
+
+        with patch.object(self.client._upload_api,
+                          'upload_pipeline') as mock_upload_pipeline:
+            with patch.object(self.client, '_is_ipython', return_value=False):
+                with tempfile.TemporaryDirectory() as tmp_path:
+                    pipeline_test_path = os.path.join(tmp_path, 'test.yaml')
+                    Compiler().compile(
+                        pipeline_func=pipeline_test_upload_without_name,
+                        package_path=pipeline_test_path)
+                    self.client.upload_pipeline(
+                        pipeline_package_path=pipeline_test_path,
+                        description='description',
+                        namespace='ns1')
+                    mock_upload_pipeline.assert_called_once_with(
+                        pipeline_test_path,
+                        name='test-upload-without-name',
+                        description='description',
+                        namespace='ns1')
+
+    def test_upload_pipeline_with_name(self):
+        with patch.object(self.client._upload_api,
+                          'upload_pipeline') as mock_upload_pipeline:
+            with patch.object(self.client, '_is_ipython', return_value=False):
+                self.client.upload_pipeline(
+                    pipeline_package_path='fake.yaml',
+                    pipeline_name='overwritten-name',
+                    description='description',
+                    namespace='ns1')
+                mock_upload_pipeline.assert_called_once_with(
+                    'fake.yaml',
+                    name='overwritten-name',
+                    description='description',
+                    namespace='ns1')
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-2.0.0b9/kfp/client/set_volume_credentials.py` & `kfp-2.0.0rc1/kfp/client/set_volume_credentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/set_volume_credentials_test.py` & `kfp-2.0.0rc1/kfp/client/set_volume_credentials_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/token_credentials_base.py` & `kfp-2.0.0rc1/kfp/client/token_credentials_base.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/client/token_credentials_base_test.py` & `kfp-2.0.0rc1/kfp/client/token_credentials_base_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/compiler/__init__.py` & `kfp-2.0.0rc1/kfp/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/compiler/compiler.py` & `kfp-2.0.0rc1/kfp/compiler/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 """KFP DSL compiler.
 
 Implementation of KFP compiler that compiles KFP pipeline into Pipeline IR:
 https://docs.google.com/document/d/1PUDuSQ8vmeKSBloli53mp7GIvzekaY7sggg6ywy35Dk/
 """
 
-from typing import Any, Callable, Dict, Optional, Union
+from typing import Any, Dict, Optional
 
 from kfp.compiler import pipeline_spec_builder as builder
 from kfp.components import base_component
 from kfp.components.types import type_utils
 
 
 class Compiler:
@@ -44,15 +44,15 @@
             package_path='path/to/pipeline.yaml',
             pipeline_parameters={'a': 1},
         )
     """
 
     def compile(
         self,
-        pipeline_func: Union[Callable[..., Any], base_component.BaseComponent],
+        pipeline_func: base_component.BaseComponent,
         package_path: str,
         pipeline_name: Optional[str] = None,
         pipeline_parameters: Optional[Dict[str, Any]] = None,
         type_check: bool = True,
     ) -> None:
         """Compiles the pipeline or component function into IR YAML.
 
@@ -77,8 +77,10 @@
                 pipeline_name=pipeline_name,
                 pipeline_parameters=pipeline_parameters,
             )
 
             builder.write_pipeline_spec_to_file(
                 pipeline_spec=pipeline_spec,
                 pipeline_description=pipeline_func.description,
-                package_path=package_path)
+                platform_spec=pipeline_func.platform_spec,
+                package_path=package_path,
+            )
```

### Comparing `kfp-2.0.0b9/kfp/compiler/pipeline_spec_builder.py` & `kfp-2.0.0rc1/kfp/compiler/pipeline_spec_builder.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Functions for creating PipelineSpec proto objects."""
 
+import copy
 import json
-from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
+import typing
+from typing import (Any, DefaultDict, Dict, List, Mapping, Optional, Tuple,
+                    Union)
 import warnings
 
 from google.protobuf import json_format
 from google.protobuf import struct_pb2
 import kfp
 from kfp.compiler import compiler_utils
 from kfp.components import for_loop
@@ -41,45 +44,34 @@
     tasks_group.TasksGroupType.FOR_LOOP: tasks_group.ParallelFor,
     tasks_group.TasksGroupType.EXIT_HANDLER: tasks_group.ExitHandler,
 }
 
 _SINGLE_OUTPUT_NAME = 'Output'
 
 
-def _additional_input_name_for_pipeline_channel(
-        channel_or_name: Union[pipeline_channel.PipelineChannel, str]) -> str:
-    """Gets the name for an additional (compiler-injected) input."""
-
-    # Adding a prefix to avoid (reduce chance of) name collision between the
-    # original component inputs and the injected input.
-    return 'pipelinechannel--' + (
-        channel_or_name.full_name if isinstance(
-            channel_or_name, pipeline_channel.PipelineChannel) else
-        channel_or_name)
-
-
 def to_protobuf_value(value: type_utils.PARAMETER_TYPES) -> struct_pb2.Value:
     """Creates a google.protobuf.struct_pb2.Value message out of a provide
     value.
 
     Args:
         value: The value to be converted to Value message.
 
     Returns:
          A google.protobuf.struct_pb2.Value message.
 
     Raises:
         ValueError if the given value is not one of the parameter types.
     """
-    if isinstance(value, str):
+    # bool check must be above (int, float) check because bool is a subclass of int so isinstance(True, int) == True
+    if isinstance(value, bool):
+        return struct_pb2.Value(bool_value=value)
+    elif isinstance(value, str):
         return struct_pb2.Value(string_value=value)
     elif isinstance(value, (int, float)):
         return struct_pb2.Value(number_value=value)
-    elif isinstance(value, bool):
-        return struct_pb2.Value(bool_value=value)
     elif isinstance(value, dict):
         return struct_pb2.Value(
             struct_value=struct_pb2.Struct(
                 fields={k: to_protobuf_value(v) for k, v in value.items()}))
     elif isinstance(value, list):
         return struct_pb2.Value(
             list_value=struct_pb2.ListValue(
@@ -133,93 +125,101 @@
         task._task_spec.enable_caching)
 
     if task._task_spec.retry_policy is not None:
         pipeline_task_spec.retry_policy.CopyFrom(
             task._task_spec.retry_policy.to_proto())
 
     for input_name, input_value in task.inputs.items():
-        if isinstance(input_value, pipeline_channel.PipelineArtifactChannel):
+
+        if isinstance(input_value,
+                      pipeline_channel.PipelineArtifactChannel) or (
+                          isinstance(input_value, for_loop.Collected) and
+                          input_value.is_artifact_channel):
 
             if input_value.task_name:
                 # Value is produced by an upstream task.
                 if input_value.task_name in tasks_in_current_dag:
                     # Dependent task within the same DAG.
                     pipeline_task_spec.inputs.artifacts[
                         input_name].task_output_artifact.producer_task = (
                             utils.sanitize_task_name(input_value.task_name))
                     pipeline_task_spec.inputs.artifacts[
                         input_name].task_output_artifact.output_artifact_key = (
                             input_value.name)
                 else:
                     # Dependent task not from the same DAG.
                     component_input_artifact = (
-                        _additional_input_name_for_pipeline_channel(input_value)
-                    )
+                        compiler_utils.
+                        additional_input_name_for_pipeline_channel(input_value))
                     assert component_input_artifact in parent_component_inputs.artifacts, \
                         f'component_input_artifact: {component_input_artifact} not found. All inputs: {parent_component_inputs}'
                     pipeline_task_spec.inputs.artifacts[
                         input_name].component_input_artifact = (
                             component_input_artifact)
             else:
                 component_input_artifact = input_value.full_name
                 if component_input_artifact not in parent_component_inputs.artifacts:
                     component_input_artifact = (
-                        _additional_input_name_for_pipeline_channel(input_value)
-                    )
+                        compiler_utils.
+                        additional_input_name_for_pipeline_channel(input_value))
                 pipeline_task_spec.inputs.artifacts[
                     input_name].component_input_artifact = (
                         component_input_artifact)
 
-        elif isinstance(input_value, pipeline_channel.PipelineParameterChannel):
-
+        elif isinstance(input_value,
+                        pipeline_channel.PipelineParameterChannel) or (
+                            isinstance(input_value, for_loop.Collected) and
+                            not input_value.is_artifact_channel):
             if input_value.task_name:
+
                 # Value is produced by an upstream task.
                 if input_value.task_name in tasks_in_current_dag:
                     # Dependent task within the same DAG.
                     pipeline_task_spec.inputs.parameters[
                         input_name].task_output_parameter.producer_task = (
                             utils.sanitize_task_name(input_value.task_name))
                     pipeline_task_spec.inputs.parameters[
                         input_name].task_output_parameter.output_parameter_key = (
                             input_value.name)
                 else:
                     # Dependent task not from the same DAG.
                     component_input_parameter = (
-                        _additional_input_name_for_pipeline_channel(input_value)
-                    )
+                        compiler_utils.
+                        additional_input_name_for_pipeline_channel(input_value))
                     assert component_input_parameter in parent_component_inputs.parameters, \
                         f'component_input_parameter: {component_input_parameter} not found. All inputs: {parent_component_inputs}'
                     pipeline_task_spec.inputs.parameters[
                         input_name].component_input_parameter = (
                             component_input_parameter)
             else:
                 # Value is from pipeline input.
                 component_input_parameter = input_value.full_name
                 if component_input_parameter not in parent_component_inputs.parameters:
                     component_input_parameter = (
-                        _additional_input_name_for_pipeline_channel(input_value)
-                    )
+                        compiler_utils.
+                        additional_input_name_for_pipeline_channel(input_value))
                 pipeline_task_spec.inputs.parameters[
                     input_name].component_input_parameter = (
                         component_input_parameter)
 
         elif isinstance(input_value, for_loop.LoopArgument):
 
             component_input_parameter = (
-                _additional_input_name_for_pipeline_channel(input_value))
+                compiler_utils.additional_input_name_for_pipeline_channel(
+                    input_value))
             assert component_input_parameter in parent_component_inputs.parameters, \
                 f'component_input_parameter: {component_input_parameter} not found. All inputs: {parent_component_inputs}'
             pipeline_task_spec.inputs.parameters[
                 input_name].component_input_parameter = (
                     component_input_parameter)
 
         elif isinstance(input_value, for_loop.LoopArgumentVariable):
 
             component_input_parameter = (
-                _additional_input_name_for_pipeline_channel(
+                compiler_utils.additional_input_name_for_pipeline_channel(
                     input_value.loop_argument))
             assert component_input_parameter in parent_component_inputs.parameters, \
                 f'component_input_parameter: {component_input_parameter} not found. All inputs: {parent_component_inputs}'
             pipeline_task_spec.inputs.parameters[
                 input_name].component_input_parameter = (
                     component_input_parameter)
             pipeline_task_spec.inputs.parameters[
@@ -234,15 +234,16 @@
             for channel in pipeline_channels:
                 # value contains PipelineChannel placeholders which needs to be
                 # replaced. And the input needs to be added to the task spec.
 
                 # Form the name for the compiler injected input, and make sure it
                 # doesn't collide with any existing input names.
                 additional_input_name = (
-                    _additional_input_name_for_pipeline_channel(channel))
+                    compiler_utils.additional_input_name_for_pipeline_channel(
+                        channel))
 
                 # We don't expect collision to happen because we prefix the name
                 # of additional input with 'pipelinechannel--'. But just in case
                 # collision did happend, throw a RuntimeError so that we don't
                 # get surprise at runtime.
                 for existing_input_name, _ in task.inputs.items():
                     if existing_input_name == additional_input_name:
@@ -259,33 +260,33 @@
                     # Value is produced by an upstream task.
                     if channel.task_name in tasks_in_current_dag:
                         # Dependent task within the same DAG.
                         pipeline_task_spec.inputs.parameters[
                             additional_input_name].task_output_parameter.producer_task = (
                                 utils.sanitize_task_name(channel.task_name))
                         pipeline_task_spec.inputs.parameters[
-                            input_name].task_output_parameter.output_parameter_key = (
+                            additional_input_name].task_output_parameter.output_parameter_key = (
                                 channel.name)
                     else:
                         # Dependent task not from the same DAG.
                         component_input_parameter = (
-                            _additional_input_name_for_pipeline_channel(channel)
-                        )
+                            compiler_utils.
+                            additional_input_name_for_pipeline_channel(channel))
                         assert component_input_parameter in parent_component_inputs.parameters, \
                             f'component_input_parameter: {component_input_parameter} not found. All inputs: {parent_component_inputs}'
                         pipeline_task_spec.inputs.parameters[
                             additional_input_name].component_input_parameter = (
                                 component_input_parameter)
                 else:
                     # Value is from pipeline input. (or loop?)
                     component_input_parameter = channel.full_name
                     if component_input_parameter not in parent_component_inputs.parameters:
                         component_input_parameter = (
-                            _additional_input_name_for_pipeline_channel(channel)
-                        )
+                            compiler_utils.
+                            additional_input_name_for_pipeline_channel(channel))
                     pipeline_task_spec.inputs.parameters[
                         additional_input_name].component_input_parameter = (
                             component_input_parameter)
 
             pipeline_task_spec.inputs.parameters[
                 input_name].runtime_value.constant.string_value = input_value
 
@@ -297,188 +298,175 @@
 
         else:
             raise ValueError(
                 'Input argument supports only the following types: '
                 'str, int, float, bool, dict, and list.'
                 f'Got {input_value} of type {type(input_value)}.')
 
+    if task._ignore_upstream_failure_tag:
+        pipeline_task_spec.trigger_policy.strategy = (
+            pipeline_spec_pb2.PipelineTaskSpec.TriggerPolicy.TriggerStrategy
+            .ALL_UPSTREAM_TASKS_COMPLETED)
+
     return pipeline_task_spec
 
 
 def build_component_spec_for_exit_task(
     task: pipeline_task.PipelineTask,) -> pipeline_spec_pb2.ComponentSpec:
     """Builds ComponentSpec for an exit task.
 
     Args:
         task: The task to build a ComponentSpec for.
 
     Returns:
         A ComponentSpec object for the exit task.
     """
-    return build_component_spec_for_task(task=task, is_exit_task=True)
+    return build_component_spec_for_task(
+        task=task, is_compiled_component=False, is_exit_task=True)
 
 
 def build_component_spec_for_task(
     task: pipeline_task.PipelineTask,
+    is_compiled_component: bool,
     is_exit_task: bool = False,
 ) -> pipeline_spec_pb2.ComponentSpec:
     """Builds ComponentSpec for a pipeline task.
 
     Args:
         task: The task to build a ComponentSpec for.
         is_exit_task: Whether the task is used as exit task in Exit Handler.
 
     Returns:
         A ComponentSpec object for the task.
     """
-    component_spec = pipeline_spec_pb2.ComponentSpec()
-    component_spec.executor_label = utils.sanitize_executor_label(task.name)
-
     for input_name, input_spec in (task.component_spec.inputs or {}).items():
+        if not is_exit_task and type_utils.is_task_final_status_type(
+                input_spec.type) and not is_compiled_component:
+            raise ValueError(
+                f'PipelineTaskFinalStatus can only be used in an exit task. Parameter {input_name} of a non exit task has type PipelineTaskFinalStatus.'
+            )
 
-        # Special handling for PipelineTaskFinalStatus first.
-        if type_utils.is_task_final_status_type(input_spec.type):
-            if not is_exit_task:
-                raise ValueError(
-                    'PipelineTaskFinalStatus can only be used in an exit task.')
-            component_spec.input_definitions.parameters[
-                input_name].parameter_type = pipeline_spec_pb2.ParameterType.STRUCT
-            continue
-
-        # skip inputs not present, as a workaround to support optional inputs.
-        if input_name not in task.inputs and input_spec.default is None:
-            continue
-
-        if type_utils.is_parameter_type(input_spec.type):
-            component_spec.input_definitions.parameters[
-                input_name].parameter_type = type_utils.get_parameter_type(
-                    input_spec.type)
-            if input_spec.default is not None:
-                _fill_in_component_input_default_value(
-                    component_spec=component_spec,
-                    input_name=input_name,
-                    default_value=input_spec.default,
-                )
-
-        else:
-            component_spec.input_definitions.artifacts[
-                input_name].artifact_type.CopyFrom(
-                    type_utils.bundled_artifact_to_artifact_proto(
-                        input_spec.type))
-
-    for output_name, output_spec in (task.component_spec.outputs or {}).items():
-        if type_utils.is_parameter_type(output_spec.type):
-            component_spec.output_definitions.parameters[
-                output_name].parameter_type = type_utils.get_parameter_type(
-                    output_spec.type)
-        else:
-            component_spec.output_definitions.artifacts[
-                output_name].artifact_type.CopyFrom(
-                    type_utils.bundled_artifact_to_artifact_proto(
-                        output_spec.type))
-
+    component_spec = _build_component_spec_from_component_spec_structure(
+        task.component_spec)
+    component_spec.executor_label = utils.sanitize_executor_label(task.name)
     return component_spec
 
 
-# TODO(chensun): merge with build_component_spec_for_task
 def _build_component_spec_from_component_spec_structure(
-    component_spec_struct: structures.ComponentSpec,
+    component_spec_struct: structures.ComponentSpec
 ) -> pipeline_spec_pb2.ComponentSpec:
     """Builds ComponentSpec proto from ComponentSpec structure."""
     component_spec = pipeline_spec_pb2.ComponentSpec()
 
     for input_name, input_spec in (component_spec_struct.inputs or {}).items():
 
         # Special handling for PipelineTaskFinalStatus first.
         if type_utils.is_task_final_status_type(input_spec.type):
             component_spec.input_definitions.parameters[
-                input_name].parameter_type = pipeline_spec_pb2.ParameterType.STRUCT
-            continue
+                input_name].parameter_type = pipeline_spec_pb2.ParameterType.TASK_FINAL_STATUS
+            component_spec.input_definitions.parameters[
+                input_name].is_optional = True
+            if input_spec.description:
+                component_spec.input_definitions.parameters[
+                    input_name].description = input_spec.description
 
-        if type_utils.is_parameter_type(input_spec.type):
+        elif type_utils.is_parameter_type(input_spec.type):
             component_spec.input_definitions.parameters[
                 input_name].parameter_type = type_utils.get_parameter_type(
                     input_spec.type)
-            if input_spec.default is not None:
+            if input_spec.optional:
+                component_spec.input_definitions.parameters[
+                    input_name].is_optional = True
                 _fill_in_component_input_default_value(
                     component_spec=component_spec,
                     input_name=input_name,
                     default_value=input_spec.default,
                 )
+            if input_spec.description:
+                component_spec.input_definitions.parameters[
+                    input_name].description = input_spec.description
 
         else:
             component_spec.input_definitions.artifacts[
                 input_name].artifact_type.CopyFrom(
                     type_utils.bundled_artifact_to_artifact_proto(
                         input_spec.type))
+            component_spec.input_definitions.artifacts[
+                input_name].is_artifact_list = input_spec.is_artifact_list
+            if input_spec.optional:
+                component_spec.input_definitions.artifacts[
+                    input_name].is_optional = True
+            if input_spec.description:
+                component_spec.input_definitions.artifacts[
+                    input_name].description = input_spec.description
 
     for output_name, output_spec in (component_spec_struct.outputs or
                                      {}).items():
         if type_utils.is_parameter_type(output_spec.type):
             component_spec.output_definitions.parameters[
                 output_name].parameter_type = type_utils.get_parameter_type(
                     output_spec.type)
+            if output_spec.description:
+                component_spec.output_definitions.parameters[
+                    output_name].description = output_spec.description
         else:
             component_spec.output_definitions.artifacts[
                 output_name].artifact_type.CopyFrom(
                     type_utils.bundled_artifact_to_artifact_proto(
                         output_spec.type))
+            component_spec.output_definitions.artifacts[
+                output_name].is_artifact_list = output_spec.is_artifact_list
+            if output_spec.description:
+                component_spec.output_definitions.artifacts[
+                    output_name].description = output_spec.description
 
     return component_spec
 
 
 def _connect_dag_outputs(
     component_spec: pipeline_spec_pb2.ComponentSpec,
     output_name: str,
     output_channel: pipeline_channel.PipelineChannel,
 ) -> None:
-    """Connects dag ouptut to a subtask output.
+    """Connects dag output to a subtask output.
 
     Args:
         component_spec: The component spec to modify its dag outputs.
         output_name: The name of the dag output.
         output_channel: The pipeline channel selected for the dag output.
     """
     if isinstance(output_channel, pipeline_channel.PipelineArtifactChannel):
         if output_name not in component_spec.output_definitions.artifacts:
-            raise ValueError(f'Pipeline output not defined: {output_name}.')
+            raise ValueError(
+                f'Pipeline or component output not defined: {output_name}. You may be missing a type annotation.'
+            )
         component_spec.dag.outputs.artifacts[
             output_name].artifact_selectors.append(
                 pipeline_spec_pb2.DagOutputsSpec.ArtifactSelectorSpec(
                     producer_subtask=output_channel.task_name,
                     output_artifact_key=output_channel.name,
                 ))
     elif isinstance(output_channel, pipeline_channel.PipelineParameterChannel):
         if output_name not in component_spec.output_definitions.parameters:
-            raise ValueError(f'Pipeline output not defined: {output_name}.')
+            raise ValueError(
+                f'Pipeline or component output not defined: {output_name}. You may be missing a type annotation.'
+            )
         component_spec.dag.outputs.parameters[
             output_name].value_from_parameter.producer_subtask = output_channel.task_name
         component_spec.dag.outputs.parameters[
             output_name].value_from_parameter.output_parameter_key = output_channel.name
 
 
 def _build_dag_outputs(
     component_spec: pipeline_spec_pb2.ComponentSpec,
-    dag_outputs: Optional[Any],
+    dag_outputs: Dict[str, pipeline_channel.PipelineChannel],
 ) -> None:
     """Builds DAG output spec."""
-    if dag_outputs is not None:
-        if isinstance(dag_outputs, pipeline_channel.PipelineChannel):
-            _connect_dag_outputs(
-                component_spec=component_spec,
-                output_name=_SINGLE_OUTPUT_NAME,
-                output_channel=dag_outputs,
-            )
-        elif isinstance(dag_outputs, tuple) and hasattr(dag_outputs, '_asdict'):
-            for output_name, output_channel in dag_outputs._asdict().items():
-                _connect_dag_outputs(
-                    component_spec=component_spec,
-                    output_name=output_name,
-                    output_channel=output_channel,
-                )
+    for output_name, output_channel in dag_outputs.items():
+        _connect_dag_outputs(component_spec, output_name, output_channel)
     # Valid dag outputs covers all outptus in component definition.
     for output_name in component_spec.output_definitions.artifacts:
         if output_name not in component_spec.dag.outputs.artifacts:
             raise ValueError(f'Missing pipeline output: {output_name}.')
     for output_name in component_spec.output_definitions.parameters:
         if output_name not in component_spec.dag.outputs.parameters:
             raise ValueError(f'Missing pipeline output: {output_name}.')
@@ -533,18 +521,26 @@
             env=[
                 pipeline_spec_pb2.PipelineDeploymentConfig.PipelineContainerSpec
                 .EnvVar(name=name, value=value)
                 for name, value in (task.container_spec.env or {}).items()
             ]))
 
     if task.container_spec.resources is not None:
-        container_spec.resources.cpu_limit = (
-            task.container_spec.resources.cpu_limit)
-        container_spec.resources.memory_limit = (
-            task.container_spec.resources.memory_limit)
+        if task.container_spec.resources.cpu_request is not None:
+            container_spec.resources.cpu_request = (
+                task.container_spec.resources.cpu_request)
+        if task.container_spec.resources.cpu_limit is not None:
+            container_spec.resources.cpu_limit = (
+                task.container_spec.resources.cpu_limit)
+        if task.container_spec.resources.memory_request is not None:
+            container_spec.resources.memory_request = (
+                task.container_spec.resources.memory_request)
+        if task.container_spec.resources.memory_limit is not None:
+            container_spec.resources.memory_limit = (
+                task.container_spec.resources.memory_limit)
         if task.container_spec.resources.accelerator_count is not None:
             container_spec.resources.accelerator.CopyFrom(
                 pipeline_spec_pb2.PipelineDeploymentConfig.PipelineContainerSpec
                 .ResourceSpec.AcceleratorConfig(
                     type=task.container_spec.resources.accelerator_type,
                     count=task.container_spec.resources.accelerator_count,
                 ))
@@ -566,23 +562,19 @@
     """
     if default_value is None:
         return
 
     parameter_type = component_spec.input_definitions.parameters[
         input_name].parameter_type
     if pipeline_spec_pb2.ParameterType.NUMBER_INTEGER == parameter_type:
-        # cast to int to support v1 component YAML where NUMBER_INTEGER defaults are included as strings
-        # for example, input Limit: https://raw.githubusercontent.com/kubeflow/pipelines/60a2612541ec08c6a85c237d2ec7525b12543a43/components/datasets/Chicago_Taxi_Trips/component.yaml
         component_spec.input_definitions.parameters[
-            input_name].default_value.number_value = int(default_value)
-        # cast to int to support v1 component YAML where NUMBER_DOUBLE defaults are included as strings
-        # for example, input learning_rate: https://raw.githubusercontent.com/kubeflow/pipelines/567c04c51ff00a1ee525b3458425b17adbe3df61/components/XGBoost/Train/component.yaml
+            input_name].default_value.number_value = default_value
     elif pipeline_spec_pb2.ParameterType.NUMBER_DOUBLE == parameter_type:
         component_spec.input_definitions.parameters[
-            input_name].default_value.number_value = float(default_value)
+            input_name].default_value.number_value = default_value
     elif pipeline_spec_pb2.ParameterType.STRING == parameter_type:
         component_spec.input_definitions.parameters[
             input_name].default_value.string_value = default_value
     elif pipeline_spec_pb2.ParameterType.BOOLEAN == parameter_type:
         component_spec.input_definitions.parameters[
             input_name].default_value.bool_value = default_value
     elif pipeline_spec_pb2.ParameterType.STRUCT == parameter_type:
@@ -592,52 +584,58 @@
     elif pipeline_spec_pb2.ParameterType.LIST == parameter_type:
         component_spec.input_definitions.parameters[
             input_name].default_value.CopyFrom(
                 to_protobuf_value(default_value))
 
 
 def build_component_spec_for_group(
-    pipeline_channels: List[pipeline_channel.PipelineChannel],
-    is_root_group: bool,
+    input_pipeline_channels: List[pipeline_channel.PipelineChannel],
+    output_pipeline_channels: Dict[str, pipeline_channel.PipelineChannel],
 ) -> pipeline_spec_pb2.ComponentSpec:
     """Builds ComponentSpec for a TasksGroup.
 
     Args:
         group: The group to build a ComponentSpec for.
         pipeline_channels: The list of pipeline channels referenced by the group.
 
     Returns:
         A PipelineTaskSpec object representing the loop group.
     """
     component_spec = pipeline_spec_pb2.ComponentSpec()
 
-    for channel in pipeline_channels:
-
-        input_name = (
-            channel.name if is_root_group else
-            _additional_input_name_for_pipeline_channel(channel))
+    for channel in input_pipeline_channels:
+        input_name = compiler_utils.additional_input_name_for_pipeline_channel(
+            channel)
 
         if isinstance(channel, pipeline_channel.PipelineArtifactChannel):
             component_spec.input_definitions.artifacts[
                 input_name].artifact_type.CopyFrom(
                     type_utils.bundled_artifact_to_artifact_proto(
                         channel.channel_type))
+            component_spec.input_definitions.artifacts[
+                input_name].is_artifact_list = channel.is_artifact_list
         else:
             # channel is one of PipelineParameterChannel, LoopArgument, or
             # LoopArgumentVariable.
             component_spec.input_definitions.parameters[
                 input_name].parameter_type = type_utils.get_parameter_type(
                     channel.channel_type)
 
-            if is_root_group:
-                _fill_in_component_input_default_value(
-                    component_spec=component_spec,
-                    input_name=input_name,
-                    default_value=channel.value,
-                )
+    for output_name, output in output_pipeline_channels.items():
+        if isinstance(output, pipeline_channel.PipelineArtifactChannel):
+            component_spec.output_definitions.artifacts[
+                output_name].artifact_type.CopyFrom(
+                    type_utils.bundled_artifact_to_artifact_proto(
+                        output.channel_type))
+            component_spec.output_definitions.artifacts[
+                output_name].is_artifact_list = output.is_artifact_list
+        else:
+            component_spec.output_definitions.parameters[
+                output_name].parameter_type = type_utils.get_parameter_type(
+                    channel.channel_type)
 
     return component_spec
 
 
 def _pop_input_from_task_spec(
     task_spec: pipeline_spec_pb2.PipelineTaskSpec,
     input_name: str,
@@ -663,17 +661,17 @@
 
     Args:
         group: The loop group to update task spec for.
         pipeline_task_spec: The pipeline task spec to update in place.
     """
     if group.items_is_pipeline_channel:
         loop_items_channel = group.loop_argument.items_or_pipeline_channel
-        input_parameter_name = _additional_input_name_for_pipeline_channel(
+        input_parameter_name = compiler_utils.additional_input_name_for_pipeline_channel(
             loop_items_channel)
-        loop_argument_item_name = _additional_input_name_for_pipeline_channel(
+        loop_argument_item_name = compiler_utils.additional_input_name_for_pipeline_channel(
             group.loop_argument.full_name)
 
         loop_arguments_item = f'{input_parameter_name}-{for_loop.LoopArgument.LOOP_ITEM_NAME_BASE}'
         assert loop_arguments_item == loop_argument_item_name
 
         pipeline_task_spec.parameter_iterator.items.input_parameter = (
             input_parameter_name)
@@ -685,19 +683,19 @@
         if isinstance(loop_items_channel, for_loop.LoopArgumentVariable):
             pipeline_task_spec.inputs.parameters[
                 input_parameter_name].parameter_expression_selector = (
                     f'parseJson(string_value)["{loop_items_channel.subvar_name}"]'
                 )
             pipeline_task_spec.inputs.parameters[
                 input_parameter_name].component_input_parameter = (
-                    _additional_input_name_for_pipeline_channel(
+                    compiler_utils.additional_input_name_for_pipeline_channel(
                         loop_items_channel.loop_argument))
 
     else:
-        input_parameter_name = _additional_input_name_for_pipeline_channel(
+        input_parameter_name = compiler_utils.additional_input_name_for_pipeline_channel(
             group.loop_argument)
         raw_values = group.loop_argument.items_or_pipeline_channel
 
         pipeline_task_spec.parameter_iterator.items.raw = json.dumps(
             raw_values, sort_keys=True)
         pipeline_task_spec.parameter_iterator.item_input = (
             input_parameter_name)
@@ -733,15 +731,15 @@
                 value_or_reference.channel_type)
             if parameter_type in [
                     pipeline_spec_pb2.ParameterType.STRUCT,
                     pipeline_spec_pb2.ParameterType.LIST,
                     pipeline_spec_pb2.ParameterType
                     .PARAMETER_TYPE_ENUM_UNSPECIFIED,
             ]:
-                input_name = _additional_input_name_for_pipeline_channel(
+                input_name = compiler_utils.additional_input_name_for_pipeline_channel(
                     value_or_reference)
                 raise ValueError(
                     f'Conditional requires scalar parameter values for comparison. Found input "{input_name}" of type {value_or_reference.channel_type} in pipeline definition instead.'
                 )
     parameter_types = set()
     for value_or_reference in [left_operand, right_operand]:
         if isinstance(value_or_reference, pipeline_channel.PipelineChannel):
@@ -776,15 +774,15 @@
         raise ValueError(
             f'Unable to determine operand types for "{left_operand}" and "{right_operand}"'
         )
 
     operand_values = []
     for value_or_reference in [left_operand, right_operand]:
         if isinstance(value_or_reference, pipeline_channel.PipelineChannel):
-            input_name = _additional_input_name_for_pipeline_channel(
+            input_name = compiler_utils.additional_input_name_for_pipeline_channel(
                 value_or_reference)
             operand_value = f"inputs.parameter_values['{input_name}']"
             parameter_type = type_utils.get_parameter_type(
                 value_or_reference.channel_type)
             if parameter_type == pipeline_spec_pb2.ParameterType.NUMBER_INTEGER:
                 operand_value = f'int({operand_value})'
         elif isinstance(value_or_reference, str):
@@ -909,15 +907,16 @@
 
         channel_full_name = channel.full_name
         subvar_name = None
         if isinstance(channel, for_loop.LoopArgumentVariable):
             channel_full_name = channel.loop_argument.full_name
             subvar_name = channel.subvar_name
 
-        input_name = _additional_input_name_for_pipeline_channel(channel)
+        input_name = compiler_utils.additional_input_name_for_pipeline_channel(
+            channel)
 
         channel_name = channel.name
         if subvar_name:
             pipeline_task_spec.inputs.parameters[
                 input_name].parameter_expression_selector = (
                     f'parseJson(string_value)["{subvar_name}"]')
             if not channel.is_with_items_loop_argument:
@@ -943,15 +942,15 @@
             pipeline_task_spec.inputs.parameters[
                 input_name].task_output_parameter.output_parameter_key = (
                     channel_name)
         else:
             pipeline_task_spec.inputs.parameters[
                 input_name].component_input_parameter = (
                     channel_full_name if is_parent_component_root else
-                    _additional_input_name_for_pipeline_channel(
+                    compiler_utils.additional_input_name_for_pipeline_channel(
                         channel_full_name))
 
     if isinstance(group, tasks_group.ParallelFor):
         _update_task_spec_for_loop_group(
             group=group,
             pipeline_task_spec=pipeline_task_spec,
         )
@@ -1068,20 +1067,23 @@
 
 
 def build_spec_by_group(
     pipeline_spec: pipeline_spec_pb2.PipelineSpec,
     deployment_config: pipeline_spec_pb2.PipelineDeploymentConfig,
     group: tasks_group.TasksGroup,
     inputs: Mapping[str, List[Tuple[pipeline_channel.PipelineChannel, str]]],
+    outputs: DefaultDict[str, Dict[str, pipeline_channel.PipelineChannel]],
     dependencies: Dict[str, List[compiler_utils.GroupOrTaskType]],
     rootgroup_name: str,
     task_name_to_parent_groups: Mapping[str,
                                         List[compiler_utils.GroupOrTaskType]],
     group_name_to_parent_groups: Mapping[str, List[tasks_group.TasksGroup]],
     name_to_for_loop_group: Mapping[str, tasks_group.ParallelFor],
+    platform_spec: pipeline_spec_pb2.PlatformSpec,
+    is_compiled_component: bool,
 ) -> None:
     """Generates IR spec given a TasksGroup.
 
     Args:
         pipeline_spec: The pipeline_spec to update in place.
         deployment_config: The deployment_config to hold all executors. The
             spec is updated in place.
@@ -1115,71 +1117,88 @@
     task_name_to_task_spec = {}
     task_name_to_component_spec = {}
 
     # Generate task specs and component specs for the dag.
     subgroups = group.groups + group.tasks
     for subgroup in subgroups:
 
-        subgroup_inputs = inputs.get(subgroup.name, [])
-        subgroup_channels = [channel for channel, _ in subgroup_inputs]
+        subgroup_input_channels = [
+            channel for channel, _ in inputs.get(subgroup.name, [])
+        ]
+        subgroup_output_channels = outputs.get(subgroup.name, {})
 
         subgroup_component_name = (utils.sanitize_component_name(subgroup.name))
 
         tasks_in_current_dag = [
             utils.sanitize_task_name(subgroup.name) for subgroup in subgroups
         ]
         is_parent_component_root = (group_component_spec == pipeline_spec.root)
 
         if isinstance(subgroup, pipeline_task.PipelineTask):
-
             subgroup_task_spec = build_task_spec_for_task(
                 task=subgroup,
                 parent_component_inputs=group_component_spec.input_definitions,
                 tasks_in_current_dag=tasks_in_current_dag,
             )
             task_name_to_task_spec[subgroup.name] = subgroup_task_spec
-
             subgroup_component_spec = build_component_spec_for_task(
-                task=subgroup)
+                task=subgroup,
+                is_compiled_component=is_compiled_component,
+            )
             task_name_to_component_spec[subgroup.name] = subgroup_component_spec
 
             if subgroup_component_spec.executor_label:
                 executor_label = utils.make_name_unique_by_adding_index(
                     name=subgroup_component_spec.executor_label,
                     collection=list(deployment_config.executors.keys()),
                     delimiter='-')
                 subgroup_component_spec.executor_label = executor_label
 
             if subgroup.container_spec is not None:
                 subgroup_container_spec = build_container_spec_for_task(
                     task=subgroup)
                 deployment_config.executors[executor_label].container.CopyFrom(
                     subgroup_container_spec)
+                single_task_platform_spec = platform_config_to_platform_spec(
+                    subgroup.platform_config,
+                    executor_label,
+                )
+                merge_platform_specs(
+                    platform_spec,
+                    single_task_platform_spec,
+                )
+
             elif subgroup.importer_spec is not None:
                 subgroup_importer_spec = build_importer_spec_for_task(
                     task=subgroup)
                 deployment_config.executors[executor_label].importer.CopyFrom(
                     subgroup_importer_spec)
             elif subgroup.pipeline_spec is not None:
-                sub_pipeline_spec = merge_deployment_spec_and_component_spec(
+                if subgroup.platform_config:
+                    raise ValueError(
+                        'Platform-specific features can only be set on primitive components. Found platform-specific feature set on a pipeline.'
+                    )
+                sub_pipeline_spec, platform_spec = merge_deployment_spec_and_component_spec(
                     main_pipeline_spec=pipeline_spec,
                     main_deployment_config=deployment_config,
                     sub_pipeline_spec=subgroup.pipeline_spec,
+                    main_platform_spec=platform_spec,
+                    sub_platform_spec=subgroup.platform_spec,
                 )
                 subgroup_component_spec = sub_pipeline_spec.root
             else:
                 raise RuntimeError
         elif isinstance(subgroup, tasks_group.ParallelFor):
 
             # "Punch the hole", adding additional inputs (other than loop
             # arguments which will be handled separately) needed by its
             # subgroups or tasks.
             loop_subgroup_channels = []
 
-            for channel in subgroup_channels:
+            for channel in subgroup_input_channels:
                 # Skip 'withItems' loop arguments if it's from an inner loop.
                 if isinstance(
                         channel,
                     (for_loop.LoopArgument, for_loop.LoopArgumentVariable
                     )) and channel.is_with_items_loop_argument:
                     withitems_loop_arg_found_in_self_or_upstream = False
                     for group_name in group_name_to_parent_groups[
@@ -1199,59 +1218,65 @@
                 # another task or an input as global pipeline parameters.
                 loop_subgroup_channels.append(
                     subgroup.loop_argument.items_or_pipeline_channel)
 
             loop_subgroup_channels.append(subgroup.loop_argument)
 
             subgroup_component_spec = build_component_spec_for_group(
-                pipeline_channels=loop_subgroup_channels,
-                is_root_group=False,
+                input_pipeline_channels=loop_subgroup_channels,
+                output_pipeline_channels=subgroup_output_channels,
             )
 
             subgroup_task_spec = build_task_spec_for_group(
                 group=subgroup,
                 pipeline_channels=loop_subgroup_channels,
                 tasks_in_current_dag=tasks_in_current_dag,
                 is_parent_component_root=is_parent_component_root,
             )
 
+            _build_dag_outputs(subgroup_component_spec,
+                               subgroup_output_channels)
+
         elif isinstance(subgroup, tasks_group.Condition):
 
             # "Punch the hole", adding inputs needed by its subgroups or
             # tasks.
-            condition_subgroup_channels = list(subgroup_channels)
+            condition_subgroup_channels = list(subgroup_input_channels)
             for operand in [
                     subgroup.condition.left_operand,
                     subgroup.condition.right_operand,
             ]:
                 if isinstance(operand, pipeline_channel.PipelineChannel):
                     condition_subgroup_channels.append(operand)
 
             subgroup_component_spec = build_component_spec_for_group(
-                pipeline_channels=condition_subgroup_channels,
-                is_root_group=False,
+                input_pipeline_channels=condition_subgroup_channels,
+                output_pipeline_channels=subgroup_output_channels,
             )
 
             subgroup_task_spec = build_task_spec_for_group(
                 group=subgroup,
                 pipeline_channels=condition_subgroup_channels,
                 tasks_in_current_dag=tasks_in_current_dag,
                 is_parent_component_root=is_parent_component_root,
             )
 
+            _build_dag_outputs(subgroup_component_spec,
+                               subgroup_output_channels)
+
         elif isinstance(subgroup, tasks_group.ExitHandler):
 
             subgroup_component_spec = build_component_spec_for_group(
-                pipeline_channels=subgroup_channels,
-                is_root_group=False,
+                input_pipeline_channels=subgroup_input_channels,
+                output_pipeline_channels={},
             )
 
             subgroup_task_spec = build_task_spec_for_group(
                 group=subgroup,
-                pipeline_channels=subgroup_channels,
+                pipeline_channels=subgroup_input_channels,
                 tasks_in_current_dag=tasks_in_current_dag,
                 is_parent_component_root=is_parent_component_root,
             )
 
         else:
             raise RuntimeError(
                 f'Unexpected task/group type: Got {subgroup} of type '
@@ -1286,19 +1311,67 @@
         tasks=group.tasks,
         task_name_to_parent_groups=task_name_to_parent_groups,
         task_name_to_component_spec=task_name_to_component_spec,
         pipeline_spec=pipeline_spec,
     )
 
 
+def platform_config_to_platform_spec(
+    platform_config: dict,
+    executor_label: str,
+) -> pipeline_spec_pb2.PlatformSpec:
+    """Converts a single task's pipeline_task.platform_config dictionary to a
+    PlatformSpec message using the executor_label for the task."""
+    platform_spec_msg = pipeline_spec_pb2.PlatformSpec()
+    json_format.ParseDict(
+        {
+            'platforms': {
+                platform_key: {
+                    'deployment_spec': {
+                        'executors': {
+                            executor_label: config
+                        }
+                    }
+                } for platform_key, config in platform_config.items()
+            }
+        }, platform_spec_msg)
+    return platform_spec_msg
+
+
+def merge_platform_specs(
+    main_msg: pipeline_spec_pb2.PlatformSpec,
+    sub_msg: pipeline_spec_pb2.PlatformSpec,
+) -> None:
+    """Merges a sub_msg PlatformSpec into the main_msg PlatformSpec, leaving
+    the sub_msg unchanged."""
+    for platform_key, single_platform_spec in sub_msg.platforms.items():
+        merge_platform_deployment_config(
+            main_msg.platforms[platform_key].deployment_spec,
+            single_platform_spec.deployment_spec,
+        )
+
+
+def merge_platform_deployment_config(
+    main_msg: pipeline_spec_pb2.PlatformDeploymentConfig,
+    sub_msg: pipeline_spec_pb2.PlatformDeploymentConfig,
+) -> None:
+    """Merges a sub_msg PlatformDeploymentConfig into the main_msg
+    PlatformDeploymentConfig, leaving the sub_msg unchanged."""
+    for executor_label, addtl_body in sub_msg.executors.items():
+        body = main_msg.executors.get(executor_label, struct_pb2.Struct())
+        body.update(addtl_body)
+        main_msg.executors[executor_label].CopyFrom(body)
+
+
 def build_exit_handler_groups_recursively(
     parent_group: tasks_group.TasksGroup,
     pipeline_spec: pipeline_spec_pb2.PipelineSpec,
     deployment_config: pipeline_spec_pb2.PipelineDeploymentConfig,
-):
+    platform_spec: pipeline_spec_pb2.PlatformSpec,
+) -> None:
     if not parent_group.groups:
         return
     for group in parent_group.groups:
         if isinstance(group, tasks_group.ExitHandler):
 
             # remove this if block to support nested exit handlers
             if not parent_group.is_root:
@@ -1326,21 +1399,32 @@
                 executor_label = utils.make_name_unique_by_adding_index(
                     name=exit_task_component_spec.executor_label,
                     collection=list(deployment_config.executors.keys()),
                     delimiter='-')
                 exit_task_component_spec.executor_label = executor_label
                 deployment_config.executors[executor_label].container.CopyFrom(
                     exit_task_container_spec)
+                single_task_platform_spec = platform_config_to_platform_spec(
+                    exit_task.platform_config,
+                    executor_label,
+                )
+                merge_platform_specs(
+                    platform_spec,
+                    single_task_platform_spec,
+                )
             elif exit_task.pipeline_spec is not None:
-                exit_task_pipeline_spec = merge_deployment_spec_and_component_spec(
+                exit_task_pipeline_spec, updated_platform_spec = merge_deployment_spec_and_component_spec(
                     main_pipeline_spec=pipeline_spec,
                     main_deployment_config=deployment_config,
                     sub_pipeline_spec=exit_task.pipeline_spec,
-                )
+                    main_platform_spec=platform_spec,
+                    sub_platform_spec=exit_task.platform_spec)
                 exit_task_component_spec = exit_task_pipeline_spec.root
+                # assign the new PlatformSpec data to the existing main PlatformSpec object
+                platform_spec.CopyFrom(updated_platform_spec)
             else:
                 raise RuntimeError(
                     f'Exit task {exit_task_name} is missing both container spec and pipeline spec.'
                 )
 
             # Add exit task component spec.
             component_name = utils.make_name_unique_by_adding_index(
@@ -1357,57 +1441,73 @@
 
             pipeline_spec.deployment_spec.update(
                 json_format.MessageToDict(deployment_config))
 
         build_exit_handler_groups_recursively(
             parent_group=group,
             pipeline_spec=pipeline_spec,
-            deployment_config=deployment_config)
+            deployment_config=deployment_config,
+            platform_spec=platform_spec,
+        )
 
 
 def merge_deployment_spec_and_component_spec(
     main_pipeline_spec: pipeline_spec_pb2.PipelineSpec,
     main_deployment_config: pipeline_spec_pb2.PipelineDeploymentConfig,
     sub_pipeline_spec: pipeline_spec_pb2.PipelineSpec,
-) -> pipeline_spec_pb2.PipelineSpec:
+    main_platform_spec: pipeline_spec_pb2.PlatformSpec,
+    sub_platform_spec: pipeline_spec_pb2.PlatformSpec,
+) -> Tuple[pipeline_spec_pb2.PipelineSpec, pipeline_spec_pb2.PlatformSpec]:
     """Merges deployment spec and component spec from a sub pipeline spec into
     the main spec.
 
-    We need to make sure that we keep the original sub pipeline spec
+    Also merges sub_platform_spec into main_platform_spec, with updated executor labels.
+
+    We need to make sure that we keep the original sub PipelineSpec and PlatformSpec
     unchanged--in case the pipeline is reused (instantiated) multiple times,
     the "template" should not carry any "signs of usage".
 
+
     Args:
-        main_pipeline_spec: The main pipeline spec to merge into.
-        main_deployment_config: The main deployment config to merge into.
-        sub_pipeline_spec: The pipeline spec of an inner pipeline whose
+        main_pipeline_spec: The main PipelineSpec to merge into.
+        main_deployment_config: The main PipelineDeploymentConfig to merge into.
+        sub_pipeline_spec: The PipelineSpec of an inner pipeline whose
             deployment specs and component specs need to be copied into the main
             specs.
+        main_platform_spec: The PlatformSpec corresponding to main_pipeline_spec.
+        sub_platform_spec: The PlatformSpec corresponding to sub_pipeline_spec.
 
     Returns:
-        The possibly modified copy of pipeline spec.
+        The possibly modified version of sub_pipeline_spec and the possibly modified version of the the main_platform_spec. The sub_pipeline_spec is "folded" into the outer pipeline, whereas the main_platform_spec is updated to contain the sub_pipeline_spec's configuration.
     """
-    # Make a copy of the sub_pipeline_spec so that the "template" remains
+    # Make a copy of the messages of the inner pipeline so that the "template" remains
     # unchanged and works even the pipeline is reused multiple times.
     sub_pipeline_spec_copy = pipeline_spec_pb2.PipelineSpec()
     sub_pipeline_spec_copy.CopyFrom(sub_pipeline_spec)
+    sub_platform_spec_copy = pipeline_spec_pb2.PlatformSpec()
+    sub_platform_spec_copy.CopyFrom(sub_platform_spec)
 
     _merge_deployment_spec(
         main_deployment_config=main_deployment_config,
-        sub_pipeline_spec=sub_pipeline_spec_copy)
+        sub_pipeline_spec=sub_pipeline_spec_copy,
+        main_platform_spec=main_platform_spec,
+        sub_platform_spec=sub_platform_spec_copy,
+    )
     _merge_component_spec(
         main_pipeline_spec=main_pipeline_spec,
         sub_pipeline_spec=sub_pipeline_spec_copy,
     )
-    return sub_pipeline_spec_copy
+    return sub_pipeline_spec_copy, main_platform_spec
 
 
 def _merge_deployment_spec(
     main_deployment_config: pipeline_spec_pb2.PipelineDeploymentConfig,
     sub_pipeline_spec: pipeline_spec_pb2.PipelineSpec,
+    main_platform_spec: pipeline_spec_pb2.PlatformSpec,
+    sub_platform_spec: pipeline_spec_pb2.PlatformSpec,
 ) -> None:
     """Merges deployment config from a sub pipeline spec into the main config.
 
     During the merge we need to ensure all executor specs have unique executor
     labels, that means we might need to update the `executor_label` referenced
     from component specs in sub_pipeline_spec.
 
@@ -1423,14 +1523,33 @@
         new_executor_label: str,
     ) -> None:
         """Renames the old executor_label to the new one in component spec."""
         for _, component_spec in pipeline_spec.components.items():
             if component_spec.executor_label == old_executor_label:
                 component_spec.executor_label = new_executor_label
 
+    def _rename_platform_config_executor_labels(
+        sub_platform_spec: pipeline_spec_pb2.PlatformSpec,
+        old_executor_label: str,
+        new_executor_label: str,
+    ) -> None:
+        # make a copy so that map size doesn't change during iteration
+        sub_platform_spec_copy = copy.deepcopy(sub_platform_spec)
+        for platform_key, platform_config in sub_platform_spec_copy.platforms.items(
+        ):
+            for cur_exec_label, task_config in platform_config.deployment_spec.executors.items(
+            ):
+                if cur_exec_label == old_executor_label:
+                    del sub_platform_spec.platforms[
+                        platform_key].deployment_spec.executors[
+                            old_executor_label]
+                    sub_platform_spec.platforms[
+                        platform_key].deployment_spec.executors[
+                            new_executor_label].CopyFrom(task_config)
+
     sub_deployment_config = pipeline_spec_pb2.PipelineDeploymentConfig()
     json_format.ParseDict(
         json_format.MessageToDict(sub_pipeline_spec.deployment_spec),
         sub_deployment_config)
 
     for executor_label, executor_spec in sub_deployment_config.executors.items(
     ):
@@ -1440,16 +1559,22 @@
             collection=list(main_deployment_config.executors.keys()),
             delimiter='-')
         if executor_label != old_executor_label:
             _rename_executor_labels(
                 pipeline_spec=sub_pipeline_spec,
                 old_executor_label=old_executor_label,
                 new_executor_label=executor_label)
+            _rename_platform_config_executor_labels(
+                sub_platform_spec,
+                old_executor_label=old_executor_label,
+                new_executor_label=executor_label)
 
         main_deployment_config.executors[executor_label].CopyFrom(executor_spec)
+        merge_platform_specs(
+            main_msg=main_platform_spec, sub_msg=sub_platform_spec)
 
 
 def _merge_component_spec(
     main_pipeline_spec: pipeline_spec_pb2.PipelineSpec,
     sub_pipeline_spec: pipeline_spec_pb2.PipelineSpec,
 ) -> None:
     """Merges component spec from a sub pipeline spec into the main config.
@@ -1505,15 +1630,15 @@
             old_name_to_new_name[old_component_name]].CopyFrom(component_spec)
 
 
 def create_pipeline_spec(
     pipeline: pipeline_context.Pipeline,
     component_spec: structures.ComponentSpec,
     pipeline_outputs: Optional[Any] = None,
-) -> pipeline_spec_pb2.PipelineSpec:
+) -> Tuple[pipeline_spec_pb2.PipelineSpec, pipeline_spec_pb2.PlatformSpec]:
     """Creates a pipeline spec object.
 
     Args:
         pipeline: The instantiated pipeline object.
         component_spec: The component spec structures.
         pipeline_outputs: The pipeline outputs via return.
 
@@ -1532,17 +1657,18 @@
     pipeline_spec.sdk_version = f'kfp-{kfp.__version__}'
     # Schema version 2.1.0 is required for kfp-pipeline-spec>0.1.13
     pipeline_spec.schema_version = '2.1.0'
 
     pipeline_spec.root.CopyFrom(
         _build_component_spec_from_component_spec_structure(component_spec))
 
-    _build_dag_outputs(
-        component_spec=pipeline_spec.root, dag_outputs=pipeline_outputs)
-
+    # TODO: add validation of returned outputs -- it's possible to return
+    # an output from a task in a condition group, for example, which isn't
+    # caught until submission time using Vertex SDK client
+    pipeline_outputs_dict = convert_pipeline_outputs_to_dict(pipeline_outputs)
     root_group = pipeline.groups[0]
 
     all_groups = compiler_utils.get_all_groups(root_group)
     group_name_to_group = {group.name: group for group in all_groups}
     task_name_to_parent_groups, group_name_to_parent_groups = (
         compiler_utils.get_parent_groups(root_group))
     condition_channels = compiler_utils.get_condition_channels_for_tasks(
@@ -1555,88 +1681,146 @@
     inputs = compiler_utils.get_inputs_for_all_groups(
         pipeline=pipeline,
         task_name_to_parent_groups=task_name_to_parent_groups,
         group_name_to_parent_groups=group_name_to_parent_groups,
         condition_channels=condition_channels,
         name_to_for_loop_group=name_to_for_loop_group,
     )
+    outputs, modified_pipeline_outputs_dict = compiler_utils.get_outputs_for_all_groups(
+        pipeline=pipeline,
+        task_name_to_parent_groups=task_name_to_parent_groups,
+        group_name_to_parent_groups=group_name_to_parent_groups,
+        all_groups=all_groups,
+        pipeline_outputs_dict=pipeline_outputs_dict)
     dependencies = compiler_utils.get_dependencies(
         pipeline=pipeline,
         task_name_to_parent_groups=task_name_to_parent_groups,
         group_name_to_parent_groups=group_name_to_parent_groups,
         group_name_to_group=group_name_to_group,
         condition_channels=condition_channels,
     )
 
+    platform_spec = pipeline_spec_pb2.PlatformSpec()
     for group in all_groups:
         build_spec_by_group(
             pipeline_spec=pipeline_spec,
             deployment_config=deployment_config,
             group=group,
             inputs=inputs,
+            outputs=outputs,
             dependencies=dependencies,
             rootgroup_name=root_group.name,
             task_name_to_parent_groups=task_name_to_parent_groups,
             group_name_to_parent_groups=group_name_to_parent_groups,
             name_to_for_loop_group=name_to_for_loop_group,
+            platform_spec=platform_spec,
+            is_compiled_component=False,
         )
 
     build_exit_handler_groups_recursively(
         parent_group=root_group,
         pipeline_spec=pipeline_spec,
         deployment_config=deployment_config,
+        platform_spec=platform_spec,
     )
 
-    return pipeline_spec
+    _build_dag_outputs(
+        component_spec=pipeline_spec.root,
+        dag_outputs=modified_pipeline_outputs_dict,
+    )
+    # call _build_dag_outputs first to verify the presence of an output annotation
+    # at all, then validate that the annotation is correct with _validate_dag_output_types
+    _validate_dag_output_types(
+        dag_outputs=modified_pipeline_outputs_dict,
+        structures_component_spec=component_spec)
+
+    return pipeline_spec, platform_spec
+
+
+def _validate_dag_output_types(
+        dag_outputs: Dict[str, pipeline_channel.PipelineChannel],
+        structures_component_spec: structures.ComponentSpec) -> None:
+    for output_name, output_channel in dag_outputs.items():
+        output_spec = structures_component_spec.outputs[output_name]
+        output_name = '' if len(dag_outputs) == 1 else f'{output_name!r} '
+        error_message_prefix = f'Incompatible return type provided for output {output_name}of pipeline {structures_component_spec.name!r}. '
+        type_utils.verify_type_compatibility(
+            output_channel,
+            output_spec,
+            error_message_prefix,
+            checks_input=False,
+        )
 
 
-def write_pipeline_spec_to_file(pipeline_spec: pipeline_spec_pb2.PipelineSpec,
-                                pipeline_description: str,
-                                package_path: str) -> None:
+def convert_pipeline_outputs_to_dict(
+    pipeline_outputs: Union[pipeline_channel.PipelineChannel, typing.NamedTuple,
+                            None]
+) -> Dict[str, pipeline_channel.PipelineChannel]:
+    """Converts the outputs from a pipeline function into a dictionary of
+    output name to PipelineChannel."""
+    if pipeline_outputs is None:
+        return {}
+    elif isinstance(pipeline_outputs, pipeline_channel.PipelineChannel):
+        return {_SINGLE_OUTPUT_NAME: pipeline_outputs}
+    elif isinstance(pipeline_outputs, tuple) and hasattr(
+            pipeline_outputs, '_asdict'):
+        return dict(pipeline_outputs._asdict())
+    else:
+        raise ValueError(f'Got unknown pipeline output: {pipeline_outputs}')
+
+
+def write_pipeline_spec_to_file(
+    pipeline_spec: pipeline_spec_pb2.PipelineSpec,
+    pipeline_description: str,
+    platform_spec: pipeline_spec_pb2.PlatformSpec,
+    package_path: str,
+) -> None:
     """Writes PipelineSpec into a YAML or JSON (deprecated) file.
 
     Args:
-        pipeline_spec (pipeline_spec_pb2.PipelineSpec): The PipelineSpec.
-        package_path (str): The path to which to write the PipelineSpec.
+        pipeline_spec: The PipelineSpec.
+        pipeline_description: Description from pipeline docstring.
+        package_path: The path to which to write the PipelineSpec.
+        platform_spec: The PlatformSpec.
     """
-    json_dict = json_format.MessageToDict(pipeline_spec)
-    yaml_comments = extract_comments_from_pipeline_spec(json_dict,
+    pipeline_spec_dict = json_format.MessageToDict(pipeline_spec)
+    yaml_comments = extract_comments_from_pipeline_spec(pipeline_spec_dict,
                                                         pipeline_description)
+    has_platform_specific_features = len(platform_spec.platforms) > 0
 
     if package_path.endswith('.json'):
         warnings.warn(
             ('Compiling to JSON is deprecated and will be '
              'removed in a future version. Please compile to a YAML file by '
              'providing a file path with a .yaml extension instead.'),
             category=DeprecationWarning,
             stacklevel=2,
         )
         with open(package_path, 'w') as json_file:
-            json.dump(json_dict, json_file, indent=2, sort_keys=True)
+            if has_platform_specific_features:
+                raise ValueError(
+                    f'Platform-specific features are only supported when serializing to YAML. Argument for {"package_path"!r} has file extension {".json"!r}.'
+                )
+            json.dump(pipeline_spec_dict, json_file, indent=2, sort_keys=True)
 
     elif package_path.endswith(('.yaml', '.yml')):
         with open(package_path, 'w') as yaml_file:
             yaml_file.write(yaml_comments)
-            yaml.dump(json_dict, yaml_file, sort_keys=True)
+            documents = [pipeline_spec_dict]
+            if has_platform_specific_features:
+                documents.append(json_format.MessageToDict(platform_spec))
+            yaml.dump_all(documents, yaml_file, sort_keys=True)
 
     else:
         raise ValueError(
             f'The output path {package_path} should end with ".yaml".')
 
 
 def extract_comments_from_pipeline_spec(pipeline_spec: dict,
                                         pipeline_description: str) -> str:
-    map_parameter_types = {
-        'NUMBER_INTEGER': int.__name__,
-        'NUMBER_DOUBLE': float.__name__,
-        'STRING': str.__name__,
-        'BOOLEAN': bool.__name__,
-        'LIST': list.__name__,
-        'STRUCT': dict.__name__
-    }
 
     map_headings = {
         'inputDefinitions': '# Inputs:',
         'outputDefinitions': '# Outputs:'
     }
 
     def collect_pipeline_signatures(root_dict: dict,
@@ -1648,16 +1832,17 @@
 
             # Collect data
             array_of_signatures = []
             for parameter_name, parameter_body in signature.get(
                     'parameters', {}).items():
                 data = {}
                 data['name'] = parameter_name
-                data['parameterType'] = map_parameter_types[
-                    parameter_body['parameterType']]
+                data[
+                    'parameterType'] = type_utils.IR_TYPE_TO_COMMENT_TYPE_STRING[
+                        parameter_body['parameterType']]
                 if 'defaultValue' in signature['parameters'][parameter_name]:
                     data['defaultValue'] = signature['parameters'][
                         parameter_name]['defaultValue']
                     if isinstance(data['defaultValue'], str):
                         data['defaultValue'] = "'" + data['defaultValue'] + "'"
                 array_of_signatures.append(data)
```

### Comparing `kfp-2.0.0b9/kfp/compiler/read_write_test.py` & `kfp-2.0.0rc1/kfp/compiler/read_write_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/__init__.py` & `kfp-2.0.0rc1/kfp/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/base_component.py` & `kfp-2.0.0rc1/kfp/components/base_component.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Base class for KFP components."""
 
 import abc
+from typing import List
 
 from kfp.components import pipeline_task
 from kfp.components import structures
 from kfp.components.types import type_utils
 from kfp.pipeline_spec import pipeline_spec_pb2
 
 
@@ -46,14 +47,26 @@
         # (backend) system to pass a value.
         self._component_inputs = {
             input_name for input_name, input_spec in (
                 self.component_spec.inputs or {}).items()
             if not type_utils.is_task_final_status_type(input_spec.type)
         }
 
+    def _prevent_using_output_lists_of_artifacts(self):
+        """This method should be called at the end of __init__ for
+        PythonComponent and ContainerComponent subclasses to temporarily block
+        outputting lists of artifacts from a component."""
+        # TODO: remove when output lists of artifacts from primitive components is supported
+        for output_name, output_spec in (self.component_spec.outputs or
+                                         {}).items():
+            if output_spec.is_artifact_list:
+                raise ValueError(
+                    f'Output lists of artifacts are only supported for pipelines. Got output list of artifacts for output parameter {output_name!r} of component {self.name!r}.'
+                )
+
     def __call__(self, *args, **kwargs) -> pipeline_task.PipelineTask:
         """Creates a PipelineTask object.
 
         The arguments are generated on the fly based on component input
         definitions.
         """
         task_inputs = {}
@@ -68,23 +81,21 @@
             if k not in self._component_inputs:
                 raise TypeError(
                     f'{self.name}() got an unexpected keyword argument "{k}".')
             task_inputs[k] = v
 
         # Skip optional inputs and arguments typed as PipelineTaskFinalStatus.
         missing_arguments = [
-            input_name for input_name, input_spec in (
-                self.component_spec.inputs or {}).items()
-            if input_name not in task_inputs and not input_spec.optional and
-            not type_utils.is_task_final_status_type(input_spec.type)
+            arg for arg in self.required_inputs if arg not in kwargs
         ]
         if missing_arguments:
             argument_or_arguments = 'argument' if len(
                 missing_arguments) == 1 else 'arguments'
-            arguments = ', '.join(missing_arguments)
+            arguments = ', '.join(
+                arg_name.replace('-', '_') for arg_name in missing_arguments)
 
             raise TypeError(
                 f'{self.name}() missing {len(missing_arguments)} required '
                 f'{argument_or_arguments}: {arguments}.')
 
         return pipeline_task.PipelineTask(
             component_spec=self.component_spec,
@@ -93,19 +104,36 @@
 
     @property
     def pipeline_spec(self) -> pipeline_spec_pb2.PipelineSpec:
         """Returns the pipeline spec of the component."""
         with BlockPipelineTaskRegistration():
             return self.component_spec.to_pipeline_spec()
 
+    @property
+    def platform_spec(self) -> pipeline_spec_pb2.PlatformSpec:
+        """Returns the PlatformSpec of the component.
+
+        Useful when the component is a GraphComponent, else will be
+        empty per component_spec.platform_spec default.
+        """
+        return self.component_spec.platform_spec
+
     @abc.abstractmethod
     def execute(self, **kwargs):
         """Executes the component locally if implemented by the inheriting
         subclass."""
 
+    @property
+    def required_inputs(self) -> List[str]:
+        return [
+            input_name for input_name, input_spec in (
+                self.component_spec.inputs or {}).items()
+            if not input_spec.optional
+        ]
+
 
 class BlockPipelineTaskRegistration:
     """Temporarily stop registering tasks to the default pipeline.
 
     Handles special, uncommon functions that decorate and mutate a
     component, possibly by using the component's .pipeline_spec
     attribute. This is exhibited in the version of
```

### Comparing `kfp-2.0.0b9/kfp/components/base_component_test.py` & `kfp-2.0.0rc1/kfp/components/base_component_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,27 +13,22 @@
 # limitations under the License.
 """Tests for kfp.components.base_component."""
 
 import unittest
 from unittest.mock import patch
 
 from kfp import dsl
-from kfp.components import base_component
 from kfp.components import pipeline_task
 from kfp.components import placeholders
+from kfp.components import PythonComponent
 from kfp.components import structures
 
-
-class TestComponent(base_component.BaseComponent):
-
-    def execute(self, *args, **kwargs):
-        pass
-
-
-component_op = TestComponent(
+component_op = PythonComponent(
+    # dummy python_func not used in behavior that is being tested
+    python_func=lambda: None,
     component_spec=structures.ComponentSpec(
         name='component_1',
         implementation=structures.Implementation(
             container=structures.ContainerSpecImplementation(
                 image='alpine',
                 command=[
                     'sh',
```

### Comparing `kfp-2.0.0b9/kfp/components/component_decorator.py` & `kfp-2.0.0rc1/kfp/components/component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/component_decorator_test.py` & `kfp-2.0.0rc1/kfp/components/component_decorator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,15 @@
                     return text
 
             self.assertIsInstance(comp, python_component.PythonComponent)
             self.assertTrue(os.path.exists(filepath))
             with open(filepath, 'r') as f:
                 yaml_text = f.read()
 
-        component_spec = structures.ComponentSpec.load_from_component_yaml(
-            yaml_text)
+        component_spec = structures.ComponentSpec.from_yaml_documents(yaml_text)
         self.assertEqual(component_spec.name, comp.component_spec.name)
 
     def test_output_named_tuple_with_dict(self):
 
         @component
         def comp(
                 text: str) -> NamedTuple('outputs', [('data', Dict[str, str])]):
```

### Comparing `kfp-2.0.0b9/kfp/components/component_factory.py` & `kfp-2.0.0rc1/kfp/components/component_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 # limitations under the License.
 import dataclasses
 import inspect
 import itertools
 import pathlib
 import re
 import textwrap
-from typing import Callable, List, Optional, Tuple
+from typing import Callable, List, Mapping, Optional, Tuple, Type, Union
 import warnings
 
 import docstring_parser
 from kfp.components import container_component
+from kfp.components import container_component_artifact_channel
 from kfp.components import graph_component
 from kfp.components import placeholders
 from kfp.components import python_component
 from kfp.components import structures
-from kfp.components.container_component_artifact_channel import \
-    ContainerComponentArtifactChannel
+from kfp.components import task_final_status
+from kfp.components.types import artifact_types
 from kfp.components.types import custom_artifact_types
 from kfp.components.types import type_annotations
 from kfp.components.types import type_utils
 
 _DEFAULT_BASE_IMAGE = 'python:3.7'
 
 
@@ -46,40 +47,59 @@
     func: Callable
     target_image: str
     module_path: pathlib.Path
     component_spec: structures.ComponentSpec
     output_component_file: Optional[str] = None
     base_image: str = _DEFAULT_BASE_IMAGE
     packages_to_install: Optional[List[str]] = None
+    pip_index_urls: Optional[List[str]] = None
 
 
 # A map from function_name to components.  This is always populated when a
 # module containing KFP components is loaded. Primarily used by KFP CLI
 # component builder to package components in a file into containers.
 REGISTERED_MODULES = None
 
 
 def _python_function_name_to_component_name(name):
     name_with_spaces = re.sub(' +', ' ', name.replace('_', ' ')).strip(' ')
     return name_with_spaces[0].upper() + name_with_spaces[1:]
 
 
-def _make_index_url_options(pip_index_urls: Optional[List[str]]) -> str:
+def make_index_url_options(pip_index_urls: Optional[List[str]]) -> str:
+    """Generates index url options for pip install command based on provided
+    pip_index_urls.
+
+    Args:
+        pip_index_urls: Optional list of pip index urls
+
+    Returns:
+        - Empty string if pip_index_urls is empty/None.
+        - '--index-url url --trusted-host url ' if pip_index_urls contains 1
+        url
+        - the above followed by '--extra-index-url url --trusted-host url '
+        for
+        each next url in pip_index_urls if pip_index_urls contains more than 1
+        url
+
+        Note: In case pip_index_urls is not empty, the returned string will
+        contain space at the end.
+    """
     if not pip_index_urls:
         return ''
 
     index_url = pip_index_urls[0]
     extra_index_urls = pip_index_urls[1:]
 
-    options = [f'--index-url {index_url} --trusted-host {index_url} ']
+    options = [f'--index-url {index_url} --trusted-host {index_url}']
     options.extend(
-        f'--extra-index-url {extra_index_url} --trusted-host {extra_index_url} '
+        f'--extra-index-url {extra_index_url} --trusted-host {extra_index_url}'
         for extra_index_url in extra_index_urls)
 
-    return ' '.join(options)
+    return ' '.join(options) + ' '
 
 
 _install_python_packages_script_template = '''
 if ! [ -x "$(command -v pip)" ]; then
     python3 -m ensurepip || python3 -m ensurepip --user || apt-get install python3-pip
 fi
 
@@ -93,15 +113,15 @@
         pip_index_urls: Optional[List[str]] = None) -> List[str]:
 
     if not package_list:
         return []
 
     concat_package_list = ' '.join(
         [repr(str(package)) for package in package_list])
-    index_url_options = _make_index_url_options(pip_index_urls)
+    index_url_options = make_index_url_options(pip_index_urls)
     install_python_packages_script = _install_python_packages_script_template.format(
         index_url_options=index_url_options,
         concat_package_list=concat_package_list)
     return ['sh', '-c', install_python_packages_script]
 
 
 def _get_default_kfp_package_path() -> str:
@@ -140,33 +160,38 @@
         if unique_name not in names:
             return unique_name
 
     raise RuntimeError(f'Too many arguments with the name {name}')
 
 
 def extract_component_interface(
-        func: Callable,
-        containerized: bool = False) -> structures.ComponentSpec:
+    func: Callable,
+    containerized: bool = False,
+    description: Optional[str] = None,
+    name: Optional[str] = None,
+) -> structures.ComponentSpec:
     single_output_name_const = 'Output'
 
     signature = inspect.signature(func)
     parameters = list(signature.parameters.values())
 
-    parsed_docstring = docstring_parser.parse(inspect.getdoc(func))
+    original_docstring = inspect.getdoc(func)
+    parsed_docstring = docstring_parser.parse(original_docstring)
 
     inputs = {}
     outputs = {}
 
     input_names = set()
     output_names = set()
     for parameter in parameters:
         parameter_type = type_annotations.maybe_strip_optional_from_annotation(
             parameter.annotation)
         passing_style = None
         io_name = parameter.name
+        is_artifact_list = False
 
         if type_annotations.is_Input_Output_artifact_annotation(parameter_type):
             # passing_style is either type_annotations.InputAnnotation or
             # type_annotations.OutputAnnotation.
             passing_style = type_annotations.get_io_artifact_annotation(
                 parameter_type)
 
@@ -179,17 +204,26 @@
                 parameter_type)
             if not type_annotations.is_artifact_class(parameter_type):
                 raise ValueError(
                     f'Input[T] and Output[T] are only supported when T is an artifact or list of artifacts. Found `{io_name} with type {parameter_type}`'
                 )
 
             if parameter.default is not inspect.Parameter.empty:
-                raise ValueError(
-                    'Default values for Input/Output artifacts are not supported.'
-                )
+                if passing_style in [
+                        type_annotations.OutputAnnotation,
+                        type_annotations.OutputPath,
+                ]:
+                    raise ValueError(
+                        'Default values for Output artifacts are not supported.'
+                    )
+                elif parameter.default is not None:
+                    raise ValueError(
+                        f'Optional Input artifacts may only have default value None. Got: {parameter.default}.'
+                    )
+
         elif isinstance(
                 parameter_type,
             (type_annotations.InputPath, type_annotations.OutputPath)):
             passing_style = type(parameter_type)
             parameter_type = parameter_type.type
             if parameter.default is not inspect.Parameter.empty and not (
                     passing_style == type_annotations.InputPath and
@@ -220,29 +254,28 @@
                     is_artifact_list=is_artifact_list)
             else:
                 output_spec = structures.OutputSpec(type=type_struct)
             outputs[io_name] = output_spec
         else:
             io_name = _maybe_make_unique(io_name, input_names)
             input_names.add(io_name)
-            if type_annotations.is_artifact_class(parameter_type):
-                schema_version = parameter_type.schema_version
-                input_spec = structures.InputSpec(
-                    type=type_utils.create_bundled_artifact_type(
-                        type_struct, schema_version),
-                    is_artifact_list=is_artifact_list,
-                )
-            else:
-                if parameter.default is not inspect.Parameter.empty:
-                    input_spec = structures.InputSpec(
-                        type=type_struct,
-                        default=parameter.default,
-                        optional=True)
-                else:
-                    input_spec = structures.InputSpec(type=type_struct,)
+            type_ = type_utils.create_bundled_artifact_type(
+                type_struct, parameter_type.schema_version
+            ) if type_annotations.is_artifact_class(
+                parameter_type) else type_struct
+            default = None if parameter.default == inspect.Parameter.empty or type_annotations.is_artifact_class(
+                parameter_type) else parameter.default
+            optional = parameter.default is not inspect.Parameter.empty or type_utils.is_task_final_status_type(
+                type_struct)
+            input_spec = structures.InputSpec(
+                type=type_,
+                default=default,
+                optional=optional,
+                is_artifact_list=is_artifact_list,
+            )
 
             inputs[io_name] = input_spec
 
     #Analyzing the return type annotations.
     return_ann = signature.return_annotation
     if not containerized:
         if hasattr(return_ann, '_fields'):  #NamedTuple
@@ -253,17 +286,20 @@
                                         None) or getattr(
                                             return_ann, '_field_types', None)
             for field_name in return_ann._fields:
                 output_name = _maybe_make_unique(field_name, output_names)
                 output_names.add(output_name)
                 type_var = field_annotations.get(field_name)
                 if type_annotations.is_list_of_artifacts(type_var):
-                    raise ValueError(
-                        f'Cannot use output lists of artifacts in NamedTuple return annotations. Got output list of artifacts annotation for NamedTuple field `{field_name}`.'
-                    )
+                    artifact_cls = type_var.__args__[0]
+                    output_spec = structures.OutputSpec(
+                        type=type_utils.create_bundled_artifact_type(
+                            artifact_cls.schema_title,
+                            artifact_cls.schema_version),
+                        is_artifact_list=True)
                 elif type_annotations.is_artifact_class(type_var):
                     output_spec = structures.OutputSpec(
                         type=type_utils.create_bundled_artifact_type(
                             type_var.schema_title, type_var.schema_version))
                 else:
                     type_struct = type_utils._annotation_to_type_struct(
                         type_var)
@@ -306,41 +342,66 @@
 
             outputs[output_name] = output_spec
     elif return_ann != inspect.Parameter.empty and return_ann != structures.ContainerSpec:
         raise TypeError(
             'Return annotation should be either ContainerSpec or omitted for container components.'
         )
 
-    # Component name and description are derived from the function's name and
-    # docstring.  The name can be overridden by setting setting func.__name__
-    # attribute (of the legacy func._component_human_name attribute).  The
-    # description can be overridden by setting the func.__doc__ attribute (or
-    # the legacy func._component_description attribute).
-    component_name = getattr(
-        func, '_component_human_name',
-        _python_function_name_to_component_name(func.__name__))
-
-    short_description = parsed_docstring.short_description
-    long_description = parsed_docstring.long_description
-    docstring_description = short_description + '\n' + long_description if long_description else short_description
-
-    description = getattr(func, '_component_description', docstring_description)
+    component_name = name or _python_function_name_to_component_name(
+        func.__name__)
 
-    if description:
-        description = description.strip()
+    def assign_descriptions(
+        inputs_or_outputs: Mapping[str, Union[structures.InputSpec,
+                                              structures.OutputSpec]],
+        docstring_params: List[docstring_parser.DocstringParam],
+    ) -> None:
+        """Assigns descriptions to InputSpec or OutputSpec for each component
+        input/output found in the parsed docstring parameters."""
+        docstring_inputs = {param.arg_name: param for param in docstring_params}
+        for name, spec in inputs_or_outputs.items():
+            if name in docstring_inputs:
+                spec.description = docstring_inputs[name].description
+
+    def parse_docstring_with_return_as_args(
+            docstring: Union[str,
+                             None]) -> Union[docstring_parser.Docstring, None]:
+        """Modifies docstring so that a return section can be treated as an
+        args section, then parses the docstring."""
+        if docstring is None:
+            return None
+
+        # Returns and Return are the only two keywords docstring_parser uses for returns
+        # use newline to avoid replacements that aren't in the return section header
+        return_keywords = ['Returns:\n', 'Returns\n', 'Return:\n', 'Return\n']
+        for keyword in return_keywords:
+            if keyword in docstring:
+                modified_docstring = docstring.replace(keyword.strip(), 'Args:')
+                return docstring_parser.parse(modified_docstring)
+
+        return None
+
+    assign_descriptions(inputs, parsed_docstring.params)
+
+    modified_parsed_docstring = parse_docstring_with_return_as_args(
+        original_docstring)
+    if modified_parsed_docstring is not None:
+        assign_descriptions(outputs, modified_parsed_docstring.params)
+
+    description = get_pipeline_description(
+        decorator_description=description,
+        docstring=parsed_docstring,
+    )
 
-    component_spec = structures.ComponentSpec(
+    return structures.ComponentSpec(
         name=component_name,
         description=description,
-        inputs=inputs if inputs else None,
-        outputs=outputs if outputs else None,
-        # Dummy implementation to bypass model validation.
+        inputs=inputs or None,
+        outputs=outputs or None,
         implementation=structures.Implementation(),
     )
-    return component_spec
 
 
 def _get_command_and_args_for_lightweight_component(
         func: Callable) -> Tuple[List[str], List[str]]:
     imports_source = [
         'import kfp',
         'from kfp import dsl',
@@ -452,77 +513,127 @@
         function_name=func.__name__,
         func=func,
         target_image=target_image,
         module_path=module_path,
         component_spec=component_spec,
         output_component_file=output_component_file,
         base_image=base_image,
-        packages_to_install=packages_to_install)
+        packages_to_install=packages_to_install,
+        pip_index_urls=pip_index_urls)
 
     if REGISTERED_MODULES is not None:
         REGISTERED_MODULES[component_name] = component_info
 
     if output_component_file:
         component_spec.save_to_component_yaml(output_component_file)
 
     return python_component.PythonComponent(
         component_spec=component_spec, python_func=func)
 
 
+def make_input_for_parameterized_container_component_function(
+    name: str, annotation: Union[Type[List[artifact_types.Artifact]],
+                                 Type[artifact_types.Artifact]]
+) -> Union[placeholders.Placeholder, container_component_artifact_channel
+           .ContainerComponentArtifactChannel]:
+    if type_annotations.is_input_artifact(annotation):
+
+        if type_annotations.is_list_of_artifacts(annotation.__origin__):
+            return placeholders.InputListOfArtifactsPlaceholder(name)
+        else:
+            return container_component_artifact_channel.ContainerComponentArtifactChannel(
+                io_type='input', var_name=name)
+
+    elif type_annotations.is_output_artifact(annotation):
+
+        if type_annotations.is_list_of_artifacts(annotation.__origin__):
+            return placeholders.OutputListOfArtifactsPlaceholder(name)
+        else:
+            return container_component_artifact_channel.ContainerComponentArtifactChannel(
+                io_type='output', var_name=name)
+
+    elif isinstance(
+            annotation,
+        (type_annotations.OutputAnnotation, type_annotations.OutputPath)):
+        return placeholders.OutputParameterPlaceholder(name)
+
+    else:
+        placeholder = placeholders.InputValuePlaceholder(name)
+        # small hack to encode the runtime value's type for a custom json.dumps function
+        if (annotation == task_final_status.PipelineTaskFinalStatus or
+                type_utils.is_task_final_status_type(annotation)):
+            placeholder._ir_type = 'STRUCT'
+        else:
+            placeholder._ir_type = type_utils.get_parameter_type_name(
+                annotation)
+        return placeholder
+
+
 def create_container_component_from_func(
         func: Callable) -> container_component.ContainerComponent:
     """Implementation for the @container_component decorator.
 
     The decorator is defined under container_component_decorator.py. See
     the decorator for the canonical documentation for this function.
     """
 
     component_spec = extract_component_interface(func, containerized=True)
-    arg_list = []
     signature = inspect.signature(func)
     parameters = list(signature.parameters.values())
+    arg_list = []
     for parameter in parameters:
         parameter_type = type_annotations.maybe_strip_optional_from_annotation(
             parameter.annotation)
-        io_name = parameter.name
-        if type_annotations.is_input_artifact(parameter_type):
-            arg_list.append(
-                ContainerComponentArtifactChannel(
-                    io_type='input', var_name=io_name))
-        elif type_annotations.is_output_artifact(parameter_type):
-            arg_list.append(
-                ContainerComponentArtifactChannel(
-                    io_type='output', var_name=io_name))
-        elif isinstance(
-                parameter_type,
-            (type_annotations.OutputAnnotation, type_annotations.OutputPath)):
-            arg_list.append(placeholders.OutputParameterPlaceholder(io_name))
-        else:  # parameter is an input value
-            arg_list.append(placeholders.InputValuePlaceholder(io_name))
+        arg_list.append(
+            make_input_for_parameterized_container_component_function(
+                parameter.name, parameter_type))
 
     container_spec = func(*arg_list)
     container_spec_implementation = structures.ContainerSpecImplementation.from_container_spec(
         container_spec)
     component_spec.implementation = structures.Implementation(
         container_spec_implementation)
     component_spec._validate_placeholders()
     return container_component.ContainerComponent(component_spec, func)
 
 
 def create_graph_component_from_func(
-        func: Callable) -> graph_component.GraphComponent:
+    func: Callable,
+    name: Optional[str] = None,
+    description: Optional[str] = None,
+    display_name: Optional[str] = None,
+) -> graph_component.GraphComponent:
     """Implementation for the @pipeline decorator.
 
     The decorator is defined under pipeline_context.py. See the
     decorator for the canonical documentation for this function.
     """
 
-    component_spec = extract_component_interface(func)
-    component_name = getattr(
-        func, '_component_human_name',
-        _python_function_name_to_component_name(func.__name__))
-
+    component_spec = extract_component_interface(
+        func,
+        description=description,
+        name=name,
+    )
     return graph_component.GraphComponent(
         component_spec=component_spec,
         pipeline_func=func,
-        name=component_name,
+        display_name=display_name,
     )
+
+
+def get_pipeline_description(
+    decorator_description: Union[str, None],
+    docstring: docstring_parser.Docstring,
+) -> Union[str, None]:
+    """Obtains the correct pipeline description from the pipeline decorator's
+    description argument and the parsed docstring.
+
+    Gives precedence to the decorator argument.
+    """
+    if decorator_description:
+        return decorator_description
+
+    short_description = docstring.short_description
+    long_description = docstring.long_description
+    docstring_description = short_description + '\n' + long_description if (
+        short_description and long_description) else short_description
+    return docstring_description.strip() if docstring_description else None
```

### Comparing `kfp-2.0.0b9/kfp/components/component_factory_test.py` & `kfp-2.0.0rc1/kfp/components/component_factory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,19 @@
 from typing import List
 import unittest
 
 from kfp import dsl
 from kfp.components import component_factory
 from kfp.components import structures
 from kfp.components.component_decorator import component
+from kfp.components.types.artifact_types import Artifact
+from kfp.components.types.artifact_types import Model
 from kfp.components.types.type_annotations import OutputPath
+from kfp.dsl import Input
+from kfp.dsl import Output
 
 
 class TestGetPackagesToInstallCommand(unittest.TestCase):
 
     def test_with_no_packages_to_install(self):
         packages_to_install = []
 
@@ -68,20 +72,14 @@
                                     r'"Output" is an invalid parameter name.'):
 
             @component
             def comp(Output: OutputPath(str), text: str) -> str:
                 pass
 
 
-from kfp.components.types.artifact_types import Artifact
-from kfp.components.types.artifact_types import Model
-from kfp.dsl import Input
-from kfp.dsl import Output
-
-
 class TestExtractComponentInterfaceListofArtifacts(unittest.TestCase):
 
     def test_python_component_input(self):
 
         def comp(i: Input[List[Model]]):
             ...
 
@@ -128,54 +126,68 @@
                 'i':
                     structures.InputSpec(
                         type='system.Model@0.0.1',
                         default=None,
                         is_artifact_list=True)
             })
 
-    def test_pipeline_with_named_tuple_fn(self):
-        from typing import NamedTuple
 
+class TestArtifactStringInInputpathOutputpath(unittest.TestCase):
+
+    def test_unknown(self):
+
+        @dsl.component
         def comp(
-            i: Input[List[Model]]
-        ) -> NamedTuple('outputs', [('output_list', List[Artifact])]):
+                i: dsl.InputPath('MyCustomType'),
+                o: dsl.OutputPath('MyCustomType'),
+        ):
             ...
 
-        with self.assertRaisesRegex(
-                ValueError,
-                r'Cannot use output lists of artifacts in NamedTuple return annotations. Got output list of artifacts annotation for NamedTuple field `output_list`\.'
+        self.assertEqual(comp.component_spec.outputs['o'].type,
+                         'system.Artifact@0.0.1')
+        self.assertFalse(comp.component_spec.outputs['o'].is_artifact_list)
+        self.assertEqual(comp.component_spec.inputs['i'].type,
+                         'system.Artifact@0.0.1')
+        self.assertFalse(comp.component_spec.inputs['i'].is_artifact_list)
+
+    def test_known_v1_back_compat(self):
+
+        @dsl.component
+        def comp(
+                i: dsl.InputPath('Dataset'),
+                o: dsl.OutputPath('Dataset'),
         ):
-            component_factory.extract_component_interface(comp)
+            ...
+
+        self.assertEqual(comp.component_spec.outputs['o'].type,
+                         'system.Dataset@0.0.1')
+        self.assertFalse(comp.component_spec.outputs['o'].is_artifact_list)
+        self.assertEqual(comp.component_spec.inputs['i'].type,
+                         'system.Dataset@0.0.1')
+        self.assertFalse(comp.component_spec.inputs['i'].is_artifact_list)
 
 
 class TestOutputListsOfArtifactsTemporarilyBlocked(unittest.TestCase):
 
     def test_python_component(self):
         with self.assertRaisesRegex(
-                NotImplementedError,
-                r'Output lists of artifacts are not yet supported\.'):
+                ValueError,
+                r"Output lists of artifacts are only supported for pipelines\. Got output list of artifacts for output parameter 'output_list' of component 'comp'\."
+        ):
 
             @dsl.component
             def comp(output_list: Output[List[Artifact]]):
                 ...
 
     def test_container_component(self):
         with self.assertRaisesRegex(
-                NotImplementedError,
-                r'Output lists of artifacts are not yet supported\.'):
+                ValueError,
+                r"Output lists of artifacts are only supported for pipelines\. Got output list of artifacts for output parameter 'output_list' of component 'comp'\."
+        ):
 
             @dsl.container_component
             def comp(output_list: Output[List[Artifact]]):
                 return dsl.ContainerSpec(image='alpine')
 
-    def test_pipeline(self):
-        with self.assertRaisesRegex(
-                NotImplementedError,
-                r'Output lists of artifacts are not yet supported\.'):
-
-            @dsl.pipeline
-            def comp() -> List[Artifact]:
-                ...
-
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-2.0.0b9/kfp/components/constants.py` & `kfp-2.0.0rc1/kfp/components/constants.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/container_component.py` & `kfp-2.0.0rc1/kfp/components/container_component.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,12 +27,14 @@
     """
 
     def __init__(self, component_spec: structures.ComponentSpec,
                  pipeline_func: Callable) -> None:
         super().__init__(component_spec=component_spec)
         self.pipeline_func = pipeline_func
 
+        self._prevent_using_output_lists_of_artifacts()
+
     def execute(self, **kwargs):
         # ContainerComponent`: Also inherits from `BaseComponent`.
         # As its name suggests, this class backs (custom) container components.
         # Its `execute()` method uses `docker run` for local component execution
         raise NotImplementedError
```

### Comparing `kfp-2.0.0b9/kfp/components/container_component_artifact_channel.py` & `kfp-2.0.0rc1/kfp/components/container_component_artifact_channel.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/container_component_artifact_channel_test.py` & `kfp-2.0.0rc1/kfp/components/container_component_artifact_channel_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import unittest
 
-from kfp.components import component_factory
+from kfp.components import container_component_artifact_channel
 from kfp.components import placeholders
 
 
 class TestContainerComponentArtifactChannel(unittest.TestCase):
 
     def test_correct_placeholder_and_attribute_error(self):
-        in_channel = component_factory.ContainerComponentArtifactChannel(
+        in_channel = container_component_artifact_channel.ContainerComponentArtifactChannel(
             'input', 'my_dataset')
-        out_channel = component_factory.ContainerComponentArtifactChannel(
+        out_channel = container_component_artifact_channel.ContainerComponentArtifactChannel(
             'output', 'my_result')
         self.assertEqual(
             in_channel.uri._to_string(),
             placeholders.InputUriPlaceholder('my_dataset')._to_string())
         self.assertEqual(
             out_channel.path._to_string(),
             placeholders.OutputPathPlaceholder('my_result')._to_string())
```

### Comparing `kfp-2.0.0b9/kfp/components/container_component_decorator.py` & `kfp-2.0.0rc1/kfp/components/container_component_decorator.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/executor.py` & `kfp-2.0.0rc1/kfp/components/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import inspect
 import json
 import os
 from typing import Any, Callable, Dict, List, Optional, Union
 
+from kfp.components import python_component
 from kfp.components import task_final_status
 from kfp.components.types import artifact_types
 from kfp.components.types import type_annotations
 
 
 class Executor():
     """Executor executes v2-based Python function components."""
 
-    def __init__(self, executor_input: Dict, function_to_execute: Callable):
-        self._func = function_to_execute
+    def __init__(self, executor_input: Dict,
+                 function_to_execute: Union[Callable,
+                                            python_component.PythonComponent]):
+        if hasattr(function_to_execute, 'python_func'):
+            self._func = function_to_execute.python_func
+        else:
+            self._func = function_to_execute
 
         self._input = executor_input
         self._input_artifacts: Dict[str,
                                     Union[artifact_types.Artifact,
                                           List[artifact_types.Artifact]]] = {}
         self._output_artifacts: Dict[str, artifact_types.Artifact] = {}
```

### Comparing `kfp-2.0.0b9/kfp/components/executor_main.py` & `kfp-2.0.0rc1/kfp/components/executor_main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/executor_test.py` & `kfp-2.0.0rc1/kfp/components/executor_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -845,14 +845,29 @@
                               "1.23 (<class 'float'>), "
                               "True (<class 'bool'>), "
                               "[1, 2] (<class 'list'>), "
                               "{'a': 1} (<class 'dict'>)."
                 },
             })
 
+    def test_function_with_optional_input_artifact(self):
+        executor_input = """\
+        {
+          "inputs": {},
+          "outputs": {
+            "outputFile": "%(test_dir)s/output_metadata.json"
+          }
+        }
+        """
+
+        def test_func(a: Optional[Input[Artifact]] = None):
+            self.assertIsNone(a)
+
+        self.execute(test_func, executor_input)
+
     def test_function_with_pipeline_task_final_status(self):
         executor_input = """\
     {
       "inputs": {
         "parameterValues": {
           "status": {"error":{"code":9,"message":"The DAG failed because some tasks failed. The failed tasks are: [fail-op]."},"pipelineJobResourceName":"projects/123/locations/us-central1/pipelineJobs/pipeline-456", "pipelineTaskName": "upstream-task", "state":"FAILED"}
         }
```

### Comparing `kfp-2.0.0b9/kfp/components/for_loop.py` & `kfp-2.0.0rc1/kfp/components/for_loop.py`

 * *Files 13% similar despite different names*

```diff
@@ -268,7 +268,48 @@
               LoopArgumentVariable is attached to.
             subvar_name: The name of this subvariable.
 
         Returns:
             The name of this loop arg variable.
         """
         return f'{loop_arg_name}{self.SUBVAR_NAME_DELIMITER}{subvar_name}'
+
+
+class Collected(pipeline_channel.PipelineChannel):
+    """For collecting into a list the output from a task in dsl.ParallelFor
+    loops.
+
+    Args:
+        output: The output of an upstream task within a dsl.ParallelFor loop.
+
+    Example:
+      ::
+
+        @dsl.pipeline
+        def math_pipeline() -> int:
+            with dsl.ParallelFor([1, 2, 3]) as x:
+                t = double(num=x)
+
+        return add(nums=dsl.Collected(t.output)).output
+    """
+
+    def __init__(
+        self,
+        output: pipeline_channel.PipelineChannel,
+    ) -> None:
+        self.output = output
+        if isinstance(output, pipeline_channel.PipelineArtifactChannel):
+            channel_type = output.channel_type
+            self.is_artifact_channel = True
+            # we know all dsl.Collected instances are lists, so set to true
+            # for type checking, which occurs before dsl.Collected is updated to
+            # it's "correct" channel during compilation
+            self.is_artifact_list = True
+        else:
+            channel_type = 'LIST'
+            self.is_artifact_channel = False
+
+        super().__init__(
+            output.name,
+            channel_type=channel_type,
+            task_name=output.task_name,
+        )
```

### Comparing `kfp-2.0.0b9/kfp/components/for_loop_test.py` & `kfp-2.0.0rc1/kfp/components/for_loop_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/graph_component.py` & `kfp-2.0.0rc1/kfp/components/graph_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Pipeline as a component (aka graph component)."""
 
 import inspect
-from typing import Callable
+from typing import Callable, Optional
 import uuid
 
 from kfp.compiler import pipeline_spec_builder as builder
 from kfp.components import base_component
 from kfp.components import pipeline_channel
 from kfp.components import pipeline_context
 from kfp.components import structures
@@ -32,52 +32,59 @@
         pipeline_func: The function that becomes the implementation of this component.
     """
 
     def __init__(
         self,
         component_spec: structures.ComponentSpec,
         pipeline_func: Callable,
-        name: str,
+        display_name: Optional[str] = None,
     ):
         super().__init__(component_spec=component_spec)
         self.pipeline_func = pipeline_func
-        self.name = name
 
         args_list = []
         signature = inspect.signature(pipeline_func)
 
         for arg_name in signature.parameters:
             input_spec = component_spec.inputs[arg_name]
             args_list.append(
                 pipeline_channel.create_pipeline_channel(
-                    name=arg_name, channel_type=input_spec.type))
+                    name=arg_name,
+                    channel_type=input_spec.type,
+                    is_artifact_list=input_spec.is_artifact_list,
+                ))
 
         with pipeline_context.Pipeline(
                 self.component_spec.name) as dsl_pipeline:
             pipeline_outputs = pipeline_func(*args_list)
 
         if not dsl_pipeline.tasks:
             raise ValueError('Task is missing from pipeline.')
 
         # Making the pipeline group name unique to prevent name clashes with
         # templates
         pipeline_group = dsl_pipeline.groups[0]
         pipeline_group.name = uuid.uuid4().hex
 
-        pipeline_spec = builder.create_pipeline_spec(
+        pipeline_spec, platform_spec = builder.create_pipeline_spec(
             pipeline=dsl_pipeline,
             component_spec=self.component_spec,
             pipeline_outputs=pipeline_outputs,
         )
 
         pipeline_root = getattr(pipeline_func, 'pipeline_root', None)
         if pipeline_root is not None:
             pipeline_spec.default_pipeline_root = pipeline_root
+        if display_name is not None:
+            pipeline_spec.pipeline_info.display_name = display_name
+        if component_spec.description is not None:
+            pipeline_spec.pipeline_info.description = component_spec.description
 
         self.component_spec.implementation.graph = pipeline_spec
+        self.component_spec.platform_spec = platform_spec
 
     @property
     def pipeline_spec(self) -> pipeline_spec_pb2.PipelineSpec:
         """Returns the pipeline spec of the component."""
         return self.component_spec.implementation.graph
 
     def execute(self, **kwargs):
```

### Comparing `kfp-2.0.0b9/kfp/components/importer_component.py` & `kfp-2.0.0rc1/kfp/components/importer_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/importer_node.py` & `kfp-2.0.0rc1/kfp/components/importer_node.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/importer_node_test.py` & `kfp-2.0.0rc1/kfp/components/importer_node_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/kfp_config.py` & `kfp-2.0.0rc1/kfp/components/kfp_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/pipeline_channel.py` & `kfp-2.0.0rc1/kfp/components/pipeline_channel.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,14 +93,22 @@
 
         self.name = name
         self.channel_type = channel_type
         # ensure value is None even if empty string or empty list/dict
         # so that serialization and unserialization remain consistent
         # (i.e. None => '' => None)
         self.task_name = task_name or None
+        from kfp.components import pipeline_context
+
+        default_pipeline = pipeline_context.Pipeline.get_default_pipeline()
+        if self.task_name is not None and default_pipeline is not None and default_pipeline.tasks:
+            self.task = pipeline_context.Pipeline.get_default_pipeline().tasks[
+                self.task_name]
+        else:
+            self.task = None
 
     @property
     def full_name(self) -> str:
         """Unique name for the PipelineChannel."""
         return f'{self.task_name}-{self.name}' if self.task_name else self.name
 
     @property
@@ -224,14 +232,15 @@
     """
 
     def __init__(
         self,
         name: str,
         channel_type: Union[str, Dict],
         task_name: Optional[str],
+        is_artifact_list: bool,
     ):
         """Initializes a PipelineArtifactChannel instance.
 
         Args:
             name: The name of the pipeline channel.
             channel_type: The type of the pipeline channel.
             task_name: Optional; the name of the task that produces the pipeline
@@ -240,26 +249,29 @@
         Raises:
             ValueError: If name or task_name contains invalid characters.
             TypeError: If the channel type is not an artifact type.
         """
         if type_utils.is_parameter_type(channel_type):
             raise TypeError(f'{channel_type} is not an artifact type.')
 
+        self.is_artifact_list = is_artifact_list
+
         super(PipelineArtifactChannel, self).__init__(
             name=name,
             channel_type=channel_type,
             task_name=task_name,
         )
 
 
 def create_pipeline_channel(
     name: str,
     channel_type: Union[str, Dict],
     task_name: Optional[str] = None,
     value: Optional[type_utils.PARAMETER_TYPES] = None,
+    is_artifact_list: bool = False,
 ) -> PipelineChannel:
     """Creates a PipelineChannel object.
 
     Args:
         name: The name of the channel.
         channel_type: The type of the channel, which decides whether it is an
             PipelineParameterChannel or PipelineArtifactChannel
@@ -277,14 +289,15 @@
             value=value,
         )
     else:
         return PipelineArtifactChannel(
             name=name,
             channel_type=channel_type,
             task_name=task_name,
+            is_artifact_list=is_artifact_list,
         )
 
 
 def extract_pipeline_channels_from_string(
         payload: str) -> List[PipelineChannel]:
     """Extracts a list of PipelineChannel instances from the payload string.
 
@@ -315,14 +328,16 @@
                 task_name=task_name,
             )
         else:
             pipeline_channel = PipelineArtifactChannel(
                 name=name,
                 channel_type=channel_type,
                 task_name=task_name,
+                # currently no support for getting the index from a list of artifacts (e.g., my_datasets[0].uri), so this will always be False until accessing a single artifact element is supported
+                is_artifact_list=False,
             )
         unique_channels.add(pipeline_channel)
 
     return list(unique_channels)
 
 
 def extract_pipeline_channels_from_any(
```

### Comparing `kfp-2.0.0b9/kfp/components/pipeline_channel_test.py` & `kfp-2.0.0rc1/kfp/components/pipeline_channel_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Tests for kfp.components.pipeline_channel."""
 
 import unittest
 
 from absl.testing import parameterized
+from kfp import dsl
 from kfp.components import pipeline_channel
 
 
 class PipelineChannelTest(parameterized.TestCase):
 
     def test_instantiate_pipline_channel(self):
         with self.assertRaisesRegex(
@@ -30,23 +31,23 @@
             )
 
     def test_invalid_name(self):
         with self.assertRaisesRegex(
                 ValueError,
                 'Only letters, numbers, spaces, "_", and "-" are allowed in the '
                 'name. Must begin with a letter. Got name: 123_abc'):
-            p = pipeline_channel.PipelineParameterChannel(
+            p = pipeline_channel.create_pipeline_channel(
                 name='123_abc',
                 channel_type='String',
             )
 
     def test_task_name_and_value_both_set(self):
         with self.assertRaisesRegex(ValueError,
                                     'task_name and value cannot be both set.'):
-            p = pipeline_channel.PipelineParameterChannel(
+            p = pipeline_channel.create_pipeline_channel(
                 name='abc',
                 channel_type='Integer',
                 task_name='task1',
                 value=123,
             )
 
     def test_invalid_type(self):
@@ -59,84 +60,85 @@
 
         with self.assertRaisesRegex(TypeError,
                                     'String is not an artifact type.'):
             p = pipeline_channel.PipelineArtifactChannel(
                 name='channel1',
                 channel_type='String',
                 task_name='task1',
+                is_artifact_list=False,
             )
 
     @parameterized.parameters(
         {
             'pipeline_channel':
-                pipeline_channel.PipelineParameterChannel(
+                pipeline_channel.create_pipeline_channel(
                     name='channel1',
                     task_name='task1',
                     channel_type='String',
                 ),
             'str_repr':
                 '{{channel:task=task1;name=channel1;type=String;}}',
         },
         {
             'pipeline_channel':
-                pipeline_channel.PipelineParameterChannel(
+                pipeline_channel.create_pipeline_channel(
                     name='channel2',
                     channel_type='Integer',
                 ),
             'str_repr':
                 '{{channel:task=;name=channel2;type=Integer;}}',
         },
         {
             'pipeline_channel':
-                pipeline_channel.PipelineArtifactChannel(
+                pipeline_channel.create_pipeline_channel(
                     name='channel3',
                     channel_type={'type_a': {
                         'property_b': 'c'
                     }},
                     task_name='task3',
                 ),
             'str_repr':
                 '{{channel:task=task3;name=channel3;type={"type_a": {"property_b": "c"}};}}',
         },
         {
             'pipeline_channel':
-                pipeline_channel.PipelineParameterChannel(
+                pipeline_channel.create_pipeline_channel(
                     name='channel4',
                     channel_type='Float',
                     value=1.23,
                 ),
             'str_repr':
                 '{{channel:task=;name=channel4;type=Float;}}',
         },
         {
             'pipeline_channel':
-                pipeline_channel.PipelineArtifactChannel(
+                pipeline_channel.create_pipeline_channel(
                     name='channel5',
                     channel_type='system.Artifact@0.0.1',
                     task_name='task5',
                 ),
             'str_repr':
                 '{{channel:task=task5;name=channel5;type=system.Artifact@0.0.1;}}',
         },
     )
     def test_str_repr(self, pipeline_channel, str_repr):
         self.assertEqual(str_repr, str(pipeline_channel))
 
     def test_extract_pipeline_channels(self):
-        p1 = pipeline_channel.PipelineParameterChannel(
+        p1 = pipeline_channel.create_pipeline_channel(
             name='channel1',
             channel_type='String',
             value='abc',
         )
-        p2 = pipeline_channel.PipelineArtifactChannel(
+        p2 = pipeline_channel.create_pipeline_channel(
             name='channel2',
             channel_type='customized_type_b',
             task_name='task2',
         )
-        p3 = pipeline_channel.PipelineArtifactChannel(
+        p3 = pipeline_channel.create_pipeline_channel(
             name='channel3',
             channel_type={'customized_type_c': {
                 'property_c': 'value_c'
             }},
             task_name='task3',
         )
         stuff_chars = ' between '
@@ -150,9 +152,23 @@
             str(p1) + stuff_chars + str(p2),
             str(p2) + stuff_chars + str(p3)
         ]
         params = pipeline_channel.extract_pipeline_channels_from_any(payload)
         self.assertListEqual([p1, p2, p3], params)
 
 
+class TestCanAccessTask(unittest.TestCase):
+
+    def test(self):
+
+        @dsl.component
+        def comp() -> str:
+            return 'text'
+
+        @dsl.pipeline
+        def my_pipeline():
+            op1 = comp()
+            self.assertEqual(op1.output.task, op1)
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-2.0.0b9/kfp/components/pipeline_context.py` & `kfp-2.0.0rc1/kfp/components/pipeline_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,25 +13,25 @@
 # limitations under the License.
 """Definition for Pipeline."""
 
 import functools
 from typing import Callable, Optional
 
 from kfp.components import component_factory
-from kfp.components import graph_component
 from kfp.components import pipeline_task
 from kfp.components import tasks_group
 from kfp.components import utils
 
 
 def pipeline(func: Optional[Callable] = None,
              *,
              name: Optional[str] = None,
              description: Optional[str] = None,
-             pipeline_root: Optional[str] = None) -> Callable:
+             pipeline_root: Optional[str] = None,
+             display_name: Optional[str] = None) -> Callable:
     """Decorator used to construct a pipeline.
 
     Example
       ::
 
         @pipeline(
           name='my-pipeline',
@@ -44,31 +44,34 @@
     Args:
         func: The Python function that defines a pipeline.
         name: The pipeline name. Defaults to a sanitized version of the
             decorated function name.
         description: A human-readable description of the pipeline.
         pipeline_root: The root directory from which to read input and output
             parameters and artifacts.
+        display_name: A human-readable name for the pipeline.
     """
     if func is None:
         return functools.partial(
             pipeline,
             name=name,
             description=description,
             pipeline_root=pipeline_root,
+            display_name=display_name,
         )
 
-    if name:
-        func._component_human_name = name
-    if description:
-        func._component_description = description
     if pipeline_root:
         func.pipeline_root = pipeline_root
 
-    return component_factory.create_graph_component_from_func(func)
+    return component_factory.create_graph_component_from_func(
+        func,
+        name=name,
+        description=description,
+        display_name=display_name,
+    )
 
 
 class Pipeline:
     """A pipeline contains a list of tasks.
 
     This class is not supposed to be used by pipeline authors since pipeline
     authors can use pipeline functions (decorated with @pipeline) to reference
```

### Comparing `kfp-2.0.0b9/kfp/components/pipeline_task.py` & `kfp-2.0.0rc1/kfp/components/pipeline_task.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Pipeline task class and operations."""
 
 import copy
+import inspect
 import itertools
 import re
 from typing import Any, Dict, List, Mapping, Optional, Union
+import warnings
 
 from kfp.components import constants
 from kfp.components import pipeline_channel
 from kfp.components import placeholders
 from kfp.components import structures
 from kfp.components import utils
 from kfp.components.types import type_utils
+from kfp.pipeline_spec import pipeline_spec_pb2
 
 _register_task_handler = lambda task: utils.maybe_rename_for_k8s(
     task.component_spec.name)
 
 
 class PipelineTask:
     """Represents a pipeline task (instantiated component).
@@ -71,61 +74,42 @@
         self.parent_task_group: Union[None, TasksGroup] = None
         args = args or {}
 
         for input_name, argument_value in args.items():
 
             if input_name not in component_spec.inputs:
                 raise ValueError(
-                    f'Component "{component_spec.name}" got an unexpected input:'
-                    f' {input_name}.')
+                    f'Component {component_spec.name!r} got an unexpected input:'
+                    f' {input_name!r}.')
 
             input_spec = component_spec.inputs[input_name]
-            input_type = input_spec.type
-            argument_type = None
-
-            if isinstance(argument_value, pipeline_channel.PipelineChannel):
-                argument_type = argument_value.channel_type
-            elif isinstance(argument_value, str):
-                argument_type = 'String'
-            elif isinstance(argument_value, bool):
-                argument_type = 'Boolean'
-            elif isinstance(argument_value, int):
-                argument_type = 'Integer'
-            elif isinstance(argument_value, float):
-                argument_type = 'Float'
-            elif isinstance(argument_value, dict):
-                argument_type = 'Dict'
-            elif isinstance(argument_value, list):
-                argument_type = 'List'
-            else:
-                raise ValueError(
-                    'Input argument supports only the following types: '
-                    'str, int, float, bool, dict, and list. Got: '
-                    f'"{argument_value}" of type "{type(argument_value)}".')
 
             type_utils.verify_type_compatibility(
-                given_type=argument_type,
-                expected_type=input_type,
+                given_value=argument_value,
+                expected_spec=input_spec,
                 error_message_prefix=(
-                    'Incompatible argument passed to the input '
-                    f'"{input_name}" of component "{component_spec.name}": '),
+                    f'Incompatible argument passed to the input '
+                    f'{input_name!r} of component {component_spec.name!r}: '),
             )
 
         self.component_spec = component_spec
 
         self._task_spec = structures.TaskSpec(
             name=self._register_task_handler(),
             inputs=dict(args.items()),
             dependent_tasks=[],
             component_ref=component_spec.name,
             enable_caching=True)
 
         self.importer_spec = None
         self.container_spec = None
         self.pipeline_spec = None
+        self._ignore_upstream_failure_tag = False
+        # platform_config for this primitive task; empty if task is for a graph component
+        self.platform_config = {}
 
         def validate_placeholder_types(
                 component_spec: structures.ComponentSpec) -> None:
             inputs_dict = component_spec.inputs or {}
             outputs_dict = component_spec.outputs or {}
             for arg in itertools.chain(
                 (component_spec.implementation.container.command or []),
@@ -144,14 +128,15 @@
             self.pipeline_spec = self.component_spec.implementation.graph
 
         self._outputs = {
             output_name: pipeline_channel.create_pipeline_channel(
                 name=output_name,
                 channel_type=output_spec.type,
                 task_name=self._task_spec.name,
+                is_artifact_list=output_spec.is_artifact_list,
             ) for output_name, output_spec in (
                 component_spec.outputs or {}).items()
         }
 
         self._inputs = args
 
         self._channel_inputs = [
@@ -159,14 +144,28 @@
             if isinstance(value, pipeline_channel.PipelineChannel)
         ] + pipeline_channel.extract_pipeline_channels_from_any([
             value for _, value in args.items()
             if not isinstance(value, pipeline_channel.PipelineChannel)
         ])
 
     @property
+    def platform_spec(self) -> pipeline_spec_pb2.PlatformSpec:
+        """PlatformSpec for all tasks in the pipeline as task.
+
+        Only for use on tasks created from GraphComponents.
+        """
+        if self.pipeline_spec:
+            return self.component_spec.platform_spec
+
+        # can only create primitive task platform spec at compile-time, since the executor label is not known until then
+        raise ValueError(
+            f'Can only access {".platform_spec"!r} property on a tasks created from pipelines. Use {".platform_config"!r} for tasks created from primitive components.'
+        )
+
+    @property
     def name(self) -> str:
         """The name of the task.
 
         Unique within its parent group.
         """
         return self._task_spec.name
 
@@ -244,76 +243,150 @@
 
         Returns:
             Self return to allow chained setting calls.
         """
         self._task_spec.enable_caching = enable_caching
         return self
 
-    def set_cpu_limit(self, cpu: str) -> 'PipelineTask':
-        """Sets CPU limit (maximum) for the task.
+    def _ensure_container_spec_exists(self) -> None:
+        """Ensures that the task has a container spec."""
+        caller_method_name = inspect.stack()[1][3]
+
+        if self.container_spec is None:
+            raise ValueError(
+                f'{caller_method_name} can only be used on single-step components, not pipelines used as components, or special components like importers.'
+            )
+
+    def _validate_cpu_request_limit(self, cpu: str) -> float:
+        """Validates cpu request/limit string and converts to its numeric
+        value.
 
         Args:
-            cpu: Maximum CPU requests allowed. This string should be a number or a number followed by an "m" to indicate millicores (1/1000). For more information, see `Specify a CPU Request and a CPU Limit <https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource/#specify-a-cpu-request-and-a-cpu-limit>`_.
+            cpu: CPU requests or limits. This string should be a number or a
+                number followed by an "m" to indicate millicores (1/1000). For
+                more information, see `Specify a CPU Request and a CPU Limit
+                <https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource/#specify-a-cpu-request-and-a-cpu-limit>`_.
+
+        Raises:
+            ValueError if the cpu request/limit string value is invalid.
 
         Returns:
-            Self return to allow chained setting calls.
+            The numeric value (float) of the cpu request/limit.
         """
         if re.match(r'([0-9]*[.])?[0-9]+m?$', cpu) is None:
             raise ValueError(
                 'Invalid cpu string. Should be float or integer, or integer'
                 ' followed by "m".')
 
-        cpu = float(cpu[:-1]) / 1000 if cpu.endswith('m') else float(cpu)
-        if self.container_spec is None:
-            raise ValueError(
-                'There is no container specified in implementation')
+        return float(cpu[:-1]) / 1000 if cpu.endswith('m') else float(cpu)
+
+    def set_cpu_request(self, cpu: str) -> 'PipelineTask':
+        """Sets CPU request (minimum) for the task.
+
+        Args:
+            cpu: Minimum CPU requests required. This string should be a number
+                or a number followed by an "m" to indicate millicores (1/1000).
+                For more information, see `Specify a CPU Request and a CPU Limit
+                <https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource/#specify-a-cpu-request-and-a-cpu-limit>`_.
+
+        Returns:
+            Self return to allow chained setting calls.
+        """
+        self._ensure_container_spec_exists()
+
+        cpu = self._validate_cpu_request_limit(cpu)
+
+        if self.container_spec.resources is not None:
+            self.container_spec.resources.cpu_request = cpu
+        else:
+            self.container_spec.resources = structures.ResourceSpec(
+                cpu_request=cpu)
+
+        return self
+
+    def set_cpu_limit(self, cpu: str) -> 'PipelineTask':
+        """Sets CPU limit (maximum) for the task.
+
+        Args:
+            cpu: Maximum CPU requests allowed. This string should be a number
+                or a number followed by an "m" to indicate millicores (1/1000).
+                For more information, see `Specify a CPU Request and a CPU Limit
+                <https://kubernetes.io/docs/tasks/configure-pod-container/assign-cpu-resource/#specify-a-cpu-request-and-a-cpu-limit>`_.
+
+        Returns:
+            Self return to allow chained setting calls.
+        """
+        self._ensure_container_spec_exists()
+
+        cpu = self._validate_cpu_request_limit(cpu)
 
         if self.container_spec.resources is not None:
             self.container_spec.resources.cpu_limit = cpu
         else:
             self.container_spec.resources = structures.ResourceSpec(
                 cpu_limit=cpu)
 
         return self
 
-    def set_gpu_limit(self, gpu: str) -> 'PipelineTask':
-        """Sets GPU limit (maximum) for the task. Only applies if accelerator
-        type is also set via .add_node_selector_constraint().
+    def set_accelerator_limit(self, limit: int) -> 'PipelineTask':
+        """Sets accelerator limit (maximum) for the task. Only applies if
+        accelerator type is also set via .set_accelerator_type().
 
         Args:
-            gpu: The maximum GPU reuqests allowed. This string should be a positive integer number of GPUs.
+            limit: Maximum number of accelerators allowed.
 
         Returns:
             Self return to allow chained setting calls.
         """
-        if re.match(r'[1-9]\d*$', gpu) is None:
-            raise ValueError('GPU must be positive integer.')
+        self._ensure_container_spec_exists()
 
-        gpu = int(gpu)
-
-        if self.container_spec is None:
-            raise ValueError(
-                'There is no container specified in implementation')
+        if isinstance(limit, str):
+            if re.match(r'[1-9]\d*$', limit) is None:
+                raise ValueError(f'{"limit"!r} must be positive integer.')
+            limit = int(limit)
 
         if self.container_spec.resources is not None:
-            self.container_spec.resources.accelerator_count = gpu
+            self.container_spec.resources.accelerator_count = limit
         else:
             self.container_spec.resources = structures.ResourceSpec(
-                accelerator_count=gpu)
+                accelerator_count=limit)
 
         return self
 
-    def set_memory_limit(self, memory: str) -> 'PipelineTask':
-        """Sets memory limit (maximum) for the task.
+    def set_gpu_limit(self, gpu: str) -> 'PipelineTask':
+        """Sets GPU limit (maximum) for the task. Only applies if accelerator
+        type is also set via .add_accelerator_type().
 
         Args:
-            memory: The maximum memory requests allowed. This string should be a number or a number followed by one of "E", "Ei", "P", "Pi", "T", "Ti", "G", "Gi", "M", "Mi", "K", or "Ki".
+            gpu: The maximum GPU reuqests allowed. This string should be a positive integer number of GPUs.
 
         Returns:
             Self return to allow chained setting calls.
+
+        :meta private:
+        """
+        warnings.warn(
+            f'{self.set_gpu_limit.__name__!r} is deprecated. Please use {self.set_accelerator_limit.__name__!r} instead.',
+            category=DeprecationWarning)
+        return self.set_accelerator_limit(gpu)
+
+    def _validate_memory_request_limit(self, memory: str) -> float:
+        """Validates memory request/limit string and converts to its numeric
+        value.
+
+        Args:
+            memory: Memory requests or limits. This string should be a number or
+               a number followed by one of "E", "Ei", "P", "Pi", "T", "Ti", "G",
+               "Gi", "M", "Mi", "K", or "Ki".
+
+        Raises:
+            ValueError if the memory request/limit string value is invalid.
+
+        Returns:
+            The numeric value (float) of the memory request/limit.
         """
         if re.match(r'^[0-9]+(E|Ei|P|Pi|T|Ti|G|Gi|M|Mi|K|Ki){0,1}$',
                     memory) is None:
             raise ValueError(
                 'Invalid memory string. Should be a number or a number '
                 'followed by one of "E", "Ei", "P", "Pi", "T", "Ti", "G", '
                 '"Gi", "M", "Mi", "K", "Ki".')
@@ -342,17 +415,53 @@
             memory = float(memory[:-1]) * constants._K / constants._G
         elif memory.endswith('Ki'):
             memory = float(memory[:-2]) * constants._KI / constants._G
         else:
             # By default interpret as a plain integer, in the unit of Bytes.
             memory = float(memory) / constants._G
 
-        if self.container_spec is None:
-            raise ValueError(
-                'There is no container specified in implementation')
+        return memory
+
+    def set_memory_request(self, memory: str) -> 'PipelineTask':
+        """Sets memory request (minimum) for the task.
+
+        Args:
+            memory: The minimum memory requests required. This string should be
+                a number or a number followed by one of "E", "Ei", "P", "Pi",
+                "T", "Ti", "G", "Gi", "M", "Mi", "K", or "Ki".
+
+        Returns:
+            Self return to allow chained setting calls.
+        """
+        self._ensure_container_spec_exists()
+
+        memory = self._validate_memory_request_limit(memory)
+
+        if self.container_spec.resources is not None:
+            self.container_spec.resources.memory_request = memory
+        else:
+            self.container_spec.resources = structures.ResourceSpec(
+                memory_request=memory)
+
+        return self
+
+    def set_memory_limit(self, memory: str) -> 'PipelineTask':
+        """Sets memory limit (maximum) for the task.
+
+        Args:
+            memory: The maximum memory requests allowed. This string should be
+                a number or a number followed by one of "E", "Ei", "P", "Pi",
+                "T", "Ti", "G", "Gi", "M", "Mi", "K", or "Ki".
+
+        Returns:
+            Self return to allow chained setting calls.
+        """
+        self._ensure_container_spec_exists()
+
+        memory = self._validate_memory_request_limit(memory)
 
         if self.container_spec.resources is not None:
             self.container_spec.resources.memory_limit = memory
         else:
             self.container_spec.resources = structures.ResourceSpec(
                 memory_limit=memory)
 
@@ -382,23 +491,34 @@
         )
         return self
 
     def add_node_selector_constraint(self, accelerator: str) -> 'PipelineTask':
         """Sets accelerator type to use when executing this task.
 
         Args:
-            value: The name of the accelerator. Available values include
-                ``'NVIDIA_TESLA_K80'`` and ``'TPU_V3'``.
+            accelerator: The name of the accelerator, such as ``'NVIDIA_TESLA_K80'``, ``'TPU_V3'``, ``'nvidia.com/gpu'`` or ``'cloud-tpus.google.com/v3'``.
 
         Returns:
             Self return to allow chained setting calls.
         """
-        if self.container_spec is None:
-            raise ValueError(
-                'There is no container specified in implementation')
+        warnings.warn(
+            f'{self.add_node_selector_constraint.__name__!r} is deprecated. Please use {self.set_accelerator_type.__name__!r} instead.',
+            category=DeprecationWarning)
+        return self.set_accelerator_type(accelerator)
+
+    def set_accelerator_type(self, accelerator: str) -> 'PipelineTask':
+        """Sets accelerator type to use when executing this task.
+
+        Args:
+            accelerator: The name of the accelerator, such as ``'NVIDIA_TESLA_K80'``, ``'TPU_V3'``, ``'nvidia.com/gpu'`` or ``'cloud-tpus.google.com/v3'``.
+
+        Returns:
+            Self return to allow chained setting calls.
+        """
+        self._ensure_container_spec_exists()
 
         if self.container_spec.resources is not None:
             self.container_spec.resources.accelerator_type = accelerator
             if self.container_spec.resources.accelerator_count is None:
                 self.container_spec.resources.accelerator_count = 1
         else:
             self.container_spec.resources = structures.ResourceSpec(
@@ -424,14 +544,16 @@
         Args:
             name: Environment variable name.
             value: Environment variable value.
 
         Returns:
             Self return to allow chained setting calls.
         """
+        self._ensure_container_spec_exists()
+
         if self.container_spec.env is not None:
             self.container_spec.env[name] = value
         else:
             self.container_spec.env = {name: value}
         return self
 
     def after(self, *tasks) -> 'PipelineTask':
@@ -452,14 +574,50 @@
                 task1 = my_component(text='1st task')
                 task2 = my_component(text='2nd task').after(task1)
         """
         for task in tasks:
             self._task_spec.dependent_tasks.append(task.name)
         return self
 
+    def ignore_upstream_failure(self) -> 'PipelineTask':
+        """If called, the pipeline task will run when any specified upstream
+        tasks complete, even if unsuccessful.
+
+        This method effectively turns the caller task into an exit task
+        if the caller task has upstream dependencies.
+
+        If the task has no upstream tasks, either via data exchange or an explicit dependency via .after(), this method has no effect.
+
+        Returns:
+            Self return to allow chained setting calls.
+
+        Example:
+          ::
+
+            @dsl.pipeline()
+            def my_pipeline(text: str = 'message'):
+                task = fail_op(message=text)
+                clean_up_task = print_op(
+                    message=task.output).ignore_upstream_failure()
+        """
+
+        for input_spec_name, input_spec in (self.component_spec.inputs or
+                                            {}).items():
+            argument_value = self._inputs[input_spec_name]
+            if (isinstance(argument_value, pipeline_channel.PipelineChannel)
+               ) and (not input_spec.optional) and (argument_value.task_name
+                                                    is not None):
+                raise ValueError(
+                    f'Tasks can only use .ignore_upstream_failure() if all input parameters that accept arguments created by an upstream task have a default value, in case the upstream task fails to produce its output. Input parameter task {self.name!r}`s {input_spec_name!r} argument is an output of an upstream task {argument_value.task_name!r}, but {input_spec_name!r} has no default value.'
+                )
+
+        self._ignore_upstream_failure_tag = True
+
+        return self
+
 
 # TODO: this function should ideally be in the function kfp.components.structures.check_placeholder_references_valid_io_name, which does something similar, but this causes the exception to be raised at component definition time, rather than compile time. This would break tests that load v1 component YAML, even though that YAML is invalid.
 def check_primitive_placeholder_is_used_for_correct_io_type(
     inputs_dict: Dict[str, structures.InputSpec],
     outputs_dict: Dict[str, structures.OutputSpec],
     arg: Union[placeholders.CommandLineElement, Any],
 ):
```

### Comparing `kfp-2.0.0b9/kfp/components/pipeline_task_test.py` & `kfp-2.0.0rc1/kfp/components/pipeline_task_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """Tests for kfp.components.pipeline_task."""
 
 import textwrap
 import unittest
 
 from absl.testing import parameterized
+from kfp import dsl
 from kfp.components import pipeline_task
 from kfp.components import placeholders
 from kfp.components import structures
 
 V2_YAML = textwrap.dedent("""\
 components:
   comp-component1:
@@ -107,89 +108,131 @@
             args=[
                 "{{$.inputs.parameters['input1']}}",
                 "{{$.outputs.artifacts['output1'].path}}",
             ],
         )
 
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
         self.assertEqual(task._task_spec, expected_task_spec)
         self.assertEqual(task.component_spec, expected_component_spec)
         self.assertEqual(task.container_spec, expected_container_spec)
 
     def test_create_pipeline_task_invalid_wrong_input(self):
         with self.assertRaisesRegex(
                 ValueError,
-                'Component "component1" got an unexpected input: input0.'):
+                "Component 'component1' got an unexpected input: 'input0'."):
             task = pipeline_task.PipelineTask(
-                component_spec=structures.ComponentSpec
-                .load_from_component_yaml(V2_YAML),
+                component_spec=structures.ComponentSpec.from_yaml_documents(
+                    V2_YAML),
                 args={
                     'input1': 'value',
                     'input0': 'abc',
                 },
             )
 
     def test_set_caching_options(self):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
         task.set_caching_options(False)
         self.assertEqual(False, task._task_spec.enable_caching)
 
     @parameterized.parameters(
         {
-            'cpu_limit': '123',
+            'cpu': '123',
             'expected_cpu_number': 123,
         },
         {
-            'cpu_limit': '123m',
+            'cpu': '123m',
             'expected_cpu_number': 0.123,
         },
         {
-            'cpu_limit': '123.0',
+            'cpu': '123.0',
             'expected_cpu_number': 123,
         },
         {
-            'cpu_limit': '123.0m',
+            'cpu': '123.0m',
             'expected_cpu_number': 0.123,
         },
     )
-    def test_set_valid_cpu_limit(self, cpu_limit: str,
-                                 expected_cpu_number: float):
+    def test_set_valid_cpu_request_limit(self, cpu: str,
+                                         expected_cpu_number: float):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
-        task.set_cpu_limit(cpu_limit)
+        task.set_cpu_request(cpu)
+        self.assertEqual(expected_cpu_number,
+                         task.container_spec.resources.cpu_request)
+        task.set_cpu_limit(cpu)
         self.assertEqual(expected_cpu_number,
                          task.container_spec.resources.cpu_limit)
 
     @parameterized.parameters(
         {
-            'gpu_limit': '666',
-            'expected_gpu_number': 666,
+            'gpu_limit': '123',
+            'expected_gpu_number': 123,
         },)
     def test_set_valid_gpu_limit(self, gpu_limit: str,
                                  expected_gpu_number: int):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
-        task.set_gpu_limit(gpu_limit)
+        with self.assertWarnsRegex(
+                DeprecationWarning,
+                "'set_gpu_limit' is deprecated. Please use 'set_accelerator_limit' instead."
+        ):
+            task.set_gpu_limit(gpu_limit)
         self.assertEqual(expected_gpu_number,
                          task.container_spec.resources.accelerator_count)
 
+    def test_add_valid_node_selector_constraint(self):
+        task = pipeline_task.PipelineTask(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
+                V2_YAML),
+            args={'input1': 'value'},
+        )
+        with self.assertWarnsRegex(
+                DeprecationWarning,
+                "'add_node_selector_constraint' is deprecated. Please use 'set_accelerator_type' instead."
+        ):
+            task.add_node_selector_constraint('TPU_V3')
+        self.assertEqual(task.container_spec.resources.accelerator_type,
+                         'TPU_V3')
+
+    @parameterized.parameters(
+        {
+            'limit': '123',
+            'expected': 123,
+        },
+        {
+            'limit': 123,
+            'expected': 123,
+        },
+    )
+    def test_set_accelerator_limit(self, limit, expected):
+        task = pipeline_task.PipelineTask(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
+                V2_YAML),
+            args={'input1': 'value'},
+        )
+
+        task.set_accelerator_limit(limit)
+        self.assertEqual(expected,
+                         task.container_spec.resources.accelerator_count)
+
     @parameterized.parameters(
         {
             'memory': '1E',
             'expected_memory_number': 1000000000,
         },
         {
             'memory': '15Ei',
@@ -238,60 +281,101 @@
         {
             'memory': '7000',
             'expected_memory_number': 0.000007,
         },
     )
     def test_set_memory_limit(self, memory: str, expected_memory_number: int):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
+        task.set_memory_request(memory)
+        self.assertEqual(expected_memory_number,
+                         task.container_spec.resources.memory_request)
         task.set_memory_limit(memory)
         self.assertEqual(expected_memory_number,
                          task.container_spec.resources.memory_limit)
 
-    def test_add_node_selector_constraint_type_only(self):
+    def test_set_accelerator_type_with_type_only(self):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
-        task.add_node_selector_constraint('NVIDIA_TESLA_K80')
+        task.set_accelerator_type('NVIDIA_TESLA_K80')
         self.assertEqual(
             structures.ResourceSpec(
                 accelerator_type='NVIDIA_TESLA_K80', accelerator_count=1),
             task.container_spec.resources)
 
-    def test_add_node_selector_constraint_accelerator_count(self):
+    def test_set_accelerator_type_with_accelerator_count(self):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
-        task.set_gpu_limit('5').add_node_selector_constraint('TPU_V3')
+        task.set_accelerator_limit('5').set_accelerator_type('TPU_V3')
         self.assertEqual(
             structures.ResourceSpec(
                 accelerator_type='TPU_V3', accelerator_count=5),
             task.container_spec.resources)
 
     def test_set_env_variable(self):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
         task.set_env_variable('env_name', 'env_value')
         self.assertEqual({'env_name': 'env_value'}, task.container_spec.env)
 
     def test_set_display_name(self):
         task = pipeline_task.PipelineTask(
-            component_spec=structures.ComponentSpec.load_from_component_yaml(
+            component_spec=structures.ComponentSpec.from_yaml_documents(
                 V2_YAML),
             args={'input1': 'value'},
         )
         task.set_display_name('test_name')
         self.assertEqual('test_name', task._task_spec.display_name)
 
+    def test_set_cpu_limit_on_pipeline_should_raise(self):
+
+        @dsl.component
+        def comp():
+            print('hello')
+
+        @dsl.pipeline
+        def graph():
+            comp()
+            comp()
+
+        with self.assertRaisesRegex(
+                ValueError,
+                r'set_cpu_limit can only be used on single-step components'):
+
+            @dsl.pipeline
+            def my_pipeline():
+                graph().set_cpu_limit('1')
+
+
+class TestPlatformSpecificFunctionality(unittest.TestCase):
+
+    def test_platform_config_to_platform_spec(self):
+
+        @dsl.component
+        def comp():
+            pass
+
+        @dsl.pipeline
+        def my_pipeline():
+            t = comp()
+            t.platform_config = {'platform1': {'feature': [1, 2, 3]}}
+            with self.assertRaisesRegex(
+                    ValueError,
+                    r"Can only access '\.platform_spec' property on a tasks created from pipelines\. Use '\.platform_config' for tasks created from primitive components\."
+            ):
+                t.platform_spec
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-2.0.0b9/kfp/components/placeholders.py` & `kfp-2.0.0rc1/kfp/components/placeholders.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,58 @@
     def __init__(self, input_name: str) -> None:
         self.input_name = input_name
 
     def _to_string(self) -> str:
         return f"{{{{$.inputs.parameters['{self.input_name}']}}}}"
 
 
+class InputListOfArtifactsPlaceholder(Placeholder):
+
+    def __init__(self, input_name: str) -> None:
+        self.input_name = input_name
+
+    def _to_string(self) -> str:
+        return f"{{{{$.inputs.artifacts['{self.input_name}']}}}}"
+
+    def __getattribute__(self, name: str) -> Any:
+        if name in {'name', 'uri', 'metadata', 'path'}:
+            raise AttributeError(
+                f'Cannot access an attribute on a list of artifacts in a Custom Container Component. Found reference to attribute {name!r} on {self.input_name!r}. Please pass the whole list of artifacts only.'
+            )
+        else:
+            return object.__getattribute__(self, name)
+
+    def __getitem__(self, k: int) -> None:
+        raise KeyError(
+            f'Cannot access individual artifacts in a list of artifacts. Found access to element {k} on {self.input_name!r}. Please pass the whole list of artifacts only.'
+        )
+
+
+class OutputListOfArtifactsPlaceholder(Placeholder):
+
+    def __init__(self, input_name: str) -> None:
+        self.output_name = input_name
+
+    def _to_string(self) -> str:
+        return f"{{{{$.outputs.artifacts['{self.output_name}']}}}}"
+
+    def __getattribute__(self, name: str) -> Any:
+        if name in {'name', 'uri', 'metadata', 'path'}:
+            raise AttributeError(
+                f'Cannot access an attribute on a list of artifacts in a Custom Container Component. Found reference to attribute {name!r} on {self.output_name!r}. Please pass the whole list of artifacts only.'
+            )
+        else:
+            return object.__getattribute__(self, name)
+
+    def __getitem__(self, k: int) -> None:
+        raise KeyError(
+            f'Cannot access individual artifacts in a list of artifacts. Found access to element {k} on {self.output_name!r}. Please pass the whole list of artifacts only.'
+        )
+
+
 class InputPathPlaceholder(Placeholder):
 
     def __init__(self, input_name: str) -> None:
         self.input_name = input_name
 
     def _to_string(self) -> str:
         return f"{{{{$.inputs.artifacts['{self.input_name}'].path}}}}"
@@ -79,14 +123,17 @@
 
     def __init__(self, input_name: str) -> None:
         self.input_name = input_name
 
     def _to_string(self) -> str:
         return f"{{{{$.inputs.artifacts['{self.input_name}'].metadata}}}}"
 
+    def __getitem__(self, key: str) -> str:
+        return f"{{{{$.inputs.artifacts['{self.input_name}'].metadata['{key}']}}}}"
+
 
 class OutputParameterPlaceholder(Placeholder):
 
     def __init__(self, output_name: str) -> None:
         self.output_name = output_name
 
     def _to_string(self) -> str:
@@ -115,14 +162,17 @@
 
     def __init__(self, output_name: str) -> None:
         self.output_name = output_name
 
     def _to_string(self) -> str:
         return f"{{{{$.outputs.artifacts['{self.output_name}'].metadata}}}}"
 
+    def __getitem__(self, key: str) -> str:
+        return f"{{{{$.outputs.artifacts['{self.output_name}'].metadata['{key}']}}}}"
+
 
 class ConcatPlaceholder(Placeholder):
     """Placeholder for concatenating multiple strings. May contain other
     placeholders.
 
     Args:
         items: Elements to concatenate.
@@ -266,18 +316,20 @@
     def __str__(self) -> str:
         raise ValueError(
             f'Cannot use {self.__class__.__name__} in an f-string.')
 
 
 _CONTAINER_PLACEHOLDERS = (IfPresentPlaceholder, ConcatPlaceholder)
 PRIMITIVE_INPUT_PLACEHOLDERS = (InputValuePlaceholder, InputPathPlaceholder,
-                                InputUriPlaceholder, InputMetadataPlaceholder)
+                                InputUriPlaceholder, InputMetadataPlaceholder,
+                                InputListOfArtifactsPlaceholder)
 PRIMITIVE_OUTPUT_PLACEHOLDERS = (OutputParameterPlaceholder,
                                  OutputPathPlaceholder, OutputUriPlaceholder,
-                                 OutputMetadataPlaceholder)
+                                 OutputMetadataPlaceholder,
+                                 OutputListOfArtifactsPlaceholder)
 
 CommandLineElement = Union[str, Placeholder]
 
 
 def convert_command_line_element_to_string(
         element: Union[str, Placeholder]) -> str:
     return element._to_string() if isinstance(element, Placeholder) else element
```

### Comparing `kfp-2.0.0b9/kfp/components/placeholders_test.py` & `kfp-2.0.0rc1/kfp/components/placeholders_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Contains tests for kfp.components.placeholders."""
 import os
 import tempfile
-from typing import Any
+from typing import Any, List
 
 from absl.testing import parameterized
 from kfp import compiler
 from kfp import dsl
 from kfp.components import placeholders
 from kfp.dsl import Artifact
+from kfp.dsl import Dataset
+from kfp.dsl import Input
 from kfp.dsl import Output
 
 
 class TestExecutorInputPlaceholder(parameterized.TestCase):
 
     def test(self):
         self.assertEqual(placeholders.ExecutorInputPlaceholder()._to_string(),
@@ -58,14 +60,26 @@
 class TestInputMetadataPlaceholder(parameterized.TestCase):
 
     def test(self):
         self.assertEqual(
             placeholders.InputMetadataPlaceholder('input1')._to_string(),
             "{{$.inputs.artifacts['input1'].metadata}}")
 
+    def test_access_top_level_metadata_key(self):
+
+        @dsl.container_component
+        def echo(d: Input[Dataset]):
+            return dsl.ContainerSpec(
+                image='alpine', command=['echo', d.metadata['key']])
+
+        self.assertEqual(
+            echo.pipeline_spec.deployment_spec['executors']['exec-echo']
+            ['container']['command'][1],
+            "{{$.inputs.artifacts['d'].metadata['key']}}")
+
 
 class TestOutputPathPlaceholder(parameterized.TestCase):
 
     def test(self):
         self.assertEqual(
             placeholders.OutputPathPlaceholder('output1')._to_string(),
             "{{$.outputs.artifacts['output1'].path}}")
@@ -90,14 +104,26 @@
 class TestOutputMetadataPlaceholder(parameterized.TestCase):
 
     def test(self):
         self.assertEqual(
             placeholders.OutputMetadataPlaceholder('output1')._to_string(),
             "{{$.outputs.artifacts['output1'].metadata}}")
 
+    def test_access_top_level_metadata_key(self):
+
+        @dsl.container_component
+        def echo(d: Output[Dataset]):
+            return dsl.ContainerSpec(
+                image='alpine', command=['echo', d.metadata['key']])
+
+        self.assertEqual(
+            echo.pipeline_spec.deployment_spec['executors']['exec-echo']
+            ['container']['command'][1],
+            "{{$.outputs.artifacts['d'].metadata['key']}}")
+
 
 class TestIfPresentPlaceholder(parameterized.TestCase):
 
     @parameterized.parameters([
         (placeholders.IfPresentPlaceholder(
             input_name='input1', then=['then'], else_=['something']),
          '{"IfPresent": {"InputName": "input1", "Then": ["then"], "Else": ["something"]}}'
@@ -375,14 +401,89 @@
                     then=dsl.IfPresentPlaceholder(
                         input_name='input1',
                         then='single-element',
                         else_=['one', 'two']))
             ])
 
 
+class TestListOfArtifactsInContainerComponentPlaceholders(
+        parameterized.TestCase):
+
+    def test_compile_component1(self):
+
+        @dsl.container_component
+        def comp(input_list: Input[List[Artifact]]):
+            return dsl.ContainerSpec(
+                image='alpine', command=[input_list], args=[input_list])
+
+        self.assertEqual(
+            comp.pipeline_spec.deployment_spec['executors']['exec-comp']
+            ['container']['command'][0], "{{$.inputs.artifacts['input_list']}}")
+        self.assertEqual(
+            comp.pipeline_spec.deployment_spec['executors']['exec-comp']
+            ['container']['args'][0], "{{$.inputs.artifacts['input_list']}}")
+
+    def test_compile_component2(self):
+
+        @dsl.container_component
+        def comp(new_name: Input[List[Dataset]]):
+            return dsl.ContainerSpec(
+                image='alpine', command=[new_name], args=[new_name])
+
+        self.assertEqual(
+            comp.pipeline_spec.deployment_spec['executors']['exec-comp']
+            ['container']['command'][0], "{{$.inputs.artifacts['new_name']}}")
+        self.assertEqual(
+            comp.pipeline_spec.deployment_spec['executors']['exec-comp']
+            ['container']['args'][0], "{{$.inputs.artifacts['new_name']}}")
+
+    def test_cannot_access_name(self):
+        with self.assertRaisesRegex(AttributeError,
+                                    'Cannot access an attribute'):
+
+            @dsl.container_component
+            def comp(new_name: Input[List[Dataset]]):
+                return dsl.ContainerSpec(
+                    image='alpine', command=[new_name.name])
+
+    def test_cannot_access_uri(self):
+        with self.assertRaisesRegex(AttributeError,
+                                    'Cannot access an attribute'):
+
+            @dsl.container_component
+            def comp(new_name: Input[List[Dataset]]):
+                return dsl.ContainerSpec(image='alpine', command=[new_name.uri])
+
+    def test_cannot_access_metadata(self):
+        with self.assertRaisesRegex(AttributeError,
+                                    'Cannot access an attribute'):
+
+            @dsl.container_component
+            def comp(new_name: Input[List[Dataset]]):
+                return dsl.ContainerSpec(
+                    image='alpine', command=[new_name.metadata])
+
+    def test_cannot_access_path(self):
+        with self.assertRaisesRegex(AttributeError,
+                                    'Cannot access an attribute'):
+
+            @dsl.container_component
+            def comp(new_name: Input[List[Dataset]]):
+                return dsl.ContainerSpec(
+                    image='alpine', command=[new_name.path])
+
+    def test_cannot_access_individual_artifact(self):
+        with self.assertRaisesRegex(KeyError,
+                                    'Cannot access individual artifacts'):
+
+            @dsl.container_component
+            def comp(new_name: Input[List[Dataset]]):
+                return dsl.ContainerSpec(image='alpine', command=[new_name[0]])
+
+
 class TestConvertCommandLineElementToStringOrStruct(parameterized.TestCase):
 
     @parameterized.parameters(['a', 'word', 1])
     def test_pass_through(self, val: Any):
         self.assertEqual(
             placeholders.convert_command_line_element_to_string_or_struct(val),
             val)
```

### Comparing `kfp-2.0.0b9/kfp/components/python_component.py` & `kfp-2.0.0rc1/kfp/components/python_component.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,10 +33,12 @@
         self,
         component_spec: structures.ComponentSpec,
         python_func: Callable,
     ):
         super().__init__(component_spec=component_spec)
         self.python_func = python_func
 
+        self._prevent_using_output_lists_of_artifacts()
+
     def execute(self, **kwargs):
         """Executes the Python function that defines the component."""
         return self.python_func(**kwargs)
```

### Comparing `kfp-2.0.0b9/kfp/components/structures.py` & `kfp-2.0.0rc1/kfp/components/structures.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 """Definitions for component spec."""
 
 import ast
 import collections
 import dataclasses
 import itertools
 import re
-from typing import Any, Dict, List, Mapping, Optional, Union
+from typing import Any, Dict, List, Mapping, Optional, Tuple, Union
 import uuid
 
 from google.protobuf import json_format
 import kfp
 from kfp.components import placeholders
 from kfp.components import utils
 from kfp.components import v1_components
@@ -41,20 +41,22 @@
     """Component input definitions.
 
     Attributes:
         type: The type of the input.
         default (optional): the default value for the input.
         optional: Wether the input is optional. An input is optional when it has an explicit default value.
         is_artifact_list: True if `type` represents a list of the artifact type. Only applies when `type` is an artifact.
+        description: Input description.
     """
     type: Union[str, dict]
     default: Optional[Any] = None
     optional: bool = False
     # This special flag for lists of artifacts allows type to be used the same way for list of artifacts and single artifacts. This is aligned with how IR represents lists of artifacts (same as for single artifacts), as well as simplifies downstream type handling/checking operations in the SDK since we don't need to parse the string `type` to determine if single artifact or list.
     is_artifact_list: bool = False
+    description: Optional[str] = None
 
     def __post_init__(self) -> None:
         self._validate_type()
         self._validate_usage_of_optional()
 
     @classmethod
     def from_ir_component_inputs_dict(
@@ -72,26 +74,36 @@
         """
         if 'parameterType' in ir_component_inputs_dict:
             type_string = ir_component_inputs_dict['parameterType']
             type_ = type_utils.IR_TYPE_TO_IN_MEMORY_SPEC_TYPE.get(type_string)
             if type_ is None:
                 raise ValueError(f'Unknown type {type_string} found in IR.')
             default_value = ir_component_inputs_dict.get('defaultValue')
-            # TODO: write the IR is_optional field to IR when compiling. currently we don't do this, so just set optional to True if default_value is not None.
-            optional = default_value is not None
+            # fallback to checking if the parameter has a default value,
+            # since some IR compiled with kfp<=2.0.0b8 will have defaults
+            # without isOptional=True
+            optional = ir_component_inputs_dict.get(
+                'isOptional', 'defaultValue' in ir_component_inputs_dict)
             return InputSpec(
                 type=type_, default=default_value, optional=optional)
 
         else:
             type_ = ir_component_inputs_dict['artifactType']['schemaTitle']
             schema_version = ir_component_inputs_dict['artifactType'][
                 'schemaVersion']
+            # TODO: would be better to extract these fields from the proto
+            # message, as False default would be preserved
+            optional = ir_component_inputs_dict.get('isOptional', False)
+            is_artifact_list = ir_component_inputs_dict.get(
+                'isArtifactList', False)
             return InputSpec(
                 type=type_utils.create_bundled_artifact_type(
-                    type_, schema_version))
+                    type_, schema_version),
+                optional=optional,
+                is_artifact_list=is_artifact_list)
 
     def __eq__(self, other: Any) -> bool:
         """Equality comparison for InputSpec. Robust to different type
         representations, such that it respects the maximum amount of
         information possible to encode in IR. That is, because
         `typing.List[str]` can only be represented a `List` in IR,
         'typing.List' == 'List' in this comparison.
@@ -132,23 +144,23 @@
 @dataclasses.dataclass
 class OutputSpec:
     """Component output definitions.
 
     Attributes:
         type: The type of the output.
         is_artifact_list: True if `type` represents a list of the artifact type. Only applies when `type` is an artifact.
+        description: Output description.
     """
     type: Union[str, dict]
     # This special flag for lists of artifacts allows type to be used the same way for list of artifacts and single artifacts. This is aligned with how IR represents lists of artifacts (same as for single artifacts), as well as simplifies downstream type handling/checking operations in the SDK since we don't need to parse the string `type` to determine if single artifact or list.
     is_artifact_list: bool = False
+    description: Optional[str] = None
 
     def __post_init__(self) -> None:
         self._validate_type()
-        # TODO: remove this method when we support output lists of artifacts
-        self._prevent_using_output_lists_of_artifacts()
 
     @classmethod
     def from_ir_component_outputs_dict(
             cls, ir_component_outputs_dict: Dict[str, Any]) -> 'OutputSpec':
         """Creates an OutputSpec from a ComponentOutputsSpec message in dict
         format (pipeline_spec.components.<component-
         key>.outputDefinitions.parameters|artifacts.<output-key>).
@@ -166,17 +178,20 @@
             if type_ is None:
                 raise ValueError(f'Unknown type {type_string} found in IR.')
             return OutputSpec(type=type_,)
         else:
             type_ = ir_component_outputs_dict['artifactType']['schemaTitle']
             schema_version = ir_component_outputs_dict['artifactType'][
                 'schemaVersion']
+            is_artifact_list = ir_component_outputs_dict.get(
+                'isArtifactList', False)
             return OutputSpec(
                 type=type_utils.create_bundled_artifact_type(
-                    type_, schema_version))
+                    type_, schema_version),
+                is_artifact_list=is_artifact_list)
 
     def __eq__(self, other: Any) -> bool:
         """Equality comparison for OutputSpec. Robust to different type
         representations, such that it respects the maximum amount of
         information possible to encode in IR. That is, because
         `typing.List[str]` can only be represented a `List` in IR,
         'typing.List' == 'List' in this comparison.
@@ -200,39 +215,38 @@
 
         This allows us to perform fewer checks downstream.
         """
         # TODO: add transformation logic so that we don't have to transform outputs at every place they are used, including v1 back compat support
         if not spec_type_is_parameter(self.type):
             type_utils.validate_bundled_artifact_type(self.type)
 
-    def _prevent_using_output_lists_of_artifacts(self):
-        if self.is_artifact_list:
-            raise NotImplementedError(
-                'Output lists of artifacts are not yet supported.')
-
 
 def spec_type_is_parameter(type_: str) -> bool:
     in_memory_type = type_annotations.maybe_strip_optional_from_annotation_string(
         type_utils.get_canonical_name_for_outer_generic(type_))
 
     return in_memory_type in type_utils.IN_MEMORY_SPEC_TYPE_TO_IR_TYPE or in_memory_type == 'PipelineTaskFinalStatus'
 
 
 @dataclasses.dataclass
 class ResourceSpec:
     """The resource requirements of a container execution.
 
     Attributes:
+        cpu_request (optional): the requirement of the number of vCPU cores.
         cpu_limit (optional): the limit of the number of vCPU cores.
+        memory_request (optional): the memory requirement in GB.
         memory_limit (optional): the memory limit in GB.
         accelerator_type (optional): the type of accelerators attached to the
             container.
         accelerator_count (optional): the number of accelerators attached.
     """
+    cpu_request: Optional[float] = None
     cpu_limit: Optional[float] = None
+    memory_request: Optional[float] = None
     memory_limit: Optional[float] = None
     accelerator_type: Optional[str] = None
     accelerator_count: Optional[int] = None
 
 
 @dataclasses.dataclass
 class ContainerSpec:
@@ -333,15 +347,15 @@
             ContainerSpecImplementation: The ContainerSpecImplementation instance.
         """
 
         return ContainerSpecImplementation(
             image=container_dict['image'],
             command=container_dict.get('command'),
             args=container_dict.get('args'),
-            env=None,  # can only be set on tasks
+            env=container_dict.get('env'),
             resources=None)  # can only be set on tasks
 
 
 @dataclasses.dataclass
 class RetryPolicy:
     """The retry policy of a container execution.
 
@@ -550,14 +564,16 @@
             (container, importer) or a DAG consists of other components.
     """
     name: str
     implementation: Implementation
     description: Optional[str] = None
     inputs: Optional[Dict[str, InputSpec]] = None
     outputs: Optional[Dict[str, OutputSpec]] = None
+    platform_spec: pipeline_spec_pb2.PlatformSpec = dataclasses.field(
+        default_factory=pipeline_spec_pb2.PlatformSpec)
 
     def __post_init__(self) -> None:
         self._transform_name()
         self._transform_inputs()
         self._transform_outputs()
         self._validate_placeholders()
 
@@ -636,23 +652,27 @@
         })
 
         inputs = {}
         for spec in component_dict.get('inputs', []):
             type_ = spec.get('type')
             optional = spec.get('optional', False) or 'default' in spec
             default = spec.get('default')
+            default = type_utils.deserialize_v1_component_yaml_default(
+                type_=type_, default=default)
+
+            if isinstance(type_, str):
+                type_ = type_utils.get_canonical_name_for_outer_generic(type_)
 
             if isinstance(type_, str) and type_ == 'PipelineTaskFinalStatus':
-                inputs[utils.sanitize_input_name(
-                    spec['name'])] = InputSpec(type=type_)
+                inputs[utils.sanitize_input_name(spec['name'])] = InputSpec(
+                    type=type_, optional=True)
                 continue
 
             elif isinstance(type_, str) and type_.lower(
             ) in type_utils._PARAMETER_TYPES_MAPPING:
-                default = spec.get('default')
                 type_enum = type_utils._PARAMETER_TYPES_MAPPING[type_.lower()]
                 ir_parameter_type_name = pipeline_spec_pb2.ParameterType.ParameterTypeEnum.Name(
                     type_enum)
                 in_memory_parameter_type_name = type_utils.IR_TYPE_TO_IN_MEMORY_SPEC_TYPE[
                     ir_parameter_type_name]
                 inputs[utils.sanitize_input_name(spec['name'])] = InputSpec(
                     type=in_memory_parameter_type_name,
@@ -678,29 +698,31 @@
                 schema_title = artifact_types.Artifact.schema_title
                 schema_version = artifact_types.Artifact.schema_version
 
             else:
                 raise ValueError(f'Unknown input: {type_}')
 
             if optional:
-                # handles a v1 edge-case where a user marks an artifact input as optional with no default value. some of these v1 component YAMLs exist.
+                # handles optional artifacts with no default value
                 inputs[utils.sanitize_input_name(spec['name'])] = InputSpec(
                     type=type_utils.create_bundled_artifact_type(
                         schema_title, schema_version),
                     default=default,
                     optional=optional,
                 )
             else:
                 inputs[utils.sanitize_input_name(spec['name'])] = InputSpec(
                     type=type_utils.create_bundled_artifact_type(
                         schema_title, schema_version))
 
         outputs = {}
         for spec in component_dict.get('outputs', []):
             type_ = spec.get('type')
+            if isinstance(type_, str):
+                type_ = type_utils.get_canonical_name_for_outer_generic(type_)
 
             if isinstance(type_, str) and type_.lower(
             ) in type_utils._PARAMETER_TYPES_MAPPING:
                 type_enum = type_utils._PARAMETER_TYPES_MAPPING[type_.lower()]
                 ir_parameter_type_name = pipeline_spec_pb2.ParameterType.ParameterTypeEnum.Name(
                     type_enum)
                 in_memory_parameter_type_name = type_utils.IR_TYPE_TO_IN_MEMORY_SPEC_TYPE[
@@ -738,16 +760,21 @@
             description=component_dict.get('description'),
             implementation=Implementation(container=container_spec),
             inputs=inputs,
             outputs=outputs,
         )
 
     @classmethod
-    def from_pipeline_spec_dict(
-            cls, pipeline_spec_dict: Dict[str, Any]) -> 'ComponentSpec':
+    def from_ir_dicts(
+        cls,
+        pipeline_spec_dict: dict,
+        platform_spec_dict: dict,
+    ) -> 'ComponentSpec':
+        """Creates a ComponentSpec from the PipelineSpec and PlatformSpec
+        messages as dicts."""
         raw_name = pipeline_spec_dict['pipelineInfo']['name']
 
         def inputs_dict_from_component_spec_dict(
                 component_spec_dict: Dict[str, Any]) -> Dict[str, InputSpec]:
             parameters = component_spec_dict.get('inputDefinitions',
                                                  {}).get('parameters', {})
             artifacts = component_spec_dict.get('inputDefinitions',
@@ -793,44 +820,35 @@
         implementation = Implementation.from_pipeline_spec_dict(
             pipeline_spec_dict, raw_name)
 
         description = extract_description_from_command(
             implementation.container.command or
             []) if implementation.container else None
 
+        platform_spec = pipeline_spec_pb2.PlatformSpec()
+        json_format.ParseDict(platform_spec_dict, platform_spec)
+
         return ComponentSpec(
             name=raw_name,
             implementation=implementation,
             description=description,
             inputs=inputs,
-            outputs=outputs)
-
-    @classmethod
-    def from_pipeline_spec_yaml(cls,
-                                pipeline_spec_yaml: str) -> 'ComponentSpec':
-        """Creates a ComponentSpec from a pipeline spec in YAML format.
-
-        Args:
-            component_yaml (str): Component spec in YAML format.
-
-        Returns:
-            ComponentSpec: The component spec object.
-        """
-        return ComponentSpec.from_pipeline_spec_dict(
-            yaml.safe_load(pipeline_spec_yaml))
+            outputs=outputs,
+            platform_spec=platform_spec,
+        )
 
     @classmethod
-    def load_from_component_yaml(cls, component_yaml: str) -> 'ComponentSpec':
-        """Loads V1 or V2 component yaml into ComponentSpec.
+    def from_yaml_documents(cls, component_yaml: str) -> 'ComponentSpec':
+        """Loads V1 or V2 component YAML into a ComponentSpec.
 
         Args:
-            component_yaml: the component yaml in string format.
+            component_yaml: PipelineSpec and optionally PlatformSpec YAML documents as a single string.
 
         Returns:
-            Component spec in the form of V2 ComponentSpec.
+            ComponentSpec: The ComponentSpec object.
         """
 
         def extract_description(component_yaml: str) -> Union[str, None]:
             heading = '# Description: '
             multi_line_description_prefix = '#             '
             index_of_heading = 2
             if heading in component_yaml:
@@ -845,38 +863,45 @@
                         len(multi_line_description_prefix) + 1:]
                     index += 1
 
                 return description[len(heading):]
             else:
                 return None
 
-        json_component = yaml.safe_load(component_yaml)
-        is_v1 = 'implementation' in set(json_component.keys())
+        pipeline_spec_dict, platform_spec_dict = load_documents_from_yaml(
+            component_yaml)
+
+        is_v1 = 'implementation' in set(pipeline_spec_dict.keys())
         if is_v1:
             v1_component = v1_components._load_component_spec_from_component_text(
                 component_yaml)
             return cls.from_v1_component_spec(v1_component)
         else:
-            component_spec = ComponentSpec.from_pipeline_spec_dict(
-                json_component)
+            component_spec = ComponentSpec.from_ir_dicts(
+                pipeline_spec_dict, platform_spec_dict)
             if not component_spec.description:
                 component_spec.description = extract_description(
                     component_yaml=component_yaml)
             return component_spec
 
     def save_to_component_yaml(self, output_file: str) -> None:
         """Saves ComponentSpec into IR YAML file.
 
         Args:
             output_file: File path to store the component yaml.
         """
         from kfp.compiler import pipeline_spec_builder as builder
 
         pipeline_spec = self.to_pipeline_spec()
-        builder.write_pipeline_spec_to_file(pipeline_spec, None, output_file)
+        builder.write_pipeline_spec_to_file(
+            pipeline_spec,
+            None,
+            pipeline_spec_pb2.PlatformSpec(),
+            output_file,
+        )
 
     def to_pipeline_spec(self) -> pipeline_spec_pb2.PipelineSpec:
         """Creates a pipeline instance and constructs the pipeline spec for a
         single component.
 
         Args:
             component_spec: The ComponentSpec to convert to PipelineSpec.
@@ -892,50 +917,57 @@
         from kfp.components import tasks_group
 
         args_dict = {}
         pipeline_inputs = self.inputs or {}
 
         for arg_name, input_spec in pipeline_inputs.items():
             args_dict[arg_name] = pipeline_channel.create_pipeline_channel(
-                name=arg_name, channel_type=input_spec.type)
+                name=arg_name,
+                channel_type=input_spec.type,
+                is_artifact_list=input_spec.is_artifact_list)
 
         task = pipeline_task.PipelineTask(self, args_dict)
 
         # instead of constructing a pipeline with pipeline_context.Pipeline,
         # just build the single task group
         group = tasks_group.TasksGroup(
             group_type=tasks_group.TasksGroupType.PIPELINE)
         group.tasks.append(task)
 
-        # Fill in the default values.
-        args_list_with_defaults = [
-            pipeline_channel.create_pipeline_channel(
-                name=input_name,
-                channel_type=input_spec.type,
-                value=input_spec.default,
-            ) for input_name, input_spec in pipeline_inputs.items()
-        ]
         group.name = uuid.uuid4().hex
 
         pipeline_name = self.name
-        pipeline_args = args_list_with_defaults
         task_group = group
 
+        pipeline_outputs = {}
+        pipeline_output_spec = self.outputs or {}
+
+        for arg_name, output_spec in pipeline_output_spec.items():
+            pipeline_outputs[
+                arg_name] = pipeline_channel.create_pipeline_channel(
+                    name=arg_name,
+                    channel_type=output_spec.type,
+                    task_name=task.name)
+
         utils.validate_pipeline_name(pipeline_name)
 
         pipeline_spec = pipeline_spec_pb2.PipelineSpec()
         pipeline_spec.pipeline_info.name = pipeline_name
         pipeline_spec.sdk_version = f'kfp-{kfp.__version__}'
         # Schema version 2.1.0 is required for kfp-pipeline-spec>0.1.13
         pipeline_spec.schema_version = '2.1.0'
-        pipeline_spec.root.CopyFrom(
-            builder.build_component_spec_for_group(
-                pipeline_channels=pipeline_args,
-                is_root_group=True,
-            ))
+
+        # if we decide to surface component outputs to pipeline level,
+        # can just assign the component_spec_proto directly to .root
+        component_spec_proto = builder._build_component_spec_from_component_spec_structure(
+            self)
+        pipeline_spec.root.CopyFrom(component_spec_proto)
+
+        builder._build_dag_outputs(
+            component_spec=pipeline_spec.root, dag_outputs=pipeline_outputs)
 
         deployment_config = pipeline_spec_pb2.PipelineDeploymentConfig()
         root_group = task_group
 
         task_name_to_parent_groups, group_name_to_parent_groups = compiler_utils.get_parent_groups(
             root_group)
 
@@ -955,19 +987,24 @@
         inputs = get_inputs(task_group, task_name_to_parent_groups)
 
         builder.build_spec_by_group(
             pipeline_spec=pipeline_spec,
             deployment_config=deployment_config,
             group=root_group,
             inputs=inputs,
+            outputs=collections.defaultdict(
+                dict),  # empty -- no sub-DAG outputs to surface
             dependencies={},  # no dependencies for single-component pipeline
             rootgroup_name=root_group.name,
             task_name_to_parent_groups=task_name_to_parent_groups,
             group_name_to_parent_groups=group_name_to_parent_groups,
-            name_to_for_loop_group={},  # no for loop for single-component pipeline
+            name_to_for_loop_group={},  # no for loop in single-component pipeline
+            platform_spec=pipeline_spec_pb2.PlatformSpec(
+            ),  # no PlatformSpec single-component pipeline
+            is_compiled_component=True,
         )
 
         return pipeline_spec
 
 
 def normalize_time_string(duration: str) -> str:
     """Normalizes a time string.
@@ -1011,7 +1048,28 @@
     """
     duration = normalize_time_string(duration)
     seconds_per_unit = {'s': 1, 'm': 60, 'h': 3_600, 'd': 86_400, 'w': 604_800}
     if duration[-1] not in seconds_per_unit.keys():
         raise ValueError(
             f"Unsupported duration unit: '{duration[-1]}' for '{duration}'.")
     return int(duration[:-1]) * seconds_per_unit[duration[-1]]
+
+
+def load_documents_from_yaml(component_yaml: str) -> Tuple[dict, dict]:
+    """Loads up to two YAML documents from a YAML string.
+
+    First document must always be present. If second document is
+    present, it is returned as a dict, else an empty dict.
+    """
+    documents = list(yaml.safe_load_all(component_yaml))
+    num_docs = len(documents)
+    if num_docs == 1:
+        pipeline_spec_dict = documents[0]
+        platform_spec_dict = {}
+    elif num_docs == 2:
+        pipeline_spec_dict = documents[0]
+        platform_spec_dict = documents[1]
+    else:
+        raise ValueError(
+            f'Expected one or two YAML documents in the IR YAML file. Got: {num_docs}.'
+        )
+    return pipeline_spec_dict, platform_spec_dict
```

### Comparing `kfp-2.0.0b9/kfp/components/structures_test.py` & `kfp-2.0.0rc1/kfp/components/structures_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import os
 import tempfile
 import textwrap
 import unittest
 
 from absl.testing import parameterized
 from kfp import compiler
+from kfp import components
 from kfp import dsl
 from kfp.components import component_factory
 from kfp.components import placeholders
 from kfp.components import structures
 
 V1_YAML_IF_PLACEHOLDER = textwrap.dedent("""\
     implementation:
@@ -161,14 +162,31 @@
                 placeholders.ExecutorInputPlaceholder(),
                 '--function_name',
                 'test_function',
             ])),
     inputs={'input': structures.InputSpec(type='String')},
 )
 
+V1_NONCANONICAL_GENERIC_TYPES_COMPONENT_SPEC = textwrap.dedent("""\
+    name: generic_types_test
+    inputs:
+    - {name: input1, type: "List[str]"}
+    - {name: input2, type: "typing.List[str]"}
+    - {name: input3, type: "Dict[str, str]"}
+    - {name: input4, type: "typing.Dict[str, str]"}
+    outputs:
+    - {name: output1, type: "List[str]"}
+    - {name: output2, type: "typing.List[str]"}
+    - {name: output3, type: "Dict[str, str]"}
+    - {name: output4, type: "typing.Dict[str, str]"}
+    implementation:
+      container:
+        image: alpine
+    """)
+
 
 class StructuresTest(parameterized.TestCase):
 
     def test_component_spec_with_placeholder_referencing_nonexisting_input_output(
             self):
         with self.assertRaisesRegex(
                 ValueError,
@@ -228,30 +246,28 @@
                         "{{$.inputs.parameters['input1']}}",
                         "{{$.outputs.parameters['output1'].output_file}}"
                     ],
                 )),
             inputs={'input1': structures.InputSpec(type='String')},
             outputs={'output1': structures.OutputSpec(type='String')},
         )
-        from kfp.components import base_component
-
-        class TestComponent(base_component.BaseComponent):
 
-            def execute(self, **kwargs):
-                pass
-
-        test_component = TestComponent(component_spec=original_component_spec)
+        test_component = components.PythonComponent(
+            # dummy python_func not used in behavior that is being tested
+            python_func=lambda: None,
+            component_spec=original_component_spec,
+        )
         with tempfile.TemporaryDirectory() as tempdir:
             output_path = os.path.join(tempdir, 'component.yaml')
             compiler.Compiler().compile(test_component, output_path)
 
             # test that it can be read back correctly
             with open(output_path, 'r') as f:
                 contents = f.read()
-            new_component_spec = structures.ComponentSpec.load_from_component_yaml(
+            new_component_spec = structures.ComponentSpec.from_yaml_documents(
                 contents)
 
         self.assertEqual(original_component_spec, new_component_spec)
 
     def test_simple_component_spec_load_from_v2_component_yaml(self):
         component_yaml_v2 = textwrap.dedent("""\
 components:
@@ -298,15 +314,15 @@
     parameters:
       input1:
         parameterType: STRING
 schemaVersion: 2.1.0
 sdkVersion: kfp-2.0.0-alpha.2
         """)
 
-        generated_spec = structures.ComponentSpec.load_from_component_yaml(
+        generated_spec = structures.ComponentSpec.from_yaml_documents(
             component_yaml_v2)
 
         expected_spec = structures.ComponentSpec(
             name='component-1',
             implementation=structures.Implementation(
                 container=structures.ContainerSpecImplementation(
                     image='alpine',
@@ -339,15 +355,15 @@
         {
             'yaml': V1_YAML_EXECUTOR_INPUT_PLACEHOLDER,
             'expected_component': COMPONENT_SPEC_EXECUTOR_INPUT_PLACEHOLDER
         },
     )
     def test_component_spec_placeholder_load_from_v2_component_yaml(
             self, yaml, expected_component):
-        generated_spec = structures.ComponentSpec.load_from_component_yaml(yaml)
+        generated_spec = structures.ComponentSpec.from_yaml_documents(yaml)
         self.assertEqual(generated_spec, expected_component)
 
     def test_component_spec_load_from_v1_component_yaml(self):
         component_yaml_v1 = textwrap.dedent("""\
         name: Component with 2 inputs and 2 outputs
         inputs:
         - {name: Input parameter, type: String}
@@ -368,15 +384,15 @@
             args:
             - {inputValue: Input parameter}
             - {inputPath: Input artifact}
             - {outputPath: Output 1}
             - {outputPath: Output 2}
         """)
 
-        generated_spec = structures.ComponentSpec.load_from_component_yaml(
+        generated_spec = structures.ComponentSpec.from_yaml_documents(
             component_yaml_v1)
 
         expected_spec = structures.ComponentSpec(
             name='Component with 2 inputs and 2 outputs',
             implementation=structures.Implementation(
                 container=structures.ContainerSpecImplementation(
                     image='busybox',
@@ -433,57 +449,35 @@
         self.assertEqual(obj.env, {'env': 'env'})
 
         obj = structures.ContainerSpecImplementation(
             image='image', command=[], args=[], env={})
         self.assertEqual(obj.env, None)
 
     def test_from_container_dict_no_placeholders(self):
-        component_spec = structures.ComponentSpec(
-            name='test',
-            implementation=structures.Implementation(
-                container=structures.ContainerSpecImplementation(
-                    image='python:3.7',
-                    command=[
-                        'sh', '-c',
-                        '\nif ! [ -x "$(command -v pip)" ]; then\n    python3 -m ensurepip || python3 -m ensurepip --user || apt-get install python3-pip\nfi\n\nPIP_DISABLE_PIP_VERSION_CHECK=1 python3 -m pip install --quiet     --no-warn-script-location \'kfp==2.0.0-alpha.2\' && "$0" "$@"\n',
-                        'sh', '-ec',
-                        'program_path=$(mktemp -d)\nprintf "%s" "$0" > "$program_path/ephemeral_component.py"\npython3 -m kfp.components.executor_main                         --component_module_path                         "$program_path/ephemeral_component.py"                         "$@"\n',
-                        '\nimport kfp\nfrom kfp import dsl\nfrom kfp.dsl import *\nfrom typing import *\n\ndef concat_message(first: str, second: str) -> str:\n    return first + second\n\n'
-                    ],
-                    args=[
-                        '--executor_input',
-                        placeholders.ExecutorInputPlaceholder(),
-                        '--function_to_execute', 'concat_message'
-                    ],
-                    env=None,
-                    resources=None),
-                graph=None,
-                importer=None),
-            description=None,
-            inputs={
-                'first': structures.InputSpec(type='String', default=None),
-                'second': structures.InputSpec(type='String', default=None)
-            },
-            outputs={'Output': structures.OutputSpec(type='String')})
+        expected_container_spec = structures.ContainerSpecImplementation(
+            image='python:3.7',
+            command=['sh', '-c', 'dummy'],
+            args=['--executor_input', '{{$}}', '--function_to_execute', 'func'],
+            env={'ENV1': 'val1'},
+            resources=None)
+
         container_dict = {
             'args': [
-                '--executor_input', '{{$}}', '--function_to_execute', 'fail_op'
-            ],
-            'command': [
-                'sh', '-c',
-                '\nif ! [ -x "$(command -v pip)" ]; then\n    python3 -m ensurepip || python3 -m ensurepip --user || apt-get install python3-pip\nfi\n\nPIP_DISABLE_PIP_VERSION_CHECK=1 python3 -m pip install --quiet     --no-warn-script-location \'kfp==2.0.0-alpha.2\' && "$0" "$@"\n',
-                'sh', '-ec',
-                'program_path=$(mktemp -d)\nprintf "%s" "$0" > "$program_path/ephemeral_component.py"\npython3 -m kfp.components.executor_main                         --component_module_path                         "$program_path/ephemeral_component.py"                         "$@"\n',
-                '\nimport kfp\nfrom kfp import dsl\nfrom kfp.dsl import *\nfrom typing import *\n\ndef fail_op(message: str):\n    """Fails."""\n    import sys\n    print(message)\n    sys.exit(1)\n\n'
+                '--executor_input', '{{$}}', '--function_to_execute', 'func'
             ],
-            'image': 'python:3.7'
+            'command': ['sh', '-c', 'dummy'],
+            'image': 'python:3.7',
+            'env': {
+                'ENV1': 'val1'
+            },
         }
 
         loaded_container_spec = structures.ContainerSpecImplementation.from_container_dict(
             container_dict)
+        self.assertEqual(expected_container_spec, loaded_container_spec)
 
     def test_raise_error_if_access_artifact_by_itself(self):
 
         def comp_with_artifact_input(dataset: dsl.Input[dsl.Dataset]):
             return dsl.ContainerSpec(
                 image='gcr.io/my-image',
                 command=['sh', 'run.sh'],
@@ -641,15 +635,15 @@
     name: component_if
     """)
 
 
 class TestReadInComponent(parameterized.TestCase):
 
     def test_read_v1(self):
-        component_spec = structures.ComponentSpec.load_from_component_yaml(
+        component_spec = structures.ComponentSpec.from_yaml_documents(
             V1_YAML_IF_PLACEHOLDER)
         self.assertEqual(component_spec.name, 'component-if')
         self.assertEqual(component_spec.implementation.container.image,
                          'alpine')
 
     def test_simple_placeholder(self):
         compiled_yaml = textwrap.dedent("""
@@ -696,15 +690,15 @@
           name: component1
   inputDefinitions:
     parameters:
       input1:
         parameterType: STRING
 schemaVersion: 2.1.0
 sdkVersion: kfp-2.0.0-alpha.2""")
-        loaded_component_spec = structures.ComponentSpec.load_from_component_yaml(
+        loaded_component_spec = structures.ComponentSpec.from_yaml_documents(
             compiled_yaml)
         component_spec = structures.ComponentSpec(
             name='component1',
             implementation=structures.Implementation(
                 container=structures.ContainerSpecImplementation(
                     image='alpine',
                     command=['sh', '-c', 'echo "$0" >> "$1"'],
@@ -764,15 +758,15 @@
           name: if
   inputDefinitions:
     parameters:
       optional_input_1:
         parameterType: STRING
 schemaVersion: 2.1.0
 sdkVersion: kfp-2.0.0-alpha.2""")
-        loaded_component_spec = structures.ComponentSpec.load_from_component_yaml(
+        loaded_component_spec = structures.ComponentSpec.from_yaml_documents(
             compiled_yaml)
         component_spec = structures.ComponentSpec(
             name='if',
             implementation=structures.Implementation(
                 container=structures.ContainerSpecImplementation(
                     image='alpine',
                     command=['sh', '-c', 'echo "$0" "$1"'],
@@ -835,15 +829,15 @@
     parameters:
       input1:
         parameterType: STRING
       input2:
         parameterType: STRING
 schemaVersion: 2.1.0
 sdkVersion: kfp-2.0.0-alpha.2""")
-        loaded_component_spec = structures.ComponentSpec.load_from_component_yaml(
+        loaded_component_spec = structures.ComponentSpec.from_yaml_documents(
             compiled_yaml)
         component_spec = structures.ComponentSpec(
             name='concat',
             implementation=structures.Implementation(
                 container=structures.ContainerSpecImplementation(
                     image='alpine',
                     command=[
@@ -918,9 +912,248 @@
         self.assertEqual(retry_policy_proto.max_retry_count, 10)
         self.assertEqual(retry_policy_proto.backoff_duration.seconds, 3600)
         self.assertEqual(retry_policy_proto.backoff_factor, 1.5)
         # tests cap
         self.assertEqual(retry_policy_proto.backoff_max_duration.seconds, 3600)
 
 
+class TestDeserializeV1ComponentYamlDefaults(unittest.TestCase):
+
+    def test_True(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Boolean, default: "True" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, True)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.bool_value, True)
+
+    def test_true(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Boolean, default: "true" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, True)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.bool_value, True)
+
+    def test_false(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Boolean, default: "false" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, False)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.bool_value, False)
+
+    def test_False(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Boolean, default: "False" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, False)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.bool_value, False)
+
+    def test_int(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Integer, default: "1" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, 1)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.number_value, 1.0)
+
+    def test_float(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: Float, default: "1.0" }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, 1.0)
+        self.assertEqual(
+            comp.pipeline_spec.root.input_definitions.parameters['val']
+            .default_value.number_value, 1.0)
+
+    def test_struct(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: JsonObject, default: '{"a": 1.0}' }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, {'a': 1.0})
+        self.assertEqual(
+            dict(comp.pipeline_spec.root.input_definitions.parameters['val']
+                 .default_value.struct_value), {'a': 1.0})
+
+    def test_array(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: JsonObject, default: '["a", 1.0]' }
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputValue: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertEqual(comp.component_spec.inputs['val'].default, ['a', 1.0])
+        self.assertEqual(
+            list(comp.pipeline_spec.root.input_definitions.parameters['val']
+                 .default_value.list_value), ['a', 1.0])
+
+    def test_artifact_with_dict_type_passes_through(self):
+        comp_text = textwrap.dedent("""\
+inputs:
+  - { name: val, type: {Key: Val}}
+implementation:
+  container:
+    image: alpine
+    command:
+      - sh
+      - -c
+      - |
+        echo $0
+      - { inputPath: val }
+""")
+        comp = components.load_component_from_text(comp_text)
+        self.assertFalse(comp.component_spec.inputs['val'].optional)
+        self.assertFalse(comp.pipeline_spec.root.input_definitions
+                         .artifacts['val'].is_optional)
+
+    def test_load_noncanonical_v1_generic_types(self):
+        loaded_comp = components.load_component_from_text(
+            V1_NONCANONICAL_GENERIC_TYPES_COMPONENT_SPEC)
+        inputs = loaded_comp.component_spec.inputs
+        outputs = loaded_comp.component_spec.outputs
+        self.assertEqual(inputs['input1'].type, 'List')
+        self.assertEqual(inputs['input2'].type, 'List')
+        self.assertEqual(inputs['input3'].type, 'Dict')
+        self.assertEqual(inputs['input4'].type, 'Dict')
+
+        self.assertEqual(outputs['output1'].type, 'List')
+        self.assertEqual(outputs['output2'].type, 'List')
+        self.assertEqual(outputs['output3'].type, 'Dict')
+        self.assertEqual(outputs['output4'].type, 'Dict')
+
+
+class TestLoadDocumentsFromYAML(unittest.TestCase):
+
+    def test_no_documents(self):
+        with self.assertRaisesRegex(
+                ValueError,
+                r'Expected one or two YAML documents in the IR YAML file\. Got\: 0\.'
+        ):
+            structures.load_documents_from_yaml('')
+
+    def test_one_document(self):
+        doc1, doc2 = structures.load_documents_from_yaml(
+            textwrap.dedent("""\
+            key1: value1
+            """))
+        self.assertEqual(doc1, {'key1': 'value1'})
+        self.assertEqual(doc2, {})
+
+    def test_two_documents(self):
+        doc1, doc2 = structures.load_documents_from_yaml(
+            textwrap.dedent("""\
+            key1: value1
+            ---
+            key2: value2
+            """))
+        self.assertEqual(doc1, {'key1': 'value1'})
+        self.assertEqual(doc2, {'key2': 'value2'})
+
+    def test_three_documents(self):
+        with self.assertRaisesRegex(
+                ValueError,
+                r'Expected one or two YAML documents in the IR YAML file\. Got\: 3\.'
+        ):
+            structures.load_documents_from_yaml(
+                textwrap.dedent("""\
+                key3: value3
+                ---
+                key3: value3
+                ---
+                key3: value3
+                """))
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `kfp-2.0.0b9/kfp/components/task_final_status.py` & `kfp-2.0.0rc1/kfp/components/task_final_status.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/tasks_group.py` & `kfp-2.0.0rc1/kfp/components/tasks_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def _make_name_unique(self):
         """Generates a unique TasksGroup name in the pipeline."""
         if not pipeline_context.Pipeline.get_default_pipeline():
             raise ValueError('Default pipeline not defined.')
 
         group_id = pipeline_context.Pipeline.get_default_pipeline(
         ).get_next_group_id()
-        self.name = f'{self.group_type}-{group_id}'
+        self.name = f'{self.group_type.value}-{group_id}'
         self.name = self.name.replace('_', '-')
 
     def remove_task_recursive(self, task: pipeline_task.PipelineTask):
         """Removes a task from the group recursively."""
         if self.tasks and task in self.tasks:
             self.tasks.remove(task)
         for group in self.groups or []:
```

### Comparing `kfp-2.0.0b9/kfp/components/tasks_group_test.py` & `kfp-2.0.0rc1/kfp/components/tasks_group_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/__init__.py` & `kfp-2.0.0rc1/kfp/components/types/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/artifact_types.py` & `kfp-2.0.0rc1/kfp/components/types/artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/artifact_types_test.py` & `kfp-2.0.0rc1/kfp/components/types/artifact_types_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/custom_artifact_types.py` & `kfp-2.0.0rc1/kfp/components/types/custom_artifact_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/custom_artifact_types_test.py` & `kfp-2.0.0rc1/kfp/components/types/custom_artifact_types_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/types/type_annotations.py` & `kfp-2.0.0rc1/kfp/components/types/type_annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,19 +102,23 @@
         type_: Union[str, Type, None]) -> Union[str, None]:
     if type_annotations.is_artifact_class(type_):
         return type_utils.create_bundled_artifact_type(type_.schema_title,
                                                        type_.schema_version)
     elif isinstance(
             type_,
             str) and type_.lower() in type_utils._ARTIFACT_CLASSES_MAPPING:
-        # v1 artifact backward compat
+        # v1 artifact backward compat, e.g. dsl.OutputPath('Dataset')
         return type_utils.create_bundled_artifact_type(
             type_utils._ARTIFACT_CLASSES_MAPPING[type_.lower()].schema_title)
-    else:
+    elif type_utils.get_parameter_type(type_):
         return type_
+    else:
+        # v1 unknown type dsl.OutputPath('MyCustomType')
+        return type_utils.create_bundled_artifact_type(
+            artifact_types.Artifact.schema_title)
 
 
 class InputAnnotation:
     """Marker type for input artifacts."""
 
 
 class OutputAnnotation:
```

### Comparing `kfp-2.0.0b9/kfp/components/types/type_annotations_test.py` & `kfp-2.0.0rc1/kfp/components/types/type_annotations_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/utils.py` & `kfp-2.0.0rc1/kfp/components/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
         package_path: The package under which the specified module resides.
     """
     module_spec = importlib.util.spec_from_file_location(
         name=module_name,
         location=os.path.join(module_directory, f'{module_name}.py'))
     module = importlib.util.module_from_spec(module_spec)
     sys.modules[module_spec.name] = module
+    sys.path.insert(0, str(module_directory))
     module_spec.loader.exec_module(module)
     return module
 
 
 def maybe_rename_for_k8s(name: str) -> str:
     """Cleans and converts a name to be k8s compatible.
```

### Comparing `kfp-2.0.0b9/kfp/components/utils_test.py` & `kfp-2.0.0rc1/kfp/components/utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/v1_components.py` & `kfp-2.0.0rc1/kfp/components/v1_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/v1_modelbase.py` & `kfp-2.0.0rc1/kfp/components/v1_modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/v1_structures.py` & `kfp-2.0.0rc1/kfp/components/v1_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/components/yaml_component.py` & `kfp-2.0.0rc1/kfp/components/yaml_component.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from typing import Optional, Tuple
 
 from google.protobuf import json_format
 from kfp import components
 from kfp.components import structures
 from kfp.pipeline_spec import pipeline_spec_pb2
 import requests
-import yaml
 
 
 class YamlComponent(components.BaseComponent):
     """A component loaded from a YAML file.
 
     **Note:** ``YamlComponent`` is not intended to be used to construct components directly. Use ``kfp.components.load_component_from_*()`` instead.
 
@@ -40,15 +39,16 @@
     ):
         super().__init__(component_spec=component_spec)
         self.component_yaml = component_yaml
 
     @property
     def pipeline_spec(self) -> pipeline_spec_pb2.PipelineSpec:
         """Returns the pipeline spec of the component."""
-        component_dict = yaml.safe_load(self.component_yaml)
+        component_dict = structures.load_documents_from_yaml(
+            self.component_yaml)[0]
         is_v1 = 'implementation' in set(component_dict.keys())
         if is_v1:
             return self.component_spec.to_pipeline_spec()
         else:
             return json_format.ParseDict(component_dict,
                                          pipeline_spec_pb2.PipelineSpec())
 
@@ -63,15 +63,15 @@
     Args:
         text (str): Component YAML text.
 
     Returns:
         Component loaded from YAML.
     """
     return YamlComponent(
-        component_spec=structures.ComponentSpec.load_from_component_yaml(text),
+        component_spec=structures.ComponentSpec.from_yaml_documents(text),
         component_yaml=text)
 
 
 def load_component_from_file(file_path: str) -> YamlComponent:
     """Loads a component from a file.
 
     Args:
```

### Comparing `kfp-2.0.0b9/kfp/components/yaml_component_test.py` & `kfp-2.0.0rc1/kfp/components/yaml_component_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/__main__.py` & `kfp-2.0.0rc1/kfp/deprecated/__main__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/_auth.py` & `kfp-2.0.0rc1/kfp/deprecated/_auth.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/_client.py` & `kfp-2.0.0rc1/kfp/client/client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,158 +1,169 @@
-# Copyright 2018 The Kubeflow Authors
+# Copyright 2022 The Kubeflow Authors
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #      http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+"""The SDK client for Kubeflow Pipelines API."""
 
-import time
-import logging
+import copy
+import dataclasses
+import datetime
 import json
+import logging
 import os
 import re
 import tarfile
 import tempfile
+import time
+from types import ModuleType
+from typing import Any, Dict, List, Optional, TextIO
 import warnings
-import yaml
 import zipfile
-import datetime
-import copy
-from typing import Mapping, Callable, Optional
 
+from google.protobuf import json_format
+from kfp import compiler
+from kfp.client import auth
+from kfp.client import set_volume_credentials
+from kfp.components import base_component
+from kfp.pipeline_spec import pipeline_spec_pb2
 import kfp_server_api
-
-from kfp.deprecated import dsl
-from kfp.deprecated.compiler import compiler
-from kfp.deprecated.compiler._k8s_helper import sanitize_k8s_name
-
-from kfp.deprecated._auth import get_auth_token, get_gcp_access_token
-from kfp_server_api import ApiException
+import yaml
 
 # Operators on scalar values. Only applies to one of |int_value|,
 # |long_value|, |string_value| or |timestamp_value|.
 _FILTER_OPERATIONS = {
-    "UNKNOWN": 0,
-    "EQUALS": 1,
-    "NOT_EQUALS": 2,
-    "GREATER_THAN": 3,
-    "GREATER_THAN_EQUALS": 5,
-    "LESS_THAN": 6,
-    "LESS_THAN_EQUALS": 7
+    'EQUALS': 1,
+    'NOT_EQUALS': 2,
+    'GREATER_THAN': 3,
+    'GREATER_THAN_EQUALS': 5,
+    'LESS_THAN': 6,
+    'LESS_THAN_EQUALS': 7,
+    'IN': 8,
+    'IS_SUBSTRING': 9,
 }
 
+KF_PIPELINES_ENDPOINT_ENV = 'KF_PIPELINES_ENDPOINT'
+KF_PIPELINES_UI_ENDPOINT_ENV = 'KF_PIPELINES_UI_ENDPOINT'
+KF_PIPELINES_DEFAULT_EXPERIMENT_NAME = 'KF_PIPELINES_DEFAULT_EXPERIMENT_NAME'
+KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME = 'KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME'
+KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_IAP_OAUTH2_CLIENT_ID'
+KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_ID'
+KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET'
 
-def _add_generated_apis(target_struct, api_module, api_client):
-    """Initializes a hierarchical API object based on the generated API module.
 
-    PipelineServiceApi.create_pipeline becomes
-    target_struct.pipelines.create_pipeline
-    """
-    Struct = type('Struct', (), {})
+@dataclasses.dataclass
+class _PipelineDoc:
+    pipeline_spec: pipeline_spec_pb2.PipelineSpec
+    platform_spec: pipeline_spec_pb2.PlatformSpec
+
+    def to_dict(self) -> dict:
+        if self.platform_spec == pipeline_spec_pb2.PlatformSpec():
+            return json_format.MessageToDict(self.pipeline_spec)
+        else:
+            return {
+                'pipeline_spec': json_format.MessageToDict(self.pipeline_spec),
+                'platform_spec': json_format.MessageToDict(self.platform_spec),
+            }
 
-    def camel_case_to_snake_case(name):
-        import re
-        return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
 
-    for api_name in dir(api_module):
-        if not api_name.endswith('ServiceApi'):
-            continue
+@dataclasses.dataclass
+class _JobConfig:
+    pipeline_spec: dict
+    pipeline_version_reference: kfp_server_api.V2beta1PipelineVersionReference
+    runtime_config: kfp_server_api.V2beta1RuntimeConfig
 
-        short_api_name = camel_case_to_snake_case(
-            api_name[0:-len('ServiceApi')]) + 's'
-        api_struct = Struct()
-        setattr(target_struct, short_api_name, api_struct)
-        service_api = getattr(api_module.api, api_name)
-        initialized_service_api = service_api(api_client)
-        for member_name in dir(initialized_service_api):
-            if member_name.startswith('_') or member_name.endswith(
-                    '_with_http_info'):
-                continue
 
-            bound_member = getattr(initialized_service_api, member_name)
-            setattr(api_struct, member_name, bound_member)
-    models_struct = Struct()
-    for member_name in dir(api_module.models):
-        if not member_name[0].islower():
-            setattr(models_struct, member_name,
-                    getattr(api_module.models, member_name))
-    target_struct.api_models = models_struct
+class RunPipelineResult:
 
+    def __init__(self, client: 'Client',
+                 run_info: kfp_server_api.V2beta1Run) -> None:
+        self._client = client
+        self.run_info = run_info
+        self.run_id = run_info.run_id
 
-KF_PIPELINES_ENDPOINT_ENV = 'KF_PIPELINES_ENDPOINT'
-KF_PIPELINES_UI_ENDPOINT_ENV = 'KF_PIPELINES_UI_ENDPOINT'
-KF_PIPELINES_DEFAULT_EXPERIMENT_NAME = 'KF_PIPELINES_DEFAULT_EXPERIMENT_NAME'
-KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME = 'KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME'
-KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_IAP_OAUTH2_CLIENT_ID'
-KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_ID'
-KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET_ENV = 'KF_PIPELINES_APP_OAUTH2_CLIENT_SECRET'
+    def wait_for_run_completion(self, timeout=None):
+        timeout = timeout or datetime.timedelta.max
+        return self._client.wait_for_run_completion(self.run_id, timeout)
 
+    def __repr__(self):
+        return f'RunPipelineResult(run_id={self.run_id})'
 
-class Client(object):
-    """API Client for KubeFlow Pipeline.
+
+class Client:
+    """The KFP SDK client for the Kubeflow Pipelines backend API.
 
     Args:
-      host: The host name to use to talk to Kubeflow Pipelines. If not set, the in-cluster
-          service DNS name will be used, which only works if the current environment is a pod
-          in the same cluster (such as a Jupyter instance spawned by Kubeflow's
-          JupyterHub).
-          Set the host based on https://www.kubeflow.org/docs/components/pipelines/sdk/connect-api/.
-      client_id: The client ID used by Identity-Aware Proxy.
-      namespace: The namespace where the kubeflow pipeline system is run.
-      other_client_id: The client ID used to obtain the auth codes and refresh tokens.
-          Reference: https://cloud.google.com/iap/docs/authentication-howto#authenticating_from_a_desktop_app.
-      other_client_secret: The client secret used to obtain the auth codes and refresh tokens.
-      existing_token: Pass in token directly, it's used for cases better get token outside of SDK, e.x. GCP Cloud Functions
-          or caller already has a token
-      cookies: CookieJar object containing cookies that will be passed to the pipelines API.
-      proxy: HTTP or HTTPS proxy server
-      ssl_ca_cert: Cert for proxy
-      kube_context: String name of context within kubeconfig to use, defaults to the current-context set within kubeconfig.
-      credentials: A TokenCredentialsBase object which provides the logic to
-          populate the requests with credentials to authenticate against the API
-          server.
-      ui_host: Base url to use to open the Kubeflow Pipelines UI. This is used when running the client from a notebook to generate and
-          print links.
-      verify_ssl: A boolean indication to verify the servers TLS certificate or not.
+        host: Host name to use to talk to Kubeflow Pipelines. If not set,
+            the in-cluster service DNS name will be used, which only works if
+            the current environment is a pod in the same cluster (such as a
+            Jupyter instance spawned by Kubeflow's JupyterHub). (`More information on connecting. <https://www.kubeflow.org/docs/components/pipelines/sdk/connect-api/>`_)
+        client_id: Client ID used by Identity-Aware Proxy.
+        namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+        other_client_id: Client ID used to obtain the auth codes and refresh
+            tokens (`reference <https://cloud.google.com/iap/docs/authentication-howto#authenticating_from_a_desktop_app>`_).
+        other_client_secret: Client secret used to obtain the auth codes and
+            refresh tokens.
+        existing_token: Authentication token to pass in directly. Used in cases where the token is
+            generated from outside the SDK.
+        cookies: CookieJar object containing cookies that will be passed to the
+            Pipelines API.
+        proxy: HTTP or HTTPS proxy server.
+        ssl_ca_cert: Certification for proxy.
+        kube_context: kubectl context to use. Must be a context listed in the kubeconfig file. Defaults to the current-context set within kubeconfig.
+        credentials: ``TokenCredentialsBase`` object which provides the logic to
+            populate the requests with credentials to authenticate against the
+            API server.
+        ui_host: Base URL to use to open the Kubeflow Pipelines UI. This is used
+            when running the client from a notebook to generate and print links.
+        verify_ssl: Whether to verify the server's TLS certificate.
     """
 
     # in-cluster DNS name of the pipeline service
-    IN_CLUSTER_DNS_NAME = 'ml-pipeline.{}.svc.cluster.local:8888'
-    KUBE_PROXY_PATH = 'api/v1/namespaces/{}/services/ml-pipeline:http/proxy/'
+    _IN_CLUSTER_DNS_NAME = 'ml-pipeline.{}.svc.cluster.local:8888'
+    _KUBE_PROXY_PATH = 'api/v1/namespaces/{}/services/ml-pipeline:http/proxy/'
 
     # Auto populated path in pods
     # https://kubernetes.io/docs/tasks/access-application-cluster/access-cluster/#accessing-the-api-from-a-pod
     # https://kubernetes.io/docs/reference/access-authn-authz/service-accounts-admin/#serviceaccount-admission-controller
-    NAMESPACE_PATH = '/var/run/secrets/kubernetes.io/serviceaccount/namespace'
+    _NAMESPACE_PATH = '/var/run/secrets/kubernetes.io/serviceaccount/namespace'
 
-    LOCAL_KFP_CONTEXT = os.path.expanduser('~/.config/kfp/context.json')
+    _LOCAL_KFP_CONTEXT = os.path.expanduser('~/.config/kfp/context.json')
 
     # TODO: Wrap the configurations for different authentication methods.
-    def __init__(self,
-                 host=None,
-                 client_id=None,
-                 namespace='kubeflow',
-                 other_client_id=None,
-                 other_client_secret=None,
-                 existing_token=None,
-                 cookies=None,
-                 proxy=None,
-                 ssl_ca_cert=None,
-                 kube_context=None,
-                 credentials=None,
-                 ui_host=None,
-                 verify_ssl=None):
+    def __init__(
+        self,
+        host: Optional[str] = None,
+        client_id: Optional[str] = None,
+        namespace: str = 'kubeflow',
+        other_client_id: Optional[str] = None,
+        other_client_secret: Optional[str] = None,
+        existing_token: Optional[str] = None,
+        cookies: Optional[str] = None,
+        proxy: Optional[str] = None,
+        ssl_ca_cert: Optional[str] = None,
+        kube_context: Optional[str] = None,
+        credentials: Optional[str] = None,
+        ui_host: Optional[str] = None,
+        verify_ssl: Optional[bool] = None,
+    ) -> None:
         """Create a new instance of kfp client."""
+        warnings.warn(
+            'This client only works with Kubeflow Pipeline v2.0.0-beta.2 '
+            'and later versions.',
+            category=FutureWarning)
+
         host = host or os.environ.get(KF_PIPELINES_ENDPOINT_ENV)
         self._uihost = os.environ.get(KF_PIPELINES_UI_ENDPOINT_ENV, ui_host or
                                       host)
         client_id = client_id or os.environ.get(
             KF_PIPELINES_IAP_OAUTH2_CLIENT_ID_ENV)
         other_client_id = other_client_id or os.environ.get(
             KF_PIPELINES_APP_OAUTH2_CLIENT_ID_ENV)
@@ -170,48 +181,54 @@
         # context settings for current client instance
         if namespace != 'kubeflow':
             self._context_setting['namespace'] = namespace
 
         self._existing_config = config
         if cookies is None:
             cookies = self._context_setting.get('client_authentication_cookie')
-        api_client = kfp_server_api.api_client.ApiClient(
+        api_client = kfp_server_api.ApiClient(
             config,
             cookie=cookies,
             header_name=self._context_setting.get(
                 'client_authentication_header_name'),
             header_value=self._context_setting.get(
                 'client_authentication_header_value'))
         _add_generated_apis(self, kfp_server_api, api_client)
-        self._job_api = kfp_server_api.api.job_service_api.JobServiceApi(
-            api_client)
-        self._run_api = kfp_server_api.api.run_service_api.RunServiceApi(
-            api_client)
-        self._experiment_api = kfp_server_api.api.experiment_service_api.ExperimentServiceApi(
-            api_client)
-        self._pipelines_api = kfp_server_api.api.pipeline_service_api.PipelineServiceApi(
-            api_client)
-        self._upload_api = kfp_server_api.api.PipelineUploadServiceApi(
-            api_client)
-        self._healthz_api = kfp_server_api.api.healthz_service_api.HealthzServiceApi(
+        self._recurring_run_api = kfp_server_api.RecurringRunServiceApi(
             api_client)
+        self._run_api = kfp_server_api.RunServiceApi(api_client)
+        self._experiment_api = kfp_server_api.ExperimentServiceApi(api_client)
+        self._pipelines_api = kfp_server_api.PipelineServiceApi(api_client)
+        self._upload_api = kfp_server_api.PipelineUploadServiceApi(api_client)
+        self._healthz_api = kfp_server_api.HealthzServiceApi(api_client)
         if not self._context_setting['namespace'] and self.get_kfp_healthz(
         ).multi_user is True:
             try:
-                with open(Client.NAMESPACE_PATH, 'r') as f:
+                with open(Client._NAMESPACE_PATH, 'r') as f:
                     current_namespace = f.read()
                     self.set_user_namespace(current_namespace)
             except FileNotFoundError:
                 logging.info(
                     'Failed to automatically set namespace.', exc_info=False)
 
-    def _load_config(self, host, client_id, namespace, other_client_id,
-                     other_client_secret, existing_token, proxy, ssl_ca_cert,
-                     kube_context, credentials, verify_ssl):
-        config = kfp_server_api.configuration.Configuration()
+    def _load_config(
+        self,
+        host: Optional[str],
+        client_id: Optional[str],
+        namespace: str,
+        other_client_id: Optional[str],
+        other_client_secret: Optional[str],
+        existing_token: Optional[str],
+        proxy: Optional[str],
+        ssl_ca_cert: Optional[str],
+        kube_context: Optional[str],
+        credentials: Optional[str],
+        verify_ssl: Optional[bool],
+    ) -> kfp_server_api.Configuration:
+        config = kfp_server_api.Configuration()
 
         if proxy:
             # https://github.com/kubeflow/pipelines/blob/c6ac5e0b1fd991e19e96419f0f508ec0a4217c29/backend/api/python_http_client/kfp_server_api/rest.py#L100
             config.proxy = proxy
         if verify_ssl is not None:
             config.verify_ssl = verify_ssl
 
@@ -219,33 +236,35 @@
             config.ssl_ca_cert = ssl_ca_cert
 
         host = host or ''
 
         # Defaults to 'https' if host does not contain 'http' or 'https' protocol.
         if host and not host.startswith('http'):
             warnings.warn(
-                'The host %s does not contain the "http" or "https" protocol.'
-                ' Defaults to "https".' % host)
+                f'The host {host} does not contain the "http" or "https" protocol. Defaults to "https".'
+            )
             host = 'https://' + host
 
         # Preprocess the host endpoint to prevent some common user mistakes.
         if not client_id:
             # always preserving the protocol (http://localhost requires it)
             host = host.rstrip('/')
 
         if host:
             config.host = host
 
         token = None
 
-        # "existing_token" is designed to accept token generated outside of SDK. Here is an example.
+        # "existing_token" is designed to accept token generated outside of SDK.
         #
         # https://cloud.google.com/functions/docs/securing/function-identity
         # https://cloud.google.com/endpoints/docs/grpc/service-account-authentication
         #
+        # Here is an example.
+        #
         # import requests
         # import kfp
         #
         # def get_access_token():
         #     url = 'http://metadata.google.internal/computeMetadata/v1/instance/service-accounts/default/token'
         #     r = requests.get(url, headers={'Metadata-Flavor': 'Google'})
         #     r.raise_for_status()
@@ -254,543 +273,533 @@
         #
         # client = kfp.Client(host='<KFPHost>', existing_token=get_access_token())
         #
         if existing_token:
             token = existing_token
             self._is_refresh_token = False
         elif client_id:
-            token = get_auth_token(client_id, other_client_id,
-                                   other_client_secret)
-            self._is_refresh_token = True
+            token, self._is_refresh_token = auth.get_auth_token(
+                client_id, other_client_id, other_client_secret)
         elif self._is_inverse_proxy_host(host):
-            token = get_gcp_access_token()
+            token = auth.get_gcp_access_token()
             self._is_refresh_token = False
         elif credentials:
             config.api_key['authorization'] = 'placeholder'
             config.api_key_prefix['authorization'] = 'Bearer'
             config.refresh_api_key_hook = credentials.refresh_api_key_hook
 
         if token:
             config.api_key['authorization'] = token
             config.api_key_prefix['authorization'] = 'Bearer'
             return config
 
         if host:
-            # if host is explicitly set with auth token, it's probably a port forward address.
+            # if host is explicitly set with auth token, it's probably a port
+            # forward address.
             return config
 
         import kubernetes as k8s
         in_cluster = True
         try:
             k8s.config.load_incluster_config()
         except:
             in_cluster = False
 
         if in_cluster:
-            config.host = Client.IN_CLUSTER_DNS_NAME.format(namespace)
+            config.host = Client._IN_CLUSTER_DNS_NAME.format(namespace)
             config = self._get_config_with_default_credentials(config)
             return config
 
         try:
             k8s.config.load_kube_config(
                 client_configuration=config, context=kube_context)
         except:
             print('Failed to load kube config.')
             return config
 
         if config.host:
-            config.host = config.host + '/' + Client.KUBE_PROXY_PATH.format(
+            config.host = config.host + '/' + Client._KUBE_PROXY_PATH.format(
                 namespace)
         return config
 
-    def _is_inverse_proxy_host(self, host):
-        if host:
-            return re.match(r'\S+.googleusercontent.com/{0,1}$', host)
-        if re.match(r'\w+', host):
-            warnings.warn(
-                'The received host is %s, please include the full endpoint address '
-                '(with ".(pipelines/notebooks).googleusercontent.com")' % host)
-        return False
+    def _is_inverse_proxy_host(self, host: str) -> bool:
+        return bool(re.match(r'\S+.googleusercontent.com/{0,1}$', host))
 
-    def _is_ipython(self):
+    def _is_ipython(self) -> bool:
         """Returns whether we are running in notebook."""
         try:
             import IPython
             ipy = IPython.get_ipython()
             if ipy is None:
                 return False
         except ImportError:
             return False
 
         return True
 
-    def _get_url_prefix(self):
+    def _get_url_prefix(self) -> str:
         if self._uihost:
             # User's own connection.
             if self._uihost.startswith('http://') or self._uihost.startswith(
                     'https://'):
                 return self._uihost
             else:
                 return 'http://' + self._uihost
 
         # In-cluster pod. We could use relative URL.
         return '/pipeline'
 
-    def _load_context_setting_or_default(self):
-        if os.path.exists(Client.LOCAL_KFP_CONTEXT):
-            with open(Client.LOCAL_KFP_CONTEXT, 'r') as f:
+    def _load_context_setting_or_default(self) -> None:
+        if os.path.exists(Client._LOCAL_KFP_CONTEXT):
+            with open(Client._LOCAL_KFP_CONTEXT, 'r') as f:
                 self._context_setting = json.load(f)
         else:
             self._context_setting = {
                 'namespace': '',
             }
 
-    def _refresh_api_client_token(self):
+    def _refresh_api_client_token(self) -> None:
         """Refreshes the existing token associated with the kfp_api_client."""
         if getattr(self, '_is_refresh_token', None):
             return
 
-        new_token = get_gcp_access_token()
+        new_token = auth.get_gcp_access_token()
         self._existing_config.api_key['authorization'] = new_token
 
-    def _get_config_with_default_credentials(self, config):
+    def _get_config_with_default_credentials(
+            self, config: kfp_server_api.Configuration
+    ) -> kfp_server_api.Configuration:
         """Apply default credentials to the configuration object.
 
         This method accepts a Configuration object and extends it with
         some default credentials interface.
         """
         # XXX: The default credentials are audience-based service account tokens
         # projected by the kubelet (ServiceAccountTokenVolumeCredentials). As we
         # implement more and more credentials, we can have some heuristic and
         # choose from a number of options.
         # See https://github.com/kubeflow/pipelines/pull/5287#issuecomment-805654121
-        from kfp.deprecated import auth
-        credentials = auth.ServiceAccountTokenVolumeCredentials()
+        credentials = set_volume_credentials.ServiceAccountTokenVolumeCredentials(
+        )
         config_copy = copy.deepcopy(config)
 
         try:
             credentials.refresh_api_key_hook(config_copy)
         except Exception:
-            logging.warning("Failed to set up default credentials. Proceeding"
-                            " without credentials...")
+            logging.warning('Failed to set up default credentials. Proceeding'
+                            ' without credentials...')
             return config
 
         config.refresh_api_key_hook = credentials.refresh_api_key_hook
         config.api_key_prefix['authorization'] = 'Bearer'
         config.refresh_api_key_hook(config)
         return config
 
-    def set_user_namespace(self, namespace: str):
-        """Set user namespace into local context setting file.
+    def set_user_namespace(self, namespace: str) -> None:
+        """Sets the namespace in the Kuberenetes cluster to use.
 
-        This function should only be used when Kubeflow Pipelines is in the multi-user mode.
+        This function should only be used when Kubeflow Pipelines is in the
+        multi-user mode.
 
         Args:
-          namespace: kubernetes namespace the user has access to.
+            namespace: Namespace to use within the Kubernetes cluster (namespace containing the Kubeflow Pipelines deployment).
         """
         self._context_setting['namespace'] = namespace
-        if not os.path.exists(os.path.dirname(Client.LOCAL_KFP_CONTEXT)):
-            os.makedirs(os.path.dirname(Client.LOCAL_KFP_CONTEXT))
-        with open(Client.LOCAL_KFP_CONTEXT, 'w') as f:
+        if not os.path.exists(os.path.dirname(Client._LOCAL_KFP_CONTEXT)):
+            os.makedirs(os.path.dirname(Client._LOCAL_KFP_CONTEXT))
+        with open(Client._LOCAL_KFP_CONTEXT, 'w') as f:
             json.dump(self._context_setting, f)
 
-    def get_kfp_healthz(self) -> kfp_server_api.ApiGetHealthzResponse:
-        """Gets healthz info of KFP deployment.
+    def get_kfp_healthz(
+        self,
+        sleep_duration: int = 5,
+    ) -> kfp_server_api.V2beta1GetHealthzResponse:
+        """Gets healthz info for KFP deployment.
+
+        Args:
+            sleep_duration: Time in seconds between retries.
 
         Returns:
-          response: json formatted response from the healtz endpoint.
+            JSON response from the healthz endpoint.
         """
         count = 0
         response = None
         max_attempts = 5
         while not response:
             count += 1
             if count > max_attempts:
                 raise TimeoutError(
-                    'Failed getting healthz endpoint after {} attempts.'.format(
-                        max_attempts))
+                    f'Failed getting healthz endpoint after {max_attempts} attempts.'
+                )
+
             try:
-                response = self._healthz_api.get_healthz()
-                return response
+                return self._healthz_api.get_healthz()
             # ApiException, including network errors, is the only type that may
             # recover after retry.
             except kfp_server_api.ApiException:
                 # logging.exception also logs detailed info about the ApiException
                 logging.exception(
-                    'Failed to get healthz info attempt {} of 5.'.format(count))
-                time.sleep(5)
+                    f'Failed to get healthz info attempt {count} of {max_attempts}.'
+                )
+                time.sleep(sleep_duration)
 
     def get_user_namespace(self) -> str:
-        """Get user namespace in context config.
+        """Gets user namespace in context config.
 
         Returns:
-          namespace: kubernetes namespace from the local context file or empty if it wasn't set.
+            Kubernetes namespace from the local context file or empty if it
+            wasn't set.
         """
         return self._context_setting['namespace']
 
     def create_experiment(
-            self,
-            name: str,
-            description: str = None,
-            namespace: str = None) -> kfp_server_api.ApiExperiment:
-        """Create a new experiment.
+        self,
+        name: str,
+        description: str = None,
+        namespace: str = None,
+    ) -> kfp_server_api.V2beta1Experiment:
+        """Creates a new experiment.
 
         Args:
-          name: The name of the experiment.
-          description: Description of the experiment.
-          namespace: Kubernetes namespace where the experiment should be created.
-            For single user deployment, leave it as None;
-            For multi user, input a namespace where the user is authorized.
+            name: Name of the experiment.
+            description: Description of the experiment.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
 
         Returns:
-          An Experiment object. Most important field is id.
+            ``V2beta1Experiment`` object.
         """
         namespace = namespace or self.get_user_namespace()
         experiment = None
         try:
             experiment = self.get_experiment(
                 experiment_name=name, namespace=namespace)
         except ValueError as error:
             # Ignore error if the experiment does not exist.
             if not str(error).startswith('No experiment is found with name'):
                 raise error
 
         if not experiment:
-            logging.info('Creating experiment {}.'.format(name))
+            logging.info(f'Creating experiment {name}.')
 
-            resource_references = []
-            if namespace:
-                key = kfp_server_api.models.ApiResourceKey(
-                    id=namespace,
-                    type=kfp_server_api.models.ApiResourceType.NAMESPACE)
-                reference = kfp_server_api.models.ApiResourceReference(
-                    key=key,
-                    relationship=kfp_server_api.models.ApiRelationship.OWNER)
-                resource_references.append(reference)
-
-            experiment = kfp_server_api.models.ApiExperiment(
-                name=name,
+            experiment = kfp_server_api.V2beta1Experiment(
+                display_name=name,
                 description=description,
-                resource_references=resource_references)
-            experiment = self._experiment_api.create_experiment_v1(
-                body=experiment)
+                namespace=namespace,
+            )
+            experiment = self._experiment_api.create_experiment(body=experiment)
 
+        link = f'{self._get_url_prefix()}/#/experiments/details/{experiment.experiment_id}'
         if self._is_ipython():
             import IPython
-            html = \
-                ('<a href="%s/#/experiments/details/%s" target="_blank" >Experiment details</a>.'
-                % (self._get_url_prefix(), experiment.id))
+            html = f'<a href="{link}" target="_blank" >Experiment details</a>.'
             IPython.display.display(IPython.display.HTML(html))
+        else:
+            print(f'Experiment details: {link}')
+
         return experiment
 
-    def get_pipeline_id(self, name) -> Optional[str]:
-        """Find the id of a pipeline by name.
+    def get_pipeline_id(self, name: str) -> Optional[str]:
+        """Gets the ID of a pipeline by its name.
 
         Args:
-          name: Pipeline name.
+            name: Pipeline name.
 
         Returns:
-          Returns the pipeline id if a pipeline with the name exists.
+            The pipeline ID if a pipeline with the name exists.
         """
         pipeline_filter = json.dumps({
-            "predicates": [{
-                "op": _FILTER_OPERATIONS["EQUALS"],
-                "key": "name",
-                "stringValue": name,
+            'predicates': [{
+                'operation': _FILTER_OPERATIONS['EQUALS'],
+                'key': 'display_name',
+                'stringValue': name,
             }]
         })
-        result = self._pipelines_api.list_pipelines_v1(filter=pipeline_filter)
+        result = self._pipelines_api.list_pipelines(filter=pipeline_filter)
         if result.pipelines is None:
             return None
         if len(result.pipelines) == 1:
-            return result.pipelines[0].id
+            return result.pipelines[0].pipeline_id
         elif len(result.pipelines) > 1:
             raise ValueError(
-                "Multiple pipelines with the name: {} found, the name needs to be unique"
-                .format(name))
+                f'Multiple pipelines with the name: {name} found, the name needs to be unique.'
+            )
         return None
 
     def list_experiments(
         self,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
         namespace: Optional[str] = None,
-        filter: Optional[str] = None
-    ) -> kfp_server_api.ApiListExperimentsResponse:
-        """List experiments.
-
-        Args:
-          page_token: Token for starting of the page.
-          page_size: Size of the page.
-          sort_by: Can be '[field_name]', '[field_name] desc'. For example, 'name desc'.
-          namespace: Kubernetes namespace where the experiment was created.
-            For single user deployment, leave it as None;
-            For multi user, input a namespace where the user is authorized.
-          filter: A url-encoded, JSON-serialized Filter protocol buffer
-            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
-
-            An example filter string would be:
-
-                # For the list of filter operations please see:
-                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
-                json.dumps({
-                    "predicates": [{
-                        "op": _FILTER_OPERATIONS["EQUALS"],
-                        "key": "name",
-                        "stringValue": "my-name",
-                    }]
-                })
+        filter: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1ListExperimentsResponse:
+        """Lists experiments.
+
+        Args:
+            page_token: Page token for obtaining page from paginated response.
+            page_size: Size of the page.
+            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'display_name desc'``.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+            filter: A url-encoded, JSON-serialized Filter protocol buffer
+                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/cb7d9a87c999eb1d2280959e5afbeee9e270ef3d/backend/api/v2beta1/filter.proto>`_). Example:
+
+                  ::
+
+                    json.dumps({
+                        "predicates": [{
+                            "operation": "EQUALS",
+                            "key": "display_name",
+                            "stringValue": "my-name",
+                        }]
+                    })
 
         Returns:
-          A response object including a list of experiments and next page token.
+            ``V2beta1ListExperimentsResponse`` object.
         """
         namespace = namespace or self.get_user_namespace()
-        response = self._experiment_api.list_experiments_v1(
+        return self._experiment_api.list_experiments(
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
-            resource_reference_key_type=kfp_server_api.models.api_resource_type
-            .ApiResourceType.NAMESPACE,
-            resource_reference_key_id=namespace,
-            filter=filter)
-        return response
+            filter=filter,
+            namespace=namespace,
+        )
 
-    def get_experiment(self,
-                       experiment_id=None,
-                       experiment_name=None,
-                       namespace=None) -> kfp_server_api.ApiExperiment:
-        """Get details of an experiment.
+    def get_experiment(
+        self,
+        experiment_id: Optional[str] = None,
+        experiment_name: Optional[str] = None,
+        namespace: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1Experiment:
+        """Gets details of an experiment.
 
-        Either experiment_id or experiment_name is required
+        Either ``experiment_id`` or ``experiment_name`` is required.
 
         Args:
-          experiment_id: Id of the experiment. (Optional)
-          experiment_name: Name of the experiment. (Optional)
-          namespace: Kubernetes namespace where the experiment was created.
-            For single user deployment, leave it as None;
-            For multi user, input the namespace where the user is authorized.
+            experiment_id: ID of the experiment.
+            experiment_name: Name of the experiment.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments.
+                For single-user deployments, this should be left as ``None``.
 
         Returns:
-          A response object including details of a experiment.
-
-        Raises:
-          kfp_server_api.ApiException: If experiment is not found or None of the arguments is provided
+            ``V2beta1Experiment`` object.
         """
         namespace = namespace or self.get_user_namespace()
         if experiment_id is None and experiment_name is None:
             raise ValueError(
-                'Either experiment_id or experiment_name is required')
+                'Either experiment_id or experiment_name is required.')
         if experiment_id is not None:
-            return self._experiment_api.get_experiment_v1(id=experiment_id)
+            return self._experiment_api.get_experiment(
+                experiment_id=experiment_id)
         experiment_filter = json.dumps({
-            "predicates": [{
-                "op": _FILTER_OPERATIONS["EQUALS"],
-                "key": "name",
-                "stringValue": experiment_name,
+            'predicates': [{
+                'operation': _FILTER_OPERATIONS['EQUALS'],
+                'key': 'display_name',
+                'stringValue': experiment_name,
             }]
         })
-        if namespace:
-            result = self._experiment_api.list_experiments_v1(
-                filter=experiment_filter,
-                resource_reference_key_type=kfp_server_api.models
-                .api_resource_type.ApiResourceType.NAMESPACE,
-                resource_reference_key_id=namespace)
+        if namespace is not None:
+            result = self._experiment_api.list_experiments(
+                filter=experiment_filter, namespace=namespace)
         else:
-            result = self._experiment_api.list_experiments_v1(
+            result = self._experiment_api.list_experiments(
                 filter=experiment_filter)
         if not result.experiments:
             raise ValueError(
-                'No experiment is found with name {}.'.format(experiment_name))
+                f'No experiment is found with name {experiment_name}.')
         if len(result.experiments) > 1:
             raise ValueError(
-                'Multiple experiments is found with name {}.'.format(
-                    experiment_name))
+                f'Multiple experiments is found with name {experiment_name}.')
         return result.experiments[0]
 
-    def archive_experiment(self, experiment_id: str):
-        """Archive experiment.
+    def archive_experiment(self, experiment_id: str) -> dict:
+        """Archives an experiment.
 
         Args:
-          experiment_id: id of the experiment.
+            experiment_id: ID of the experiment.
 
-        Raises:
-          kfp_server_api.ApiException: If experiment is not found.
+        Returns:
+            Empty dictionary.
         """
-        self._experiment_api.archive_experiment_v1(experiment_id)
+        return self._experiment_api.archive_experiment(
+            experiment_id=experiment_id)
 
-    def delete_experiment(self, experiment_id):
-        """Delete experiment.
+    def unarchive_experiment(self, experiment_id: str) -> dict:
+        """Unarchives an experiment.
 
         Args:
-          experiment_id: id of the experiment.
+            experiment_id: ID of the experiment.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
-
-        Raises:
-          kfp_server_api.ApiException: If experiment is not found.
+            Empty dictionary.
         """
-        return self._experiment_api.delete_experiment_v1(id=experiment_id)
-
-    def _extract_pipeline_yaml(self, package_file):
+        return self._experiment_api.unarchive_experiment(
+            experiment_id=experiment_id)
 
-        def _choose_pipeline_yaml_file(file_list) -> str:
-            yaml_files = [file for file in file_list if file.endswith('.yaml')]
-            if len(yaml_files) == 0:
-                raise ValueError(
-                    'Invalid package. Missing pipeline yaml file in the package.'
-                )
-
-            if 'pipeline.yaml' in yaml_files:
-                return 'pipeline.yaml'
-            else:
-                if len(yaml_files) == 1:
-                    return yaml_files[0]
-                raise ValueError(
-                    'Invalid package. There is no pipeline.yaml file and there are multiple yaml files.'
-                )
+    def delete_experiment(self, experiment_id: str) -> dict:
+        """Delete experiment.
 
-        if package_file.endswith('.tar.gz') or package_file.endswith('.tgz'):
-            with tarfile.open(package_file, "r:gz") as tar:
-                file_names = [member.name for member in tar if member.isfile()]
-                pipeline_yaml_file = _choose_pipeline_yaml_file(file_names)
-                with tar.extractfile(tar.getmember(pipeline_yaml_file)) as f:
-                    return yaml.safe_load(f)
-        elif package_file.endswith('.zip'):
-            with zipfile.ZipFile(package_file, 'r') as zip:
-                pipeline_yaml_file = _choose_pipeline_yaml_file(zip.namelist())
-                with zip.open(pipeline_yaml_file) as f:
-                    return yaml.safe_load(f)
-        elif package_file.endswith('.yaml') or package_file.endswith('.yml'):
-            with open(package_file, 'r') as f:
-                return yaml.safe_load(f)
-        else:
-            raise ValueError(
-                'The package_file ' + package_file +
-                ' should end with one of the following formats: [.tar.gz, .tgz, .zip, .yaml, .yml]'
-            )
+        Args:
+            experiment_id: ID of the experiment.
 
-    def _override_caching_options(self, workflow: dict, enable_caching: bool):
-        templates = workflow['spec']['templates']
-        for template in templates:
-            if 'metadata' in template \
-               and 'labels' in template['metadata'] \
-               and 'pipelines.kubeflow.org/enable_caching' in template['metadata']['labels']:
-                template['metadata']['labels'][
-                    'pipelines.kubeflow.org/enable_caching'] = str(
-                        enable_caching).lower()
+        Returns:
+            Empty dictionary.
+        """
+        return self._experiment_api.delete_experiment(
+            experiment_id=experiment_id)
 
     def list_pipelines(
         self,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
-        filter: Optional[str] = None
-    ) -> kfp_server_api.ApiListPipelinesResponse:
-        """List pipelines.
+        filter: Optional[str] = None,
+        namespace: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1ListPipelinesResponse:
+        """Lists pipelines.
 
         Args:
-          page_token: Token for starting of the page.
-          page_size: Size of the page.
-          sort_by: one of 'field_name', 'field_name desc'. For example, 'name desc'.
-          filter: A url-encoded, JSON-serialized Filter protocol buffer
-            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+            page_token: Page token for obtaining page from paginated response.
+            page_size: Size of the page.
+            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'display_name desc'``.
+            filter: A url-encoded, JSON-serialized Filter protocol buffer
+                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/cb7d9a87c999eb1d2280959e5afbeee9e270ef3d/backend/api/v2beta1/filter.proto>`_). Example:
 
-            An example filter string would be:
+                  ::
 
-                # For the list of filter operations please see:
-                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
-                json.dumps({
-                    "predicates": [{
-                        "op": _FILTER_OPERATIONS["EQUALS"],
-                        "key": "name",
-                        "stringValue": "my-name",
-                    }]
-                })
+                    json.dumps({
+                        "predicates": [{
+                            "operation": "EQUALS",
+                            "key": "display_name",
+                            "stringValue": "my-name",
+                        }]
+                    })
 
         Returns:
-          A response object including a list of pipelines and next page token.
+            ``V2beta1ListPipelinesResponse`` object.
         """
-        return self._pipelines_api.list_pipelines_v1(
+        return self._pipelines_api.list_pipelines(
+            namespace=namespace,
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
             filter=filter)
 
     # TODO: provide default namespace, similar to kubectl default namespaces.
     def run_pipeline(
         self,
         experiment_id: str,
         job_name: str,
         pipeline_package_path: Optional[str] = None,
-        params: Optional[dict] = None,
+        params: Optional[Dict[str, Any]] = None,
         pipeline_id: Optional[str] = None,
         version_id: Optional[str] = None,
         pipeline_root: Optional[str] = None,
-        enable_caching: Optional[str] = None,
+        enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ) -> kfp_server_api.ApiRun:
-        """Run a specified pipeline.
+    ) -> kfp_server_api.V2beta1Run:
+        """Runs a specified pipeline.
 
         Args:
-          experiment_id: The id of an experiment.
-          job_name: Name of the job.
-          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
-          params: A dictionary with key (string) as param name and value (string) as as param value.
-          pipeline_id: The id of a pipeline.
-          version_id: The id of a pipeline version.
-            If both pipeline_id and version_id are specified, version_id will take precendence.
-            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
-          pipeline_root: The root path of the pipeline outputs. This argument should
-            be used only for pipeline compiled with
-            dsl.PipelineExecutionMode.V2_COMPATIBLE or
-            dsl.PipelineExecutionMode.V2_ENGINGE mode.
-          enable_caching: Optional. Whether or not to enable caching for the run.
-            This setting affects v2 compatible mode and v2 mode only.
-            If not set, defaults to the compile time settings, which are True for all
-            tasks by default, while users may specify different caching options for
-            individual tasks.
-            If set, the setting applies to all tasks in the pipeline -- overrides
-            the compile time settings.
-          service_account: Optional. Specifies which Kubernetes service account this
-            run uses.
+            experiment_id: ID of an experiment.
+            job_name: Name of the job.
+            pipeline_package_path: Local path of the pipeline package (the
+                filename should end with one of the following .tar.gz, .tgz,
+                .zip, .json).
+            params: Arguments to the pipeline function provided as a dict.
+            pipeline_id: ID of the pipeline.
+            version_id: ID of the pipeline version to run.
+                If both pipeline_id and version_id are specified, version_id
+                will take precendence.
+                If only pipeline_id is specified, the default version of this
+                pipeline is used to create the run.
+            pipeline_root: Root path of the pipeline outputs.
+            enable_caching: Whether or not to enable caching for the
+                run. If not set, defaults to the compile-time settings, which
+                is ``True`` for all tasks by default. If set, the
+                setting applies to all tasks in the pipeline (overrides the
+                compile time settings).
+            service_account: Specifies which Kubernetes service
+                account to use for this run.
 
         Returns:
-          A run object. Most important field is id.
+            ``V2beta1Run`` object.
         """
-        if params is None:
-            params = {}
-
-        if pipeline_root is not None:
-            params[dsl.ROOT_PARAMETER_NAME] = pipeline_root
-
         job_config = self._create_job_config(
-            experiment_id=experiment_id,
             params=params,
             pipeline_package_path=pipeline_package_path,
             pipeline_id=pipeline_id,
             version_id=version_id,
             enable_caching=enable_caching,
+            pipeline_root=pipeline_root,
         )
-        run_body = kfp_server_api.models.ApiRun(
-            pipeline_spec=job_config.spec,
-            resource_references=job_config.resource_references,
-            name=job_name,
+
+        run_body = kfp_server_api.V2beta1Run(
+            experiment_id=experiment_id,
+            display_name=job_name,
+            pipeline_spec=job_config.pipeline_spec,
+            pipeline_version_reference=job_config.pipeline_version_reference,
+            runtime_config=job_config.runtime_config,
             service_account=service_account)
 
-        response = self._run_api.create_run_v1(body=run_body)
+        response = self._run_api.create_run(body=run_body)
 
+        link = f'{self._get_url_prefix()}/#/runs/details/{response.run_id}'
         if self._is_ipython():
             import IPython
-            html = (
-                '<a href="%s/#/runs/details/%s" target="_blank" >Run details</a>.'
-                % (self._get_url_prefix(), response.run.id))
+            html = (f'<a href="{link}" target="_blank" >Run details</a>.')
             IPython.display.display(IPython.display.HTML(html))
-        return response.run
+        else:
+            print(f'Run details: {link}')
+
+        return response
+
+    def archive_run(self, run_id: str) -> dict:
+        """Archives a run.
+
+        Args:
+            run_id: ID of the run.
+
+        Returns:
+            Empty dictionary.
+        """
+        return self._run_api.archive_run(run_id=run_id)
+
+    def unarchive_run(self, run_id: str) -> dict:
+        """Restores an archived run.
+
+        Args:
+            run_id: ID of the run.
+
+        Returns:
+            Empty dictionary.
+        """
+        return self._run_api.unarchive_run(run_id=run_id)
+
+    def delete_run(self, run_id: str) -> dict:
+        """Deletes a run.
+
+        Args:
+            run_id: ID of the run.
+
+        Returns:
+            Empty dictionary.
+        """
+        return self._run_api.delete_run(run_id=run_id)
+
+    def terminate_run(self, run_id: str) -> dict:
+        """Terminates a run.
+
+        Args:
+            run_id: ID of the run.
+
+        Returns:
+            Empty dictionary.
+        """
+        return self._run_api.terminate_run(run_id=run_id)
 
     def create_recurring_run(
         self,
         experiment_id: str,
         job_name: str,
         description: Optional[str] = None,
         start_time: Optional[str] = None,
@@ -800,731 +809,891 @@
         max_concurrency: Optional[int] = 1,
         no_catchup: Optional[bool] = None,
         params: Optional[dict] = None,
         pipeline_package_path: Optional[str] = None,
         pipeline_id: Optional[str] = None,
         version_id: Optional[str] = None,
         enabled: bool = True,
+        pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ) -> kfp_server_api.ApiJob:
-        """Create a recurring run.
+    ) -> kfp_server_api.V2beta1RecurringRun:
+        """Creates a recurring run.
 
         Args:
-          experiment_id: The string id of an experiment.
-          job_name: Name of the job.
-          description: An optional job description.
-          start_time: The RFC3339 time string of the time when to start the job.
-          end_time: The RFC3339 time string of the time when to end the job.
-          interval_second: Integer indicating the seconds between two recurring runs in for a periodic schedule.
-          cron_expression: A cron expression representing a set of times, using 6 space-separated fields, e.g. "0 0 9 ? * 2-6".
-            See `here <https://pkg.go.dev/github.com/robfig/cron#hdr-CRON_Expression_Format>`_ for details of the cron expression format.
-          max_concurrency: Integer indicating how many jobs can be run in parallel.
-          no_catchup: Whether the recurring run should catch up if behind schedule.
-            For example, if the recurring run is paused for a while and re-enabled
-            afterwards. If no_catchup=False, the scheduler will catch up on (backfill) each
-            missed interval. Otherwise, it only schedules the latest interval if more than one interval
-            is ready to be scheduled.
-            Usually, if your pipeline handles backfill internally, you should turn catchup
-            off to avoid duplicate backfill. (default: {False})
-          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
-          params: A dictionary with key (string) as param name and value (string) as param value.
-          pipeline_id: The id of a pipeline.
-          version_id: The id of a pipeline version.
-            If both pipeline_id and version_id are specified, version_id will take precendence.
-            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
-          enabled: A bool indicating whether the recurring run is enabled or disabled.
-          enable_caching: Optional. Whether or not to enable caching for the run.
-            This setting affects v2 compatible mode and v2 mode only.
-            If not set, defaults to the compile time settings, which are True for all
-            tasks by default, while users may specify different caching options for
-            individual tasks.
-            If set, the setting applies to all tasks in the pipeline -- overrides
-            the compile time settings.
-          service_account: Optional. Specifies which Kubernetes service account this
-            recurring run uses.
-
+            experiment_id: ID of the experiment.
+            job_name: Name of the job.
+            description: Description of the job.
+            start_time: RFC3339 time string of the time when to start the
+                job.
+            end_time: RFC3339 time string of the time when to end the job.
+            interval_second: Integer indicating the seconds between two
+                recurring runs in for a periodic schedule.
+            cron_expression: Cron expression representing a set of times,
+                using 6 space-separated fields (e.g., ``'0 0 9 ? * 2-6'``). See `cron format
+                <https://pkg.go.dev/github.com/robfig/cron#hdr-CRON_Expression_Format>`_.
+            max_concurrency: Integer indicating how many jobs can be run in
+                parallel.
+            no_catchup: Whether the recurring run should catch up if behind
+                schedule. For example, if the recurring run is paused for a
+                while and re-enabled afterwards. If ``no_catchup=False``, the
+                scheduler will catch up on (backfill) each missed interval.
+                Otherwise, it only schedules the latest interval if more than
+                one interval is ready to be scheduled. Usually, if your pipeline
+                handles backfill internally, you should turn catchup off to
+                avoid duplicate backfill.
+            pipeline_package_path: Local path of the pipeline package (the
+                filename should end with one of the following .tar.gz, .tgz,
+                .zip, .json).
+            params: Arguments to the pipeline function provided as a dict.
+            pipeline_id: ID of a pipeline.
+            version_id: ID of a pipeline version.
+                If both ``pipeline_id`` and ``version_id`` are specified, ``version_id``
+                will take precedence.
+                If only ``pipeline_id`` is specified, the default version of this
+                pipeline is used to create the run.
+            enabled: Whether to enable or disable the recurring run.
+            pipeline_root: Root path of the pipeline outputs.
+            enable_caching: Whether or not to enable caching for the
+                run. If not set, defaults to the compile time settings, which
+                is ``True`` for all tasks by default, while users may specify
+                different caching options for individual tasks. If set, the
+                setting applies to all tasks in the pipeline (overrides the
+                compile time settings).
+            service_account: Specifies which Kubernetes service
+                account this recurring run uses.
         Returns:
-          A Job object. Most important field is id.
-
-        Raises:
-          ValueError: If required parameters are not supplied.
+            ``V2beta1RecurringRun`` object.
         """
 
         job_config = self._create_job_config(
-            experiment_id=experiment_id,
             params=params,
             pipeline_package_path=pipeline_package_path,
             pipeline_id=pipeline_id,
             version_id=version_id,
             enable_caching=enable_caching,
+            pipeline_root=pipeline_root,
         )
 
         if all([interval_second, cron_expression
                ]) or not any([interval_second, cron_expression]):
             raise ValueError(
-                'Either interval_second or cron_expression is required')
+                'Either interval_second or cron_expression is required.')
         if interval_second is not None:
-            trigger = kfp_server_api.models.ApiTrigger(
-                periodic_schedule=kfp_server_api.models.ApiPeriodicSchedule(
+            trigger = kfp_server_api.V2beta1Trigger(
+                periodic_schedule=kfp_server_api.V2beta1PeriodicSchedule(
                     start_time=start_time,
                     end_time=end_time,
                     interval_second=interval_second))
         if cron_expression is not None:
-            trigger = kfp_server_api.models.ApiTrigger(
-                cron_schedule=kfp_server_api.models.ApiCronSchedule(
+            trigger = kfp_server_api.V2beta1Trigger(
+                cron_schedule=kfp_server_api.V2beta1CronSchedule(
                     start_time=start_time,
                     end_time=end_time,
                     cron=cron_expression))
 
-        job_body = kfp_server_api.models.ApiJob(
-            enabled=enabled,
-            pipeline_spec=job_config.spec,
-            resource_references=job_config.resource_references,
-            name=job_name,
+        mode = kfp_server_api.RecurringRunMode.DISABLE
+        if enabled:
+            mode = kfp_server_api.RecurringRunMode.ENABLE
+
+        job_body = kfp_server_api.V2beta1RecurringRun(
+            experiment_id=experiment_id,
+            mode=mode,
+            pipeline_spec=job_config.pipeline_spec,
+            pipeline_version_reference=job_config.pipeline_version_reference,
+            runtime_config=job_config.runtime_config,
+            display_name=job_name,
             description=description,
             no_catchup=no_catchup,
             trigger=trigger,
             max_concurrency=max_concurrency,
             service_account=service_account)
-        return self._job_api.create_job(body=job_body)
+        return self._recurring_run_api.create_recurring_run(body=job_body)
 
     def _create_job_config(
         self,
-        experiment_id: str,
-        params: Optional[dict],
+        params: Optional[Dict[str, Any]],
         pipeline_package_path: Optional[str],
         pipeline_id: Optional[str],
         version_id: Optional[str],
         enable_caching: Optional[bool],
-    ):
-        """Create a JobConfig with spec and resource_references.
-
-        Args:
-          experiment_id: The id of an experiment.
-          pipeline_package_path: Local path of the pipeline package(the filename should end with one of the following .tar.gz, .tgz, .zip, .yaml, .yml).
-          params: A dictionary with key (string) as param name and value (string) as param value.
-          pipeline_id: The id of a pipeline.
-          version_id: The id of a pipeline version.
-            If both pipeline_id and version_id are specified, version_id will take precendence.
-            If only pipeline_id is specified, the default version of this pipeline is used to create the run.
-          enable_caching: Whether or not to enable caching for the run.
-            This setting affects v2 compatible mode and v2 mode only.
-            If not set, defaults to the compile time settings, which are True for all
-            tasks by default, while users may specify different caching options for
-            individual tasks.
-            If set, the setting applies to all tasks in the pipeline -- overrides
-            the compile time settings.
-
-        Returns:
-          A JobConfig object with attributes spec and resource_reference.
-        """
-
-        class JobConfig:
+        pipeline_root: Optional[str],
+    ) -> _JobConfig:
+        """Creates a JobConfig with spec and resource_references.
+
+        Args:
+            pipeline_package_path: Local path of the pipeline package (the
+                filename should end with one of the following .tar.gz, .tgz,
+                .zip, .yaml, .yml).
+            params: A dictionary with key as param name and value as param value.
+            pipeline_id: ID of a pipeline.
+            version_id: ID of a pipeline version.
+                If both pipeline_id and version_id are specified, version_id
+                will take precedence. If only pipeline_id is specified, the
+                default version of this pipeline is used to create the run.
+            enable_caching: Whether or not to enable caching for the
+                run. If not set, defaults to the compile time settings, which
+                is ``True`` for all tasks by default, while users may specify
+                different caching options for individual tasks. If set, the
+                setting applies to all tasks in the pipeline (overrides the
+                compile time settings).
+            pipeline_root: Root path of the pipeline outputs.
+
+        Returns:
+            A _JobConfig object with attributes .pipeline_spec,
+                .pipeline_version_reference, and .runtime_config.
+        """
+        from_spec = pipeline_package_path is not None
+        from_template = pipeline_id is not None or version_id is not None
+        if from_spec == from_template:
+            raise ValueError(
+                'Must specify either `pipeline_pacakge_path` or both `pipeline_id` and `version_id`.'
+            )
+        if (pipeline_id is None) != (version_id is None):
+            raise ValueError(
+                'To run a pipeline from an existing template, both `pipeline_id` and `version_id` are required.'
+            )
 
-            def __init__(self, spec, resource_references):
-                self.spec = spec
-                self.resource_references = resource_references
+        if params is None:
+            params = {}
 
-        params = params or {}
-        pipeline_json_string = None
+        pipeline_spec = None
         if pipeline_package_path:
-            pipeline_obj = self._extract_pipeline_yaml(pipeline_package_path)
+            pipeline_doc = _extract_pipeline_yaml(pipeline_package_path)
 
-            # Caching option set at submission time overrides the compile time settings.
+            # Caching option set at submission time overrides the compile time
+            # settings.
             if enable_caching is not None:
-                self._override_caching_options(pipeline_obj, enable_caching)
+                _override_caching_options(pipeline_doc.pipeline_spec,
+                                          enable_caching)
+            pipeline_spec = pipeline_doc.to_dict()
+
+        pipeline_version_reference = None
+        if pipeline_id is not None and version_id is not None:
+            pipeline_version_reference = kfp_server_api.V2beta1PipelineVersionReference(
+                pipeline_id=pipeline_id, pipeline_version_id=version_id)
 
-            pipeline_json_string = json.dumps(pipeline_obj)
-        api_params = [
-            kfp_server_api.ApiParameter(
-                name=sanitize_k8s_name(name=k, allow_capital_underscore=True),
-                value=str(v) if type(v) not in (list, dict) else json.dumps(v))
-            for k, v in params.items()
-        ]
-        resource_references = []
-        key = kfp_server_api.models.ApiResourceKey(
-            id=experiment_id,
-            type=kfp_server_api.models.ApiResourceType.EXPERIMENT)
-        reference = kfp_server_api.models.ApiResourceReference(
-            key=key, relationship=kfp_server_api.models.ApiRelationship.OWNER)
-        resource_references.append(reference)
-
-        if version_id:
-            key = kfp_server_api.models.ApiResourceKey(
-                id=version_id,
-                type=kfp_server_api.models.ApiResourceType.PIPELINE_VERSION)
-            reference = kfp_server_api.models.ApiResourceReference(
-                key=key,
-                relationship=kfp_server_api.models.ApiRelationship.CREATOR)
-            resource_references.append(reference)
-
-        spec = kfp_server_api.models.ApiPipelineSpec(
-            pipeline_id=pipeline_id,
-            workflow_manifest=pipeline_json_string,
-            parameters=api_params)
-        return JobConfig(spec=spec, resource_references=resource_references)
+        runtime_config = kfp_server_api.V2beta1RuntimeConfig(
+            pipeline_root=pipeline_root,
+            parameters=params,
+        )
+        return _JobConfig(
+            pipeline_spec=pipeline_spec,
+            pipeline_version_reference=pipeline_version_reference,
+            runtime_config=runtime_config,
+        )
 
     def create_run_from_pipeline_func(
         self,
-        pipeline_func: Callable,
-        arguments: Mapping[str, str],
+        pipeline_func: base_component.BaseComponent,
+        arguments: Optional[Dict[str, Any]] = None,
         run_name: Optional[str] = None,
         experiment_name: Optional[str] = None,
-        pipeline_conf: Optional[dsl.PipelineConf] = None,
         namespace: Optional[str] = None,
-        mode: dsl.PipelineExecutionMode = dsl.PipelineExecutionMode.V1_LEGACY,
-        launcher_image: Optional[str] = None,
         pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ):
+        experiment_id: Optional[str] = None,
+    ) -> RunPipelineResult:
         """Runs pipeline on KFP-enabled Kubernetes cluster.
 
-        This command compiles the pipeline function, creates or gets an experiment and submits the pipeline for execution.
+        This command compiles the pipeline function, creates or gets an
+        experiment, then submits the pipeline for execution.
 
         Args:
-          pipeline_func: A function that describes a pipeline by calling components and composing them into execution graph.
-          arguments: Arguments to the pipeline function provided as a dict.
-          run_name: Optional. Name of the run to be shown in the UI.
-          experiment_name: Optional. Name of the experiment to add the run to.
-          pipeline_conf: Optional. Pipeline configuration ops that will be applied
-            to all the ops in the pipeline func.
-          namespace: Kubernetes namespace where the pipeline runs are created.
-            For single user deployment, leave it as None;
-            For multi user, input a namespace where the user is authorized
-          mode: The PipelineExecutionMode to use when compiling and running
-            pipeline_func.
-          launcher_image: The launcher image to use if the mode is specified as
-            PipelineExecutionMode.V2_COMPATIBLE. Should only be needed for tests
-            or custom deployments right now.
-          pipeline_root: The root path of the pipeline outputs. This argument should
-            be used only for pipeline compiled with
-            dsl.PipelineExecutionMode.V2_COMPATIBLE or
-            dsl.PipelineExecutionMode.V2_ENGINGE mode.
-          enable_caching: Optional. Whether or not to enable caching for the run.
-            This setting affects v2 compatible mode and v2 mode only.
-            If not set, defaults to the compile time settings, which are True for all
-            tasks by default, while users may specify different caching options for
-            individual tasks.
-            If set, the setting applies to all tasks in the pipeline -- overrides
-            the compile time settings.
-          service_account: Optional. Specifies which Kubernetes service account this
-            run uses.
-        """
-        if pipeline_root is not None and mode == dsl.PipelineExecutionMode.V1_LEGACY:
-            raise ValueError('`pipeline_root` should not be used with '
-                             'dsl.PipelineExecutionMode.V1_LEGACY mode.')
+            pipeline_func: Pipeline function constructed with ``@kfp.dsl.pipeline`` decorator.
+            arguments: Arguments to the pipeline function provided as a dict.
+            run_name: Name of the run to be shown in the UI.
+            experiment_name: Name of the experiment to add the run to. You cannot specify both experiment_name and experiment_id.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+            pipeline_root: Root path of the pipeline outputs.
+            enable_caching: Whether or not to enable caching for the
+                run. If not set, defaults to the compile time settings, which
+                is ``True`` for all tasks by default, while users may specify
+                different caching options for individual tasks. If set, the
+                setting applies to all tasks in the pipeline (overrides the
+                compile time settings).
+            service_account: Specifies which Kubernetes service
+                account to use for this run.
+            experiment_id: ID of the experiment to add the run to. You cannot specify both experiment_id and experiment_name.
 
+        Returns:
+            ``RunPipelineResult`` object containing information about the pipeline run.
+        """
         #TODO: Check arguments against the pipeline function
-        pipeline_name = pipeline_func.__name__
+        pipeline_name = pipeline_func.name
         run_name = run_name or pipeline_name + ' ' + datetime.datetime.now(
         ).strftime('%Y-%m-%d %H-%M-%S')
+
         with tempfile.TemporaryDirectory() as tmpdir:
             pipeline_package_path = os.path.join(tmpdir, 'pipeline.yaml')
-            compiler.Compiler(
-                mode=mode, launcher_image=launcher_image).compile(
-                    pipeline_func=pipeline_func,
-                    package_path=pipeline_package_path,
-                    pipeline_conf=pipeline_conf)
+            compiler.Compiler().compile(
+                pipeline_func=pipeline_func,
+                package_path=pipeline_package_path,
+            )
 
             return self.create_run_from_pipeline_package(
                 pipeline_file=pipeline_package_path,
                 arguments=arguments,
                 run_name=run_name,
+                experiment_id=experiment_id,
                 experiment_name=experiment_name,
                 namespace=namespace,
                 pipeline_root=pipeline_root,
                 enable_caching=enable_caching,
                 service_account=service_account,
             )
 
     def create_run_from_pipeline_package(
         self,
         pipeline_file: str,
-        arguments: Mapping[str, str],
+        arguments: Optional[Dict[str, Any]] = None,
         run_name: Optional[str] = None,
         experiment_name: Optional[str] = None,
         namespace: Optional[str] = None,
         pipeline_root: Optional[str] = None,
         enable_caching: Optional[bool] = None,
         service_account: Optional[str] = None,
-    ):
+        experiment_id: Optional[str] = None,
+    ) -> RunPipelineResult:
         """Runs pipeline on KFP-enabled Kubernetes cluster.
 
-        This command takes a local pipeline package, creates or gets an experiment
-        and submits the pipeline for execution.
+        This command takes a local pipeline package, creates or gets an
+        experiment, then submits the pipeline for execution.
 
         Args:
-          pipeline_file: A compiled pipeline package file.
-          arguments: Arguments to the pipeline function provided as a dict.
-          run_name: Optional. Name of the run to be shown in the UI.
-          experiment_name: Optional. Name of the experiment to add the run to.
-          namespace: Kubernetes namespace where the pipeline runs are created.
-            For single user deployment, leave it as None;
-            For multi user, input a namespace where the user is authorized
-          pipeline_root: The root path of the pipeline outputs. This argument should
-            be used only for pipeline compiled with
-            dsl.PipelineExecutionMode.V2_COMPATIBLE or
-            dsl.PipelineExecutionMode.V2_ENGINGE mode.
-          enable_caching: Optional. Whether or not to enable caching for the run.
-            This setting affects v2 compatible mode and v2 mode only.
-            If not set, defaults to the compile time settings, which are True for all
-            tasks by default, while users may specify different caching options for
-            individual tasks.
-            If set, the setting applies to all tasks in the pipeline -- overrides
-            the compile time settings.
-          service_account: Optional. Specifies which Kubernetes service account this
-            run uses.
-        """
-
-        class RunPipelineResult:
-
-            def __init__(self, client, run_info):
-                self._client = client
-                self.run_info = run_info
-                self.run_id = run_info.id
-
-            def wait_for_run_completion(self, timeout=None):
-                timeout = timeout or datetime.timedelta.max
-                return self._client.wait_for_run_completion(
-                    self.run_id, timeout)
+            pipeline_file: A compiled pipeline package file.
+            arguments: Arguments to the pipeline function provided as a dict.
+            run_name:  Name of the run to be shown in the UI.
+            experiment_name: Name of the experiment to add the run to. You cannot specify both experiment_name and experiment_id.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+            pipeline_root: Root path of the pipeline outputs.
+            enable_caching: Whether or not to enable caching for the
+                run. If not set, defaults to the compile time settings, which
+                is ``True`` for all tasks by default, while users may specify
+                different caching options for individual tasks. If set, the
+                setting applies to all tasks in the pipeline (overrides the
+                compile time settings).
+            service_account: Specifies which Kubernetes service
+                account to use for this run.
+            experiment_id: ID of the experiment to add the run to. You cannot specify both experiment_id and experiment_name.
 
-            def __repr__(self):
-                return 'RunPipelineResult(run_id={})'.format(self.run_id)
+        Returns:
+            ``RunPipelineResult`` object containing information about the pipeline run.
+        """
 
         #TODO: Check arguments against the pipeline function
         pipeline_name = os.path.basename(pipeline_file)
-        experiment_name = experiment_name or os.environ.get(
-            KF_PIPELINES_DEFAULT_EXPERIMENT_NAME, None)
-        overridden_experiment_name = os.environ.get(
-            KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME, experiment_name)
-        if overridden_experiment_name != experiment_name:
-            import warnings
-            warnings.warn('Changing experiment name from "{}" to "{}".'.format(
-                experiment_name, overridden_experiment_name))
-        experiment_name = overridden_experiment_name or 'Default'
+
+        if (experiment_name is not None) and (experiment_id is not None):
+            raise ValueError(
+                'You cannot specify both experiment_name and experiment_id.')
+
+        if not experiment_id:
+            experiment_name = experiment_name or os.environ.get(
+                KF_PIPELINES_DEFAULT_EXPERIMENT_NAME, None)
+            overridden_experiment_name = os.environ.get(
+                KF_PIPELINES_OVERRIDE_EXPERIMENT_NAME, experiment_name)
+            if overridden_experiment_name != experiment_name:
+                warnings.warn(
+                    f'Changing experiment name from "{experiment_name}" to "{overridden_experiment_name}".'
+                )
+            experiment_name = overridden_experiment_name or 'Default'
+            experiment = self.create_experiment(
+                name=experiment_name, namespace=namespace)
+            experiment_id = experiment.experiment_id
+
         run_name = run_name or (
             pipeline_name + ' ' +
             datetime.datetime.now().strftime('%Y-%m-%d %H-%M-%S'))
-        experiment = self.create_experiment(
-            name=experiment_name, namespace=namespace)
+
         run_info = self.run_pipeline(
-            experiment_id=experiment.id,
+            experiment_id=experiment_id,
             job_name=run_name,
             pipeline_package_path=pipeline_file,
             params=arguments,
             pipeline_root=pipeline_root,
             enable_caching=enable_caching,
             service_account=service_account,
         )
         return RunPipelineResult(self, run_info)
 
-    def delete_job(self, job_id: str):
-        """Deletes a job.
+    def delete_job(self, job_id: str) -> dict:
+        """Deletes a job (recurring run).
 
         Args:
-          job_id: id of the job.
+            job_id: ID of the job.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
+            Empty dictionary.
+        """
+        warnings.warn(
+            '`delete_job` is deprecated. Please use `delete_recurring_run` instead.'
+            f'\nReroute to calling `delete_recurring_run(recurring_run_id="{job_id}")`',
+            category=DeprecationWarning,
+            stacklevel=2)
+        return self.delete_recurring_run(recurring_run_id=job_id)
+
+    def delete_recurring_run(self, recurring_run_id: str) -> dict:
+        """Deletes a recurring run.
 
-        Raises:
-          kfp_server_api.ApiException: If the job is not found.
+        Args:
+            recurring_run_id: ID of the recurring_run.
+
+        Returns:
+            Empty dictionary.
         """
-        return self._job_api.delete_job(id=job_id)
+        return self._recurring_run_api.delete_recurring_run(
+            recurring_run_id=recurring_run_id)
 
-    def disable_job(self, job_id: str):
-        """Disables a job.
+    def disable_job(self, job_id: str) -> dict:
+        """Disables a job (recurring run).
 
         Args:
-          job_id: id of the job.
+            job_id: ID of the job.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
+            Empty dictionary.
+        """
+        warnings.warn(
+            '`disable_job` is deprecated. Please use `disable_recurring_run` instead.'
+            f'\nReroute to calling `disable_recurring_run(recurring_run_id="{job_id}")`',
+            category=DeprecationWarning,
+            stacklevel=2)
+        return self.disable_recurring_run(recurring_run_id=job_id)
+
+    def disable_recurring_run(self, recurring_run_id: str) -> dict:
+        """Disables a recurring run.
 
-        Raises:
-          ApiException: If the job is not found.
+        Args:
+            recurring_run_id: ID of the recurring_run.
+
+        Returns:
+            Empty dictionary.
         """
-        return self._job_api.disable_job(id=job_id)
+        return self._recurring_run_api.disable_recurring_run(
+            recurring_run_id=recurring_run_id)
 
-    def enable_job(self, job_id: str):
-        """Enables a job.
+    def enable_job(self, job_id: str) -> dict:
+        """Enables a job (recurring run).
 
         Args:
-          job_id: id of the job.
+            job_id: ID of the job.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
+            Empty dictionary.
+        """
+        warnings.warn(
+            '`enable_job` is deprecated. Please use `enable_recurring_run` instead.'
+            f'\nReroute to calling `enable_recurring_run(recurring_run_id="{job_id}")`',
+            category=DeprecationWarning,
+            stacklevel=2)
+        return self.enable_recurring_run(recurring_run_id=job_id)
+
+    def enable_recurring_run(self, recurring_run_id: str) -> dict:
+        """Enables a recurring run.
 
-        Raises:
-          ApiException: If the job is not found.
+        Args:
+            recurring_run_id: ID of the recurring_run.
+
+        Returns:
+            Empty dictionary.
         """
-        return self._job_api.enable_job(id=job_id)
+        return self._recurring_run_api.enable_recurring_run(
+            recurring_run_id=recurring_run_id)
 
     def list_runs(
-            self,
-            page_token: str = '',
-            page_size: int = 10,
-            sort_by: str = '',
-            experiment_id: Optional[str] = None,
-            namespace: Optional[str] = None,
-            filter: Optional[str] = None) -> kfp_server_api.ApiListRunsResponse:
-        """List runs, optionally can be filtered by experiment or namespace.
-
-        Args:
-          page_token: Token for starting of the page.
-          page_size: Size of the page.
-          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
-          experiment_id: Experiment id to filter upon
-          namespace: Kubernetes namespace to filter upon.
-            For single user deployment, leave it as None;
-            For multi user, input a namespace where the user is authorized.
-          filter: A url-encoded, JSON-serialized Filter protocol buffer
-            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
-
-            An example filter string would be:
-
-                # For the list of filter operations please see:
-                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
-                json.dumps({
-                    "predicates": [{
-                        "op": _FILTER_OPERATIONS["EQUALS"],
-                        "key": "name",
-                        "stringValue": "my-name",
-                    }]
-                })
+        self,
+        page_token: str = '',
+        page_size: int = 10,
+        sort_by: str = '',
+        experiment_id: Optional[str] = None,
+        namespace: Optional[str] = None,
+        filter: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1ListRunsResponse:
+        """List runs.
+
+        Args:
+            page_token: Page token for obtaining page from paginated response.
+            page_size: Size of the page.
+            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'display_name desc'``.
+            experiment_id: Experiment ID to filter upon
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+            filter: A url-encoded, JSON-serialized Filter protocol buffer
+                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/cb7d9a87c999eb1d2280959e5afbeee9e270ef3d/backend/api/v2beta1/filter.proto>`_). For a list of all filter operations ``'opertion'``, see `here <https://github.com/kubeflow/pipelines/blob/777c98153daf3dfae82730e14ff37bdddc334c4d/sdk/python/kfp/client/client.py#L37-L45>`_. Example:
+
+                  ::
+
+                    json.dumps({
+                        "predicates": [{
+                            "operation": "EQUALS",
+                            "key": "display_name",
+                            "stringValue": "my-name",
+                        }]
+                    })
 
-        Returns:
-          A response object including a list of experiments and next page token.
+          Returns:
+            ``V2beta1ListRunsResponse`` object.
         """
         namespace = namespace or self.get_user_namespace()
         if experiment_id is not None:
-            response = self._run_api.list_runs_v1(
+            return self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.models
-                .api_resource_type.ApiResourceType.EXPERIMENT,
-                resource_reference_key_id=experiment_id,
+                experiment_id=experiment_id,
                 filter=filter)
-        elif namespace:
-            response = self._run_api.list_runs_v1(
+
+        elif namespace is not None:
+            return self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.models
-                .api_resource_type.ApiResourceType.NAMESPACE,
-                resource_reference_key_id=namespace,
+                namespace=namespace,
                 filter=filter)
+
         else:
-            response = self._run_api.list_runs_v1(
+            return self._run_api.list_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
                 filter=filter)
-        return response
 
     def list_recurring_runs(
-            self,
-            page_token: str = '',
-            page_size: int = 10,
-            sort_by: str = '',
-            experiment_id: Optional[str] = None,
-            filter: Optional[str] = None) -> kfp_server_api.ApiListJobsResponse:
-        """List recurring runs.
-
-        Args:
-          page_token: Token for starting of the page.
-          page_size: Size of the page.
-          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
-          experiment_id: Experiment id to filter upon.
-          filter: A url-encoded, JSON-serialized Filter protocol buffer
-            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
-
-            An example filter string would be:
-
-                # For the list of filter operations please see:
-                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
-                json.dumps({
-                    "predicates": [{
-                        "op": _FILTER_OPERATIONS["EQUALS"],
-                        "key": "name",
-                        "stringValue": "my-name",
-                    }]
-                })
+        self,
+        page_token: str = '',
+        page_size: int = 10,
+        sort_by: str = '',
+        experiment_id: Optional[str] = None,
+        namespace: Optional[str] = None,
+        filter: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1ListRecurringRunsResponse:
+        """Lists recurring runs.
+
+        Args:
+            page_token: Page token for obtaining page from paginated response.
+            page_size: Size of the page.
+            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'display_name desc'``.
+            experiment_id: Experiment ID to filter upon.
+            namespace: Kubernetes namespace to use. Used for multi-user deployments. For single-user deployments, this should be left as ``None``.
+            filter: A url-encoded, JSON-serialized Filter protocol buffer
+                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/cb7d9a87c999eb1d2280959e5afbeee9e270ef3d/backend/api/v2beta1/filter.proto>`_). Example:
+
+                  ::
+
+                    json.dumps({
+                        "predicates": [{
+                            "operation": "EQUALS",
+                            "key": "display_name",
+                            "stringValue": "my-name",
+                        }]
+                    })
 
         Returns:
-          A response object including a list of recurring_runs and next page token.
+            ``V2beta1ListRecurringRunsResponse`` object.
         """
         if experiment_id is not None:
-            response = self._job_api.list_jobs(
+            return self._recurring_run_api.list_recurring_runs(
+                page_token=page_token,
+                page_size=page_size,
+                sort_by=sort_by,
+                experiment_id=experiment_id,
+                filter=filter)
+
+        elif namespace is not None:
+            return self._recurring_run_api.list_recurring_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
-                resource_reference_key_type=kfp_server_api.models
-                .api_resource_type.ApiResourceType.EXPERIMENT,
-                resource_reference_key_id=experiment_id,
+                namespace=namespace,
                 filter=filter)
+
         else:
-            response = self._job_api.list_jobs(
+            return self._recurring_run_api.list_recurring_runs(
                 page_token=page_token,
                 page_size=page_size,
                 sort_by=sort_by,
                 filter=filter)
-        return response
 
-    def get_recurring_run(self, job_id: str) -> kfp_server_api.ApiJob:
-        """Get recurring_run details.
+    def get_recurring_run(
+        self,
+        recurring_run_id: str,
+        job_id: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1RecurringRun:
+        """Gets recurring run details.
 
         Args:
-          job_id: id of the recurring_run.
+            recurring_run_id: ID of the recurring run.
+            job_id: Deprecated. Use `recurring_run_id` instead.
 
         Returns:
-          A response object including details of a recurring_run.
-
-        Raises:
-          kfp_server_api.ApiException: If recurring_run is not found.
+            ``V2beta1RecurringRun`` object.
         """
-        return self._job_api.get_job(id=job_id)
+        if job_id is not None:
+            warnings.warn(
+                '`job_id` is deprecated. Please use `recurring_run_id` instead.',
+                category=DeprecationWarning,
+                stacklevel=2)
+            recurring_run_id = recurring_run_id or job_id
+
+        return self._recurring_run_api.get_recurring_run(
+            recurring_run_id=recurring_run_id)
 
-    def get_run(self, run_id: str) -> kfp_server_api.ApiRun:
-        """Get run details.
+    def get_run(self, run_id: str) -> kfp_server_api.V2beta1Run:
+        """Gets run details.
 
         Args:
-          run_id: id of the run.
+            run_id: ID of the run.
 
         Returns:
-          A response object including details of a run.
-
-        Raises:
-          kfp_server_api.ApiException: If run is not found.
+            ``V2beta1Run`` object.
         """
-        return self._run_api.get_run_v1(run_id=run_id)
+        return self._run_api.get_run(run_id=run_id)
 
-    def wait_for_run_completion(self, run_id: str, timeout: int):
+    def wait_for_run_completion(
+        self,
+        run_id: str,
+        timeout: int,
+        sleep_duration: int = 5,
+    ) -> kfp_server_api.V2beta1Run:
         """Waits for a run to complete.
 
         Args:
-          run_id: Run id, returned from run_pipeline.
-          timeout: Timeout in seconds.
+            run_id: ID of the run.
+            timeout: Timeout after which the client should stop waiting for run completion (seconds).
+            sleep_duration: Time in seconds between retries.
 
         Returns:
-          A run detail object: Most important fields are run and pipeline_runtime.
-
-        Raises:
-          TimeoutError: if the pipeline run failed to finish before the specified timeout.
+            ``V2beta1Run`` object.
         """
-        status = 'Running:'
+        state = 'Running:'
         start_time = datetime.datetime.now()
         if isinstance(timeout, datetime.timedelta):
             timeout = timeout.total_seconds()
         is_valid_token = False
-        while (status is None or status.lower()
-               not in ['succeeded', 'failed', 'skipped', 'error']):
+        finish_states = ['succeeded', 'failed', 'skipped', 'error']
+        while True:
             try:
-                get_run_response = self._run_api.get_run_v1(run_id=run_id)
+                get_run_response = self._run_api.get_run(run_id=run_id)
                 is_valid_token = True
-            except ApiException as api_ex:
+            except kfp_server_api.ApiException as api_ex:
                 # if the token is valid but receiving 401 Unauthorized error
                 # then refresh the token
                 if is_valid_token and api_ex.status == 401:
                     logging.info('Access token has expired !!! Refreshing ...')
                     self._refresh_api_client_token()
                     continue
                 else:
                     raise api_ex
-            status = get_run_response.run.status
+            state = get_run_response.state
             elapsed_time = (datetime.datetime.now() -
                             start_time).total_seconds()
             logging.info('Waiting for the job to complete...')
             if elapsed_time > timeout:
                 raise TimeoutError('Run timeout')
-            time.sleep(5)
-        return get_run_response
-
-    def _get_workflow_json(self, run_id):
-        """Get the workflow json.
-
-        Args:
-          run_id: run id, returned from run_pipeline.
-
-        Returns:
-          workflow: Json workflow
-        """
-        get_run_response = self._run_api.get_run_v1(run_id=run_id)
-        workflow = get_run_response.pipeline_runtime.workflow_manifest
-        workflow_json = json.loads(workflow)
-        return workflow_json
+            if state is not None and state.lower() in finish_states:
+                return get_run_response
+            time.sleep(sleep_duration)
 
     def upload_pipeline(
         self,
-        pipeline_package_path: str = None,
-        pipeline_name: str = None,
-        description: str = None,
-    ) -> kfp_server_api.ApiPipeline:
-        """Uploads the pipeline to the Kubeflow Pipelines cluster.
+        pipeline_package_path: str,
+        pipeline_name: Optional[str] = None,
+        description: Optional[str] = None,
+        namespace: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1Pipeline:
+        """Uploads a pipeline.
 
         Args:
-          pipeline_package_path: Local path to the pipeline package.
-          pipeline_name: Optional. Name of the pipeline to be shown in the UI.
-          description: Optional. Description of the pipeline to be shown in the UI.
+            pipeline_package_path: Local path to the pipeline package.
+            pipeline_name: Name of the pipeline to be shown in the UI.
+            description: Description of the pipeline to be shown in the UI.
+            namespace: Optional. Kubernetes namespace where the pipeline should
+                be uploaded. For single user deployment, leave it as None; For
+                multi user, input a namespace where the user is authorized.
 
         Returns:
-          Server response object containing pipleine id and other information.
+            ``V2beta1Pipeline`` object.
         """
-
+        if pipeline_name is None:
+            pipeline_doc = _extract_pipeline_yaml(pipeline_package_path)
+            pipeline_name = pipeline_doc.pipeline_spec.pipeline_info.name
+        validate_pipeline_resource_name(pipeline_name)
         response = self._upload_api.upload_pipeline(
-            pipeline_package_path, name=pipeline_name, description=description)
+            pipeline_package_path,
+            name=pipeline_name,
+            description=description,
+            namespace=namespace)
+        link = f'{self._get_url_prefix()}/#/pipelines/details/{response.pipeline_id}'
         if self._is_ipython():
             import IPython
-            html = '<a href=%s/#/pipelines/details/%s>Pipeline details</a>.' % (
-                self._get_url_prefix(), response.id)
+            html = f'<a href="{link}" target="_blank" >Pipeline details</a>.'
             IPython.display.display(IPython.display.HTML(html))
+        else:
+            print(f'Pipeline details: {link}')
+
         return response
 
     def upload_pipeline_version(
         self,
-        pipeline_package_path,
+        pipeline_package_path: str,
         pipeline_version_name: str,
         pipeline_id: Optional[str] = None,
         pipeline_name: Optional[str] = None,
         description: Optional[str] = None,
-    ) -> kfp_server_api.ApiPipelineVersion:
-        """Uploads a new version of the pipeline to the Kubeflow Pipelines
-        cluster.
+    ) -> kfp_server_api.V2beta1PipelineVersion:
+        """Uploads a new version of the pipeline.
 
         Args:
-          pipeline_package_path: Local path to the pipeline package.
-          pipeline_version_name:  Name of the pipeline version to be shown in the UI.
-          pipeline_id: Optional. Id of the pipeline.
-          pipeline_name: Optional. Name of the pipeline.
-          description: Optional. Description of the pipeline version to be shown in the UI.
+            pipeline_package_path: Local path to the pipeline package.
+            pipeline_version_name:  Name of the pipeline version to be shown in
+                the UI.
+            pipeline_id: ID of the pipeline.
+            pipeline_name: Name of the pipeline.
+            description: Description of the pipeline version to show in the UI.
 
         Returns:
-          Server response object containing pipleine id and other information.
-
-        Raises:
-          ValueError when none or both of pipeline_id or pipeline_name are specified
-          kfp_server_api.ApiException: If pipeline id is not found.
+            ``V2beta1PipelineVersion`` object.
         """
 
         if all([pipeline_id, pipeline_name
                ]) or not any([pipeline_id, pipeline_name]):
-            raise ValueError('Either pipeline_id or pipeline_name is required')
+            raise ValueError('Either pipeline_id or pipeline_name is required.')
 
         if pipeline_name:
             pipeline_id = self.get_pipeline_id(pipeline_name)
         kwargs = dict(
             name=pipeline_version_name,
             pipelineid=pipeline_id,
         )
 
         if description:
             kwargs['description'] = description
-        try:
-            response = self._upload_api.upload_pipeline_version(
-                pipeline_package_path, **kwargs)
-        except kfp_server_api.exceptions.ApiTypeError as e:
-            # ToDo: Remove this once we drop support for kfp_server_api < 1.7.1
-            if 'description' in e.message and 'unexpected keyword argument' in e.message:
-                raise NotImplementedError(
-                    'Pipeline version description is not supported in current kfp-server-api pypi package. Upgrade to 1.7.1 or above'
-                )
-            else:
-                raise e
 
+        response = self._upload_api.upload_pipeline_version(
+            pipeline_package_path, **kwargs)
+
+        link = f'{self._get_url_prefix()}/#/pipelines/details/{response.pipeline_id}/version/{response.pipeline_version_id}'
         if self._is_ipython():
             import IPython
-            html = '<a href=%s/#/pipelines/details/%s>Pipeline details</a>.' % (
-                self._get_url_prefix(), response.id)
+            html = f'<a href="{link}" target="_blank" >Pipeline details</a>.'
             IPython.display.display(IPython.display.HTML(html))
+        else:
+            print(f'Pipeline details: {link}')
+
         return response
 
-    def get_pipeline(self, pipeline_id: str) -> kfp_server_api.ApiPipeline:
-        """Get pipeline details.
+    def get_pipeline(self, pipeline_id: str) -> kfp_server_api.V2beta1Pipeline:
+        """Gets pipeline details.
 
         Args:
-          pipeline_id: id of the pipeline.
+            pipeline_id: ID of the pipeline.
 
         Returns:
-          A response object including details of a pipeline.
-
-        Raises:
-          kfp_server_api.ApiException: If pipeline is not found.
+            ``V2beta1Pipeline`` object.
         """
-        return self._pipelines_api.get_pipeline_v1(id=pipeline_id)
+        return self._pipelines_api.get_pipeline(pipeline_id=pipeline_id)
 
-    def delete_pipeline(self, pipeline_id):
-        """Delete pipeline.
+    def delete_pipeline(self, pipeline_id: str) -> dict:
+        """Deletes a pipeline.
 
         Args:
-          pipeline_id: id of the pipeline.
+            pipeline_id: ID of the pipeline.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
-
-        Raises:
-          kfp_server_api.ApiException: If pipeline is not found.
+            Empty dictionary.
         """
-        return self._pipelines_api.delete_pipeline_v1(id=pipeline_id)
+        return self._pipelines_api.delete_pipeline(pipeline_id=pipeline_id)
 
     def list_pipeline_versions(
         self,
         pipeline_id: str,
         page_token: str = '',
         page_size: int = 10,
         sort_by: str = '',
-        filter: Optional[str] = None
-    ) -> kfp_server_api.ApiListPipelineVersionsResponse:
+        filter: Optional[str] = None,
+    ) -> kfp_server_api.V2beta1ListPipelineVersionsResponse:
         """Lists pipeline versions.
 
         Args:
-          pipeline_id: Id of the pipeline to list versions
-          page_token: Token for starting of the page.
-          page_size: Size of the page.
-          sort_by: One of 'field_name', 'field_name desc'. For example, 'name desc'.
-          filter: A url-encoded, JSON-serialized Filter protocol buffer
-            (see [filter.proto](https://github.com/kubeflow/pipelines/blob/master/backend/api/filter.proto)).
+            pipeline_id: ID of the pipeline for which to list versions.
+            page_token: Page token for obtaining page from paginated response.
+            page_size: Size of the page.
+            sort_by: Sort string of format ``'[field_name]', '[field_name] desc'``. For example, ``'display_name desc'``.
+            filter: A url-encoded, JSON-serialized Filter protocol buffer
+                (see `filter.proto message <https://github.com/kubeflow/pipelines/blob/cb7d9a87c999eb1d2280959e5afbeee9e270ef3d/backend/api/v2beta1/filter.proto>`_). Example:
 
-            An example filter string would be:
+                  ::
 
-                # For the list of filter operations please see:
-                # https://github.com/kubeflow/pipelines/blob/master/sdk/python/kfp/_client.py#L40
-                json.dumps({
-                    "predicates": [{
-                        "op": _FILTER_OPERATIONS["EQUALS"],
-                        "key": "name",
-                        "stringValue": "my-name",
-                    }]
-                })
+                    json.dumps({
+                        "predicates": [{
+                            "operation": "EQUALS",
+                            "key": "display_name",
+                            "stringValue": "my-name",
+                        }]
+                    })
 
         Returns:
-          A response object including a list of versions and next page token.
-
-        Raises:
-          kfp_server_api.ApiException: If pipeline is not found.
+            ``V2beta1ListPipelineVersionsResponse`` object.
         """
 
-        return self._pipelines_api.list_pipeline_versions_v1(
+        return self._pipelines_api.list_pipeline_versions(
             page_token=page_token,
             page_size=page_size,
             sort_by=sort_by,
-            resource_key_type=kfp_server_api.models.api_resource_type
-            .ApiResourceType.PIPELINE,
-            resource_key_id=pipeline_id,
+            pipeline_id=pipeline_id,
             filter=filter)
 
-    def delete_pipeline_version(self, version_id: str):
-        """Delete pipeline version.
+    def get_pipeline_version(
+        self,
+        pipeline_id: str,
+        pipeline_version_id: str,
+    ) -> kfp_server_api.V2beta1PipelineVersion:
+        """Gets a pipeline version.
 
         Args:
-          version_id: id of the pipeline version.
+            pipeline_id: ID of the pipeline.
+            pipeline_version_id: ID of the pipeline version.
 
         Returns:
-          Object. If the method is called asynchronously, returns the request thread.
+            ``V2beta1PipelineVersion`` object.
+        """
+        return self._pipelines_api.get_pipeline_version(
+            pipeline_id=pipeline_id,
+            pipeline_version_id=pipeline_version_id,
+        )
 
-        Raises:
-          Exception if pipeline version is not found.
+    def delete_pipeline_version(
+        self,
+        pipeline_id: str,
+        pipeline_version_id: str,
+    ) -> dict:
+        """Deletes a pipeline version.p.
+
+        Args:
+            pipeline_id: ID of the pipeline.
+            pipeline_version_id: ID of the pipeline version.
+
+        Returns:
+            Empty dictionary.
         """
-        return self._pipelines_api.delete_pipeline_version_v1(
-            version_id=version_id)
+        return self._pipelines_api.delete_pipeline_version(
+            pipeline_id=pipeline_id,
+            pipeline_version_id=pipeline_version_id,
+        )
+
+
+def _add_generated_apis(
+    target_struct: Any,
+    api_module: ModuleType,
+    api_client: kfp_server_api.ApiClient,
+) -> None:
+    """Initializes a hierarchical API object based on the generated API module.
+
+    PipelineServiceApi.create_pipeline becomes
+    target_struct.pipelines.create_pipeline
+    """
+    Struct = type('Struct', (), {})
+
+    def camel_case_to_snake_case(name: str) -> str:
+        return re.sub('([a-z0-9])([A-Z])', r'\1_\2', name).lower()
+
+    for api_name in dir(api_module):
+        if not api_name.endswith('ServiceApi'):
+            continue
+
+        short_api_name = camel_case_to_snake_case(
+            api_name[0:-len('ServiceApi')]) + 's'
+        api_struct = Struct()
+        setattr(target_struct, short_api_name, api_struct)
+        service_api = getattr(api_module.api, api_name)
+        initialized_service_api = service_api(api_client)
+        for member_name in dir(initialized_service_api):
+            if member_name.startswith('_') or member_name.endswith(
+                    '_with_http_info'):
+                continue
+
+            bound_member = getattr(initialized_service_api, member_name)
+            setattr(api_struct, member_name, bound_member)
+    models_struct = Struct()
+    for member_name in dir(api_module.models):
+        if not member_name[0].islower():
+            setattr(models_struct, member_name,
+                    getattr(api_module.models, member_name))
+    target_struct.api_models = models_struct
+
+
+def validate_pipeline_resource_name(name: str) -> None:
+    REGEX = r'[a-z0-9]([-a-z0-9]*[a-z0-9])?(\\.[a-z0-9]([-a-z0-9]*[a-z0-9])?)*'
+
+    if re.fullmatch(REGEX, name) is None:
+        raise ValueError(
+            f'Invalid pipeline name: "{name}". Pipeline name must conform to the regex: "{REGEX}".'
+        )
+
+
+def _extract_pipeline_yaml(package_file: str) -> _PipelineDoc:
+
+    def _choose_pipeline_file(file_list: List[str]) -> str:
+        pipeline_files = [file for file in file_list if file.endswith('.yaml')]
+        if not pipeline_files:
+            raise ValueError(
+                'Invalid package. Missing pipeline yaml file in the package.')
+
+        if 'pipeline.yaml' in pipeline_files:
+            return 'pipeline.yaml'
+        elif len(pipeline_files) == 1:
+            return pipeline_files[0]
+        else:
+            raise ValueError(
+                'Invalid package. There is no pipeline.json file or there '
+                'are multiple yaml files.')
+
+    def _safe_load_yaml(stream: TextIO) -> _PipelineDoc:
+        docs = yaml.safe_load_all(stream)
+        pipeline_spec_dict = None
+        platform_spec_dict = {}
+        for doc in docs:
+            if pipeline_spec_dict is None:
+                pipeline_spec_dict = doc
+            else:
+                platform_spec_dict.update(doc)
+
+        return _PipelineDoc(
+            pipeline_spec=json_format.ParseDict(
+                pipeline_spec_dict, pipeline_spec_pb2.PipelineSpec()),
+            platform_spec=json_format.ParseDict(
+                platform_spec_dict, pipeline_spec_pb2.PlatformSpec()))
+
+    if package_file.endswith('.tar.gz') or package_file.endswith('.tgz'):
+        with tarfile.open(package_file, 'r:gz') as tar:
+            file_names = [member.name for member in tar if member.isfile()]
+            pipeline_file = _choose_pipeline_file(file_names)
+            with tar.extractfile(
+                    tar.getmember(pipeline_file)) as f:  # type: ignore
+                return _safe_load_yaml(f)
+    elif package_file.endswith('.zip'):
+        with zipfile.ZipFile(package_file, 'r') as zip:
+            pipeline_file = _choose_pipeline_file(zip.namelist())
+            with zip.open(pipeline_file) as f:
+                return _safe_load_yaml(f)
+    elif package_file.endswith('.yaml') or package_file.endswith('.yml'):
+        with open(package_file, 'r') as f:
+            return _safe_load_yaml(f)
+    else:
+        raise ValueError(
+            f'The package_file {package_file} should end with one of the '
+            'following formats: [.tar.gz, .tgz, .zip, .yaml, .yml].')
+
+
+def _override_caching_options(
+    pipeline_spec: pipeline_spec_pb2.PipelineSpec,
+    enable_caching: bool,
+) -> None:
+    """Overrides caching options.
+
+    Args:
+        pipeline_spec: The PipelineSpec object to update in-place.
+        enable_caching: Overrides options, one of True, False.
+    """
+    for _, task_spec in pipeline_spec.root.dag.tasks.items():
+        task_spec.caching_options.enable_cache = enable_caching
```

### Comparing `kfp-2.0.0b9/kfp/deprecated/_config.py` & `kfp-2.0.0rc1/kfp/deprecated/_config.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/_local_client.py` & `kfp-2.0.0rc1/kfp/deprecated/_local_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/_runners.py` & `kfp-2.0.0rc1/kfp/deprecated/_runners.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/auth/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/auth/_satvolumecredentials.py` & `kfp-2.0.0rc1/kfp/deprecated/auth/_satvolumecredentials.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/auth/_tokencredentialsbase.py` & `kfp-2.0.0rc1/kfp/deprecated/auth/_tokencredentialsbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/aws.py` & `kfp-2.0.0rc1/kfp/deprecated/aws.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/azure.py` & `kfp-2.0.0rc1/kfp/deprecated/azure.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/cli.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/components.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/components_test.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/components_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/dev_env.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/dev_env_test.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/dev_env_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/gcp.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/gcp_test.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/gcp_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me/kubernetes_cluster_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me/utility.py` & `kfp-2.0.0rc1/kfp/cli/diagnose_me/utility.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# Lint as: python3
 # Copyright 2019 The Kubeflow Authors. All Rights Reserved.
 #
 # Licensed under the Apache License,Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -29,37 +28,35 @@
     TODO() This class should be extended to contain data structure to better
     represent the underlying data instaed of dict for various response types.
     """
 
     def execute_command(self, command_list: List[Text]):
         """Executes the command in command_list.
 
-        sets values for _stdout,_std_err, and returncode accordingly.
+        sets values for _stdout, _stderr, and _returncode accordingly.
 
         TODO(): This method is kept in ExecutorResponse for simplicity, however this
         deviates from MVP design pattern. It should be factored out in future.
 
         Args:
           command_list: A List of strings that represts the command and parameters
             to be executed.
 
         Returns:
           Instance of utility.ExecutorResponse.
         """
 
         try:
-            # TODO() switch to process.run to simplify the code.
-            process = subprocess.Popen(
-                command_list, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-            stdout, stderr = process.communicate()
-            self._stdout = stdout.decode('utf-8')
-            self._stderr = stderr.decode('utf-8')
+            process = subprocess.run(
+                command_list, capture_output=True, check=False)
+            self._stdout = process.stdout.decode('utf-8')
+            self._stderr = process.stderr.decode('utf-8')
             self._returncode = process.returncode
         except OSError as e:
-            self._stderr = e
+            self._stderr = str(e)
             self._stdout = ''
             self._returncode = e.errno
         self._parse_raw_input()
         return self
 
     def _parse_raw_input(self):
         """Parses the raw input and popluates _json and _parsed properies."""
```

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/diagnose_me_cli.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/diagnose_me_cli.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/experiment.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/output.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/output.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/pipeline.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/recurring_run.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/recurring_run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/cli/run.py` & `kfp-2.0.0rc1/kfp/deprecated/cli/run.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/_data_passing_rewriter.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_rewriter.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/_data_passing_using_volume.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/_data_passing_using_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/_default_transformers.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/_default_transformers.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/_k8s_helper.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/_k8s_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/_op_to_template.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/_op_to_template.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/compiler.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/main.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/main.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/v2_compat.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compat.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/compiler/v2_compatible_compiler_test.py` & `kfp-2.0.0rc1/kfp/deprecated/compiler/v2_compatible_compiler_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/components/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_airflow_op.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_airflow_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_component_store.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_component_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_components.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_data_passing.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_data_passing.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_dynamic.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_dynamic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_key_value_store.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_key_value_store.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_naming.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_naming.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_python_op.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_python_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_python_to_graph_component.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_python_to_graph_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_structures.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_structures.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/_yaml_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/components/_yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/modelbase.py` & `kfp-2.0.0rc1/kfp/deprecated/components/modelbase.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/type_annotation_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/components/type_annotation_utils_test.py` & `kfp-2.0.0rc1/kfp/deprecated/components/type_annotation_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_build_image_api.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_build_image_api.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_cache.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_cache.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_component_builder.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_component_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_container_builder.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_container_builder.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_gcs_helper.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_gcs_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/_k8s_job_helper.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/_k8s_job_helper.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/entrypoint.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/containers/entrypoint_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/containers/entrypoint_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_component.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_component.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_component_bridge.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_component_bridge.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_container_op.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_container_op_test.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_container_op_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_for_loop.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_for_loop.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_metadata.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_metadata.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_ops_group.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_ops_group.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline_param.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_param.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_pipeline_volume.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_pipeline_volume.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_resource_op.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_resource_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_volume_op.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/_volume_snapshot_op.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/_volume_snapshot_op.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/artifact.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/artifact.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/artifact_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/artifact_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/component_spec.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/component_spec_test.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/component_spec_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/data_passing_methods.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/data_passing_methods.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/dsl_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/dsl_utils_test.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/dsl_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/extensions/kubernetes.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/extensions/kubernetes.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/io_types.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/io_types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/metrics_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/metrics_utils_test.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/metrics_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/serialization_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/serialization_utils_test.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/serialization_utils_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/type_utils.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/type_utils.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/dsl/types.py` & `kfp-2.0.0rc1/kfp/deprecated/dsl/types.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/gcp.py` & `kfp-2.0.0rc1/kfp/deprecated/gcp.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/notebook/__init__.py` & `kfp-2.0.0rc1/kfp/deprecated/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/notebook/_magic.py` & `kfp-2.0.0rc1/kfp/deprecated/notebook/_magic.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/deprecated/onprem.py` & `kfp-2.0.0rc1/kfp/deprecated/onprem.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/dsl/__init__.py` & `kfp-2.0.0rc1/kfp/dsl/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,26 +19,30 @@
     'container_component',
     'pipeline',
     'importer',
     'ContainerSpec',
     'Condition',
     'ExitHandler',
     'ParallelFor',
+    'Collected',
     'Input',
     'Output',
     'InputPath',
     'OutputPath',
     'IfPresentPlaceholder',
     'ConcatPlaceholder',
     'PipelineTaskFinalStatus',
     'PIPELINE_JOB_NAME_PLACEHOLDER',
     'PIPELINE_JOB_RESOURCE_NAME_PLACEHOLDER',
     'PIPELINE_JOB_ID_PLACEHOLDER',
     'PIPELINE_TASK_NAME_PLACEHOLDER',
     'PIPELINE_TASK_ID_PLACEHOLDER',
+    'PIPELINE_ROOT_PLACEHOLDER',
+    'PIPELINE_JOB_CREATE_TIME_UTC_PLACEHOLDER',
+    'PIPELINE_JOB_SCHEDULE_TIME_UTC_PLACEHOLDER',
     'Artifact',
     'ClassificationMetrics',
     'Dataset',
     'HTML',
     'Markdown',
     'Metrics',
     'Model',
@@ -51,14 +55,15 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from typing import TypeVar
 
 from kfp.components.component_decorator import component
 from kfp.components.container_component_decorator import container_component
+from kfp.components.for_loop import Collected
 from kfp.components.importer_node import importer
 from kfp.components.pipeline_context import pipeline
 from kfp.components.pipeline_task import PipelineTask
 from kfp.components.placeholders import ConcatPlaceholder
 from kfp.components.placeholders import IfPresentPlaceholder
 from kfp.components.structures import ContainerSpec
 from kfp.components.task_final_status import PipelineTaskFinalStatus
@@ -145,14 +150,28 @@
         @dsl.pipeline
         def my_pipeline():
             print_op(
                 msg='Task ID:',
                 value=dsl.PIPELINE_TASK_ID_PLACEHOLDER,
             )
 """
+
+PIPELINE_ROOT_PLACEHOLDER = '{{$.pipeline_root}}'
+"""A placeholder used to obtain the pipeline root.
+
+    Example:
+      ::
+
+        @dsl.pipeline
+        def my_pipeline():
+            store_model(
+                tmp_dir=dsl.PIPELINE_ROOT_PLACEHOLDER+'/tmp',
+            )
+"""
+
 PIPELINE_JOB_CREATE_TIME_UTC_PLACEHOLDER = '{{$.pipeline_job_create_time_utc}}'
 """A placeholder used to obtain the time that a pipeline job was created.
 
     Example:
       ::
 
         @dsl.pipeline
```

### Comparing `kfp-2.0.0b9/kfp/registry/__init__.py` & `kfp-2.0.0rc1/kfp/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/registry/context/__init__.py` & `kfp-2.0.0rc1/kfp/registry/context/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/registry/context/default_pkg_dev.json` & `kfp-2.0.0rc1/kfp/registry/context/default_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/registry/context/kfp_pkg_dev.json` & `kfp-2.0.0rc1/kfp/registry/context/kfp_pkg_dev.json`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/registry/registry_client.py` & `kfp-2.0.0rc1/kfp/registry/registry_client.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/registry/registry_client_test.py` & `kfp-2.0.0rc1/kfp/registry/registry_client_test.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/v2/__init__.py` & `kfp-2.0.0rc1/kfp/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/v2/compiler.py` & `kfp-2.0.0rc1/kfp/v2/compiler.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/v2/components.py` & `kfp-2.0.0rc1/kfp/v2/components.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp/v2/dsl.py` & `kfp-2.0.0rc1/kfp/v2/dsl.py`

 * *Files identical despite different names*

### Comparing `kfp-2.0.0b9/kfp.egg-info/PKG-INFO` & `kfp-2.0.0rc1/kfp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kfp
-Version: 2.0.0b9
+Version: 2.0.0rc1
 Summary: Kubeflow Pipelines SDK
 Home-page: https://github.com/kubeflow/pipelines
 Author: The Kubeflow Authors
 License: UNKNOWN
 Project-URL: Documentation, https://kubeflow-pipelines.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/kubeflow/pipelines/issues
 Project-URL: Source, https://github.com/kubeflow/pipelines/tree/master/sdk
@@ -65,15 +65,17 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7.0
+Requires-Python: >=3.7.0,<3.12.0
 Description-Content-Type: text/markdown
 Provides-Extra: all
+Provides-Extra: kubernetes
```

### Comparing `kfp-2.0.0b9/kfp.egg-info/SOURCES.txt` & `kfp-2.0.0rc1/kfp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 kfp/client/set_volume_credentials_test.py
 kfp/client/token_credentials_base.py
 kfp/client/token_credentials_base_test.py
 kfp/compiler/__init__.py
 kfp/compiler/compiler.py
 kfp/compiler/compiler_test.py
 kfp/compiler/compiler_utils.py
+kfp/compiler/compiler_utils_test.py
 kfp/compiler/pipeline_spec_builder.py
 kfp/compiler/pipeline_spec_builder_test.py
 kfp/compiler/read_write_test.py
 kfp/components/__init__.py
 kfp/components/base_component.py
 kfp/components/base_component_test.py
 kfp/components/component_decorator.py
@@ -213,8 +214,9 @@
 kfp/registry/registry_client_test.py
 kfp/registry/context/__init__.py
 kfp/registry/context/default_pkg_dev.json
 kfp/registry/context/kfp_pkg_dev.json
 kfp/v2/__init__.py
 kfp/v2/compiler.py
 kfp/v2/components.py
-kfp/v2/dsl.py
+kfp/v2/dsl.py
+tests/test_kfp.py
```

### Comparing `kfp-2.0.0b9/setup.py` & `kfp-2.0.0rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,17 @@
 
 def read_readme() -> str:
     readme_path = os.path.join(os.path.dirname(__file__), 'README.md')
     with open(readme_path) as f:
         return f.read()
 
 
+docker = ['docker']
+kubernetes = ['kfp-kubernetes<2']
+
 setuptools.setup(
     name='kfp',
     version=find_version('kfp', '__init__.py'),
     description='Kubeflow Pipelines SDK',
     long_description=read_readme(),
     long_description_content_type='text/markdown',
     author='The Kubeflow Authors',
@@ -70,34 +73,36 @@
         'Source':
             'https://github.com/kubeflow/pipelines/tree/master/sdk',
         'Changelog':
             'https://github.com/kubeflow/pipelines/blob/master/sdk/RELEASE.md',
     },
     install_requires=get_requirements('requirements.in'),
     extras_require={
-        'all': ['docker'],
+        'all': docker + kubernetes,
+        'kubernetes': kubernetes,
     },
     packages=setuptools.find_packages(exclude=['*test*']),
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Software Development',
         'Topic :: Software Development :: Libraries',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
-    python_requires='>=3.7.0',
+    python_requires='>=3.7.0,<3.12.0',
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'dsl-compile = kfp.cli.compile_:main',
             'dsl-compile-deprecated = kfp.deprecated.compiler.main:main',
             'kfp=kfp.cli.__main__:main',
         ]
```

