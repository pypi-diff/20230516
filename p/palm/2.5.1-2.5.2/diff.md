# Comparing `tmp/palm-2.5.1.tar.gz` & `tmp/palm-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "palm-2.5.1.tar", last modified: Wed Nov 23 18:44:44 2022, max compression
+gzip compressed data, was "palm-2.5.2.tar", last modified: Thu Mar 16 16:41:19 2023, max compression
```

## Comparing `palm-2.5.1.tar` & `palm-2.5.2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-11-23 18:44:44.893800 palm-2.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1460 2022-11-23 18:44:35.000000 palm-2.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:35.000000 palm-2.5.1/palm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5293 2022-11-23 18:44:35.000000 palm-2.5.1/palm/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2971 2022-11-23 18:44:35.000000 palm-2.5.1/palm/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6251 2022-11-23 18:44:35.000000 palm-2.5.1/palm/containerizer.py
--rw-r--r--   0 runner    (1001) docker     (121)     4615 2022-11-23 18:44:35.000000 palm-2.5.1/palm/environment.py
--rw-r--r--   0 runner    (1001) docker     (121)     6028 2022-11-23 18:44:35.000000 palm-2.5.1/palm/palm_config.py
--rw-r--r--   0 runner    (1001) docker     (121)      370 2022-11-23 18:44:35.000000 palm-2.5.1/palm/palm_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2945 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugin_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm/plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3262 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/base_plugin_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm/plugins/core/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm/plugins/core/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_build.py
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_containerize.py
--rw-r--r--   0 runner    (1001) docker     (121)     1745 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_init.py
--rw-r--r--   0 runner    (1001) docker     (121)      220 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_lint.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_override.py
--rw-r--r--   0 runner    (1001) docker     (121)     4508 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)     2182 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_scaffold.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_shell.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      760 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/commands/cmd_update.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/core_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/create_files.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm/plugins/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/core/templates/command/
--rw-r--r--   0 runner    (1001) docker     (121)      331 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/command/new_cmd.tpl.py
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/command/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/core/templates/command_group/
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/command_group/new_cmd_group.tpl.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/command_group/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/core/templates/containerize/
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/containerize/Dockerfile.txt
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/containerize/docker-compose.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/containerize/entrypoint.sh.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/containerize/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/core/templates/plugin/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/plugin/empty_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/plugin/plugin_init.tpl.py
--rw-r--r--   0 runner    (1001) docker     (121)      439 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/plugin/plugin_template.tpl.py
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/plugin/setup.tpl.py
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/core/templates/plugin/template-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/repo/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/repo/repo_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/setup/
--rw-r--r--   0 runner    (1001) docker     (121)       60 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/setup/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/setup/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     2026 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/setup/commands/cmd_new.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/setup/setup_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/test_internal/
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/test_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.893800 palm-2.5.1/palm/plugins/test_internal/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/test_internal/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/test_internal/commands/cmd_run.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-11-23 18:44:35.000000 palm-2.5.1/palm/plugins/test_internal/test_internal_plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)      911 2022-11-23 18:44:35.000000 palm-2.5.1/palm/project_setup_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1596 2022-11-23 18:44:35.000000 palm-2.5.1/palm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-23 18:44:44.889800 palm-2.5.1/palm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2300 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2110 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-11-23 18:44:44.000000 palm-2.5.1/palm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-23 18:44:44.893800 palm-2.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1477 2022-11-23 18:44:35.000000 palm-2.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-16 16:41:11.000000 palm-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-16 16:41:19.347770 palm-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-03-16 16:41:11.000000 palm-2.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.339770 palm-2.5.2/palm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:11.000000 palm-2.5.2/palm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-03-16 16:41:11.000000 palm-2.5.2/palm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-03-16 16:41:11.000000 palm-2.5.2/palm/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-03-16 16:41:11.000000 palm-2.5.2/palm/containerizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-16 16:41:11.000000 palm-2.5.2/palm/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-03-16 16:41:11.000000 palm-2.5.2/palm/palm_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-03-16 16:41:11.000000 palm-2.5.2/palm/palm_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugin_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.343770 palm-2.5.2/palm/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/base_plugin_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.343770 palm-2.5.2/palm/plugins/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/core/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_containerize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4508 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_scaffold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/commands/cmd_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/core_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/create_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.335770 palm-2.5.2/palm/plugins/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/core/templates/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/command/new_cmd.tpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/command/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/core/templates/command_group/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/command_group/new_cmd_group.tpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/command_group/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/core/templates/containerize/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/containerize/Dockerfile.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/containerize/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/containerize/entrypoint.sh.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/containerize/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/core/templates/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/plugin/empty_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/plugin/plugin_init.tpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/plugin/plugin_template.tpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/plugin/setup.tpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/core/templates/plugin/template-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/repo/repo_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/setup/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/setup/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/setup/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/setup/commands/cmd_new.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/setup/setup_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/test_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/test_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.347770 palm-2.5.2/palm/plugins/test_internal/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/test_internal/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/test_internal/commands/cmd_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-16 16:41:11.000000 palm-2.5.2/palm/plugins/test_internal/test_internal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-16 16:41:11.000000 palm-2.5.2/palm/project_setup_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-16 16:41:11.000000 palm-2.5.2/palm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 16:41:19.343770 palm-2.5.2/palm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-16 16:41:19.000000 palm-2.5.2/palm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 16:41:19.347770 palm-2.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-03-16 16:41:11.000000 palm-2.5.2/setup.py
```

### Comparing `palm-2.5.1/PKG-INFO` & `palm-2.5.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 Metadata-Version: 2.1
 Name: palm
-Version: 2.5.1
+Version: 2.5.2
 Summary: Palm CLI
 Home-page: https://github.com/palmetto/palm-cli
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
-Description: # Palm CLI: The extensible CLI at your fingertips
-        
-        _Palm_ is a universal CLI developed to improve the life and work of data professionals.
-        
-        [Palm CLI documentation](https://palm-cli.readthedocs.io/en/latest/)
-        
-        ## Installing Palm
-        
-        ```bash
-        pip install palm
-        ```
-        
-        **note for mac users**: if you get this warning:
-        
-        ```bash
-          WARNING: The script palm is installed in '/Users/yourname/Library/Python/3.8/bin' which is not on PATH.
-          Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
-        ```
-        
-        you will need to add `'/Users/yourname/Library/Python/3.8/bin'` to your path for `palm` to work.
-        
-        you can do that with this command:
-        
-        ```bash
-        echo "\nexport PATH=$PATH:/Users/yourname/Library/Python/3.8/bin\n" >> ~/.zprofile
-        ```
-        
-        ### Upgrading palm
-        
-        To upgrade palm to the latest version, use `pip install palm -U`
-        
-        ### Requirements
-        
-        1. You will need [Docker](https://docs.docker.com/get-docker/)
-           You can check to see if you already have it with `docker --version`
-        
-        2. You will need [Python3](https://www.python.org/downloads/)
-           You can check to see if you already have it with `python3 --version`
-        
-        ### Developing palm
-        
-        **If you have the repo on your computer** This will install whatever version you have checked out at the moment.
-        
-        ```bash
-        cd path/to/this/repo &&
-        python3 -m pip uninstall palm || true # for new installs
-        python3 -m pip install .
-        ```
-        
-        You can verify the install with
-        
-        ```bash
-        palm --help
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Palm CLI: The extensible CLI at your fingertips
+
+_Palm_ is a universal CLI developed to improve the life and work of data professionals.
+
+[Palm CLI documentation](https://palm-cli.readthedocs.io/en/latest/)
+
+## Installing Palm
+
+```bash
+pip install palm
+```
+
+**note for mac users**: if you get this warning:
+
+```bash
+  WARNING: The script palm is installed in '/Users/yourname/Library/Python/3.8/bin' which is not on PATH.
+  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+you will need to add `'/Users/yourname/Library/Python/3.8/bin'` to your path for `palm` to work.
+
+you can do that with this command:
+
+```bash
+echo "\nexport PATH=$PATH:/Users/yourname/Library/Python/3.8/bin\n" >> ~/.zprofile
+```
+
+### Upgrading palm
+
+To upgrade palm to the latest version, use `pip install palm -U`
+
+### Requirements
+
+1. You will need [Docker](https://docs.docker.com/get-docker/)
+   You can check to see if you already have it with `docker --version`
+
+2. You will need [Python3](https://www.python.org/downloads/)
+   You can check to see if you already have it with `python3 --version`
+
+### Developing palm
+
+**If you have the repo on your computer** This will install whatever version you have checked out at the moment.
+
+```bash
+cd path/to/this/repo &&
+python3 -m pip uninstall palm || true # for new installs
+python3 -m pip install .
+```
+
+You can verify the install with
+
+```bash
+palm --help
+```
+
+
```

### Comparing `palm-2.5.1/README.md` & `palm-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/cli.py` & `palm-2.5.2/palm/cli.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/code_generator.py` & `palm-2.5.2/palm/code_generator.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/containerizer.py` & `palm-2.5.2/palm/containerizer.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/environment.py` & `palm-2.5.2/palm/environment.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/palm_config.py` & `palm-2.5.2/palm/palm_config.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugin_manager.py` & `palm-2.5.2/palm/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/base.py` & `palm-2.5.2/palm/plugins/base.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/base_plugin_config.py` & `palm-2.5.2/palm/plugins/base_plugin_config.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_containerize.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_containerize.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_init.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_init.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_override.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_override.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_plugin.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_plugin.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_scaffold.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_scaffold.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/commands/cmd_update.py` & `palm-2.5.2/palm/plugins/core/commands/cmd_update.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/create_files.py` & `palm-2.5.2/palm/plugins/core/create_files.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/core/templates/plugin/setup.tpl.py` & `palm-2.5.2/palm/plugins/core/templates/plugin/setup.tpl.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/plugins/setup/commands/cmd_new.py` & `palm-2.5.2/palm/plugins/setup/commands/cmd_new.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/project_setup_utils.py` & `palm-2.5.2/palm/project_setup_utils.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm/utils.py` & `palm-2.5.2/palm/utils.py`

 * *Files identical despite different names*

### Comparing `palm-2.5.1/palm.egg-info/PKG-INFO` & `palm-2.5.2/palm.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,67 +1,70 @@
 Metadata-Version: 2.1
 Name: palm
-Version: 2.5.1
+Version: 2.5.2
 Summary: Palm CLI
 Home-page: https://github.com/palmetto/palm-cli
 Author: Palmetto - Data & Analytics team
 Author-email: data-analytics-team@palmetto.com
 License: Apache License 2.0
-Description: # Palm CLI: The extensible CLI at your fingertips
-        
-        _Palm_ is a universal CLI developed to improve the life and work of data professionals.
-        
-        [Palm CLI documentation](https://palm-cli.readthedocs.io/en/latest/)
-        
-        ## Installing Palm
-        
-        ```bash
-        pip install palm
-        ```
-        
-        **note for mac users**: if you get this warning:
-        
-        ```bash
-          WARNING: The script palm is installed in '/Users/yourname/Library/Python/3.8/bin' which is not on PATH.
-          Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
-        ```
-        
-        you will need to add `'/Users/yourname/Library/Python/3.8/bin'` to your path for `palm` to work.
-        
-        you can do that with this command:
-        
-        ```bash
-        echo "\nexport PATH=$PATH:/Users/yourname/Library/Python/3.8/bin\n" >> ~/.zprofile
-        ```
-        
-        ### Upgrading palm
-        
-        To upgrade palm to the latest version, use `pip install palm -U`
-        
-        ### Requirements
-        
-        1. You will need [Docker](https://docs.docker.com/get-docker/)
-           You can check to see if you already have it with `docker --version`
-        
-        2. You will need [Python3](https://www.python.org/downloads/)
-           You can check to see if you already have it with `python3 --version`
-        
-        ### Developing palm
-        
-        **If you have the repo on your computer** This will install whatever version you have checked out at the moment.
-        
-        ```bash
-        cd path/to/this/repo &&
-        python3 -m pip uninstall palm || true # for new installs
-        python3 -m pip install .
-        ```
-        
-        You can verify the install with
-        
-        ```bash
-        palm --help
-        ```
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Palm CLI: The extensible CLI at your fingertips
+
+_Palm_ is a universal CLI developed to improve the life and work of data professionals.
+
+[Palm CLI documentation](https://palm-cli.readthedocs.io/en/latest/)
+
+## Installing Palm
+
+```bash
+pip install palm
+```
+
+**note for mac users**: if you get this warning:
+
+```bash
+  WARNING: The script palm is installed in '/Users/yourname/Library/Python/3.8/bin' which is not on PATH.
+  Consider adding this directory to PATH or, if you prefer to suppress this warning, use --no-warn-script-location.
+```
+
+you will need to add `'/Users/yourname/Library/Python/3.8/bin'` to your path for `palm` to work.
+
+you can do that with this command:
+
+```bash
+echo "\nexport PATH=$PATH:/Users/yourname/Library/Python/3.8/bin\n" >> ~/.zprofile
+```
+
+### Upgrading palm
+
+To upgrade palm to the latest version, use `pip install palm -U`
+
+### Requirements
+
+1. You will need [Docker](https://docs.docker.com/get-docker/)
+   You can check to see if you already have it with `docker --version`
+
+2. You will need [Python3](https://www.python.org/downloads/)
+   You can check to see if you already have it with `python3 --version`
+
+### Developing palm
+
+**If you have the repo on your computer** This will install whatever version you have checked out at the moment.
+
+```bash
+cd path/to/this/repo &&
+python3 -m pip uninstall palm || true # for new installs
+python3 -m pip install .
+```
+
+You can verify the install with
+
+```bash
+palm --help
+```
+
+
```

### Comparing `palm-2.5.1/palm.egg-info/SOURCES.txt` & `palm-2.5.2/palm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 palm/__init__.py
 palm/cli.py
 palm/code_generator.py
 palm/containerizer.py
 palm/environment.py
```

### Comparing `palm-2.5.1/setup.py` & `palm-2.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # User-friendly description from README.md
 this_directory = Path(__file__).parent
 long_description = Path(this_directory, "README.md").read_text()
 
 setup(
     name="palm",
-    version="2.5.1",  # Don't forget to bump the version in docs/source/conf.py too!
+    version="2.5.2",  # Don't forget to bump the version in docs/source/conf.py too!
     description="Palm CLI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Palmetto - Data & Analytics team",
     author_email="data-analytics-team@palmetto.com",
     url="https://github.com/palmetto/palm-cli",
     # Packages to include into the distribution
```

