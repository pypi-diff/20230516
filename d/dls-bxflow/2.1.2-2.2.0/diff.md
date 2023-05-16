# Comparing `tmp/dls-bxflow-2.1.2.tar.gz` & `tmp/dls-bxflow-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-2.1.2.tar", last modified: Fri Feb 17 10:43:44 2023, max compression
+gzip compressed data, was "dls-bxflow-2.2.0.tar", last modified: Tue May 16 13:40:42 2023, max compression
```

## Comparing `dls-bxflow-2.1.2.tar` & `dls-bxflow-2.2.0.tar`

### file list

```diff
@@ -1,426 +1,426 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.315130 dls-bxflow-2.1.2/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.315130 dls-bxflow-2.1.2/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.315130 dls-bxflow-2.1.2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.315130 dls-bxflow-2.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.303130 dls-bxflow-2.1.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.315130 dls-bxflow-2.1.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.307130 dls-bxflow-2.1.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/_static/css/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/api/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/api/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.319130 dls-bxflow-2.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3772 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.311130 dls-bxflow-2.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/remex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_api/things.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.323130 dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/dataface_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/news_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.327130 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/execute_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/find_xanes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/fire_i22.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/report_dcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/report_ispyb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.327130 dls-bxflow-2.1.2/src/dls_bxflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-02-17 10:43:44.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.327130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/ispyb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.331130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/gdascan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.331130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/bx_composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.331130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.335130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.335130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/bx_databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.335130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    28516 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/news_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.335130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/scandir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.335130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40092 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/bx_guis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/curses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.339130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.343130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.343130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.311130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.343130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.311130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.347130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.311130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.347130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.347130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.347130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.351130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.351130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/island.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/popener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/qsubber.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.355130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/graylogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.355130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/bx_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.355130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/zocalo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.359130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/bx_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.359130 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19288 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.359130 dls-bxflow-2.1.2/src/dls_bxflow_lib/dummies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/dummies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/dummies/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.359130 dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/overall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/parser1.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.359130 dls-bxflow-2.1.2/src/dls_bxflow_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.363130 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/bx_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.363130 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/bx_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/filename_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/module_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/pickled_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/symlink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.367130 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/bx_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/src/dls_bxflow_run/main_isolated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.375130 dls-bxflow-2.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.375130 dls-bxflow-2.1.2/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/configurations/backend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/configurations/filestore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/configurations/ispyb-local.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.375130 dls-bxflow-2.1.2/tests/configurations/ptypy_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.375130 dls-bxflow-2.1.2/tests/configurations/ptyrex_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/configurations/ptyrex_configfiles/region_p4_p6.json
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.375130 dls-bxflow-2.1.2/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/datafiles/dawn2_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.311130 dls-bxflow-2.1.2/tests/datafiles/gaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/datafiles/gaml/workflow1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/datafiles/gaml/workflow1/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/datafiles/gaml/workflow2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/datafiles/gaml/workflow2/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/datafiles/i22-4996.nxs
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/gda_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/gda_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/jupyter/execute.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/jupyter/jupyter1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/jupyter/jupyter_bad_cell.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/notebooks/c.ipynb
--rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/qacct
--rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/qstat
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/qsub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/stub_commands/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/stub_commands/dawn
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/stub_commands/mpirun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/stub_commands/ptychotools.ptypy_mpi_recipe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_collector_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_extract_error_lines_dawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_extract_error_lines_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_gaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_job_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_job_a_bc_d.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_job_pubcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_job_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9588 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_launcher_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_launcher_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_launcher_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_launcher_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_logstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_protocolj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_scheduler_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/test_workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.379130 dls-bxflow-2.1.2/tests/workflows/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/a/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/tests/workflows/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/b/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/tests/workflows/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/c/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/tests/workflows/e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/e/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/tests/workflows/f/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/f/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/f/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:44.383130 dls-bxflow-2.1.2/tests/workflows/g/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/g/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-17 10:43:32.000000 dls-bxflow-2.1.2/tests/workflows/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/_static/css/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13933 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13273 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/remex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_api/things.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.631035 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/dataface_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/news_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/find_xanes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/fire_i22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_dcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 13:40:42.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12963 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16315 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.635035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16023 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10912 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5744 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23673 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28516 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/scandir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40092 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/curses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.639035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.623035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.643035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23146 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/island.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/popener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20536 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.647035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/bx_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10211 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19291 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/overall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/parser1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.651035 dls-bxflow-2.2.0/src/dls_bxflow_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/bx_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13556 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5369 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11617 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/module_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/symlink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.655035 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/bx_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/src/dls_bxflow_run/main_isolated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7855 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12460 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/backend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/filestore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ispyb-local.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.659036 dls-bxflow-2.2.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/dawn2_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.627035 dls-bxflow-2.2.0/tests/datafiles/gaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow1/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/gaml/workflow2/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/datafiles/i22-4996.nxs
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/gda_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/gda_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/execute.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/jupyter1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/jupyter/jupyter_bad_cell.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/notebooks/c.ipynb
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1800 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qacct
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qstat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/qsub
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/stub_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/dawn
+-rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/mpirun
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_collector_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_extract_error_lines_dawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_extract_error_lines_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_gaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9462 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_a_bc_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_pubcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_job_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12969 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7819 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10618 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_launcher_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_logstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_protocolj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_scheduler_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/test_workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.663035 dls-bxflow-2.2.0/tests/workflows/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/a/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/b/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/c/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/e/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/f/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/f/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/f/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:42.667036 dls-bxflow-2.2.0/tests/workflows/g/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/g/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-16 13:40:31.000000 dls-bxflow-2.2.0/tests/workflows/utilities.py
```

### Comparing `dls-bxflow-2.1.2/.dae-devops/Makefile` & `dls-bxflow-2.2.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/conventions.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/developing.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/devops.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/docs_structure.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/installing.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/docs/testing.rst` & `dls-bxflow-2.2.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.dae-devops/project.yaml` & `dls-bxflow-2.2.0/.dae-devops/project.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
   dependencies:
     - type: pypi
       list:
         - aio-pika
         - dask[distributed]
         - dls-servbase
         - dls-mainiac
+        - dls-multiconf
         - dls-utilpack
         - dls-pairstream
         - future
         - graypy
         - h5py
         # There is a newer version 7 of ispyb but it doesn't support the import ispyb.model.__future__.
         # TODO: Change away from using import ispyb.model.__future__.
```

### Comparing `dls-bxflow-2.1.2/.devcontainer/Dockerfile` & `dls-bxflow-2.2.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.devcontainer/devcontainer.json` & `dls-bxflow-2.2.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/CONTRIBUTING.rst` & `dls-bxflow-2.2.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/actions/install_requirements/action.yml` & `dls-bxflow-2.2.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/dependabot.yml` & `dls-bxflow-2.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/pages/make_switcher.py` & `dls-bxflow-2.2.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/workflows/code.yml` & `dls-bxflow-2.2.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/workflows/docs.yml` & `dls-bxflow-2.2.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/workflows/docs_clean.yml` & `dls-bxflow-2.2.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.github/workflows/linkcheck.yml` & `dls-bxflow-2.2.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.gitignore` & `dls-bxflow-2.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.gitlab-ci.yml` & `dls-bxflow-2.2.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/.vscode/launch.json` & `dls-bxflow-2.2.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/LICENSE` & `dls-bxflow-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/PKG-INFO` & `dls-bxflow-2.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.1.2
+Version: 2.2.0
 Summary: Distributed beamline data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.1.2/README.rst` & `dls-bxflow-2.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/docs/conf.py` & `dls-bxflow-2.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/docs/images/dls-favicon.ico` & `dls-bxflow-2.2.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/docs/images/dls-logo.svg` & `dls-bxflow-2.2.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/pyproject.toml` & `dls-bxflow-2.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,39 @@
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Distributed beamline data processing workflow engine and gui platform core."
-dependencies = ["aio-pika", "dask[distributed]", "dls-servbase", "dls-mainiac", "dls-utilpack", "dls-pairstream", "future", "graypy", "h5py", "ispyb==6.13.0", "ipykernel", "jsonpickle", "lxml", "nbclient", "nbconvert", "nbformat", "pika", "prettytable", "pyyaml", "ruamel.yaml", "stomp.py", "workflows"]
+dependencies = [
+    "aio-pika",
+    "dask[distributed]",
+    "dls-servbase",
+    "dls-mainiac",
+    "dls-multiconf",
+    "dls-utilpack",
+    "dls-pairstream",
+    "future",
+    "graypy",
+    "h5py",
+    "ispyb==6.13.0",
+    "ipykernel",
+    "jsonpickle",
+    "lxml",
+    "nbclient",
+    "nbconvert",
+    "nbformat",
+    "pika",
+    "prettytable",
+    "pyyaml",
+    "ruamel.yaml",
+    "stomp.py",
+    "workflows",
+]
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.rst"
 requires-python = ">=3.9"
 
 [project.optional-dependencies]
 dev = [
@@ -30,14 +54,15 @@
     "Flake8-pyproject",
     "pipdeptree",
     "pre-commit",
     "pytest-cov",
     "pydocstyle[toml]",
     "tox-direct",
     "types-mock",
+    "types-PyYAML",
 ]
 docs = [
     "pydata-sphinx-theme>=0.12",
     "sphinx-argparse",
     "sphinx-autobuild",
     "sphinx-copybutton",
     "sphinx-design",
@@ -80,15 +105,15 @@
 ]
 max-line-length = 88 # Respect black's line length (default 88),
 exclude = [".tox", "venv"]
 
 
 [tool.pytest.ini_options]
 # Run pytest with all our checkers, and don't spam us with massive tracebacks on error
-addopts = "    --tb=native -vv --doctest-modules --doctest-glob=\"*.rst\"\n    --cov=dls_bxflow_lib --cov-report term --cov-report xml:cov.xml\n    "
+addopts = "    --tb=native -vv --doctest-modules --doctest-glob=\"*.rst\"\n    "
 # https://iscinumpy.gitlab.io/post/bound-version-constraints/#watch-for-warnings
 filterwarnings = "error"
 # Doctest python code in docs, python code in src docstrings, test functions in tests
 testpaths = "docs src tests"
 
 [tool.coverage.run]
 data_file = "/tmp/dls_bxflow_lib.coverage"
@@ -98,8 +123,8 @@
 source = ["src", "**/site-packages/"]
 
 # tox must currently be configured via an embedded ini string
 # See: https://github.com/tox-dev/tox/issues/999
 [tool.tox]
 legacy_tox_ini = "[tox]\nskipsdist=True\n\n[testenv:{pre-commit,mypy,pytest,docs}]\n# Don't create a virtualenv for the command, requires tox-direct plugin\ndirect = True\npassenv = *\nallowlist_externals = \n    pytest \n    pre-commit\n    mypy\n    sphinx-build\n    sphinx-autobuild\ncommands =\n    pytest: pytest {posargs}\n    mypy: mypy src tests {posargs}\n    pre-commit: pre-commit run --all-files {posargs}\n    docs: sphinx-{posargs:build -EW --keep-going} -T docs build/html\n"
 
-# dae_devops_fingerprint b97e16b96e68ca07d6deb43f26bc64ee
+# dae_devops_fingerprint 32c67ec7b2a3de3d46988bba8c8821ef
```

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow.egg-info/PKG-INFO` & `dls-bxflow-2.2.0/src/dls_bxflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.1.2
+Version: 2.2.0
 Summary: Distributed beamline data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow.egg-info/SOURCES.txt` & `dls-bxflow-2.2.0/src/dls_bxflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/bx_databases/constants.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_databases/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/bx_datafaces/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/exceptions.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/remex.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/remex.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/thing.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/thing.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_api/things.py` & `dls-bxflow-2.2.0/src/dls_bxflow_api/things.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/dataface_client.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/dataface_client.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/filestore.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/contexts/news_consumer.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/contexts/news_consumer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/main.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/execute_workflow.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/find_xanes.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/find_xanes.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/fire_i22.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/fire_i22.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/recipe_parser.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/recipe_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/report_dcg.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_dcg.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/report_ispyb.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/report_ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/start_services.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/subcommands/submit.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/subcommands/submit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_cli/version.py` & `dls-bxflow-2.2.0/src/dls_bxflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/__main__.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_catalogs/ispyb.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/bx_collectors.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/gdascan.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/gdascan.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/manual.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/manual.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_collectors/scraper.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_collectors/scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/bx_composers.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/bx_composers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/html.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/prettyhelper.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_composers/text.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_composers/text.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_configurators/yaml.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_configurators/yaml.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/bx_contexts.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_contexts/classic.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/aiosqlite.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_databases/bx_databases.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_databases/bx_databases.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_datafaces/news_producer.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/bx_filestores.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/explicit.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/explicit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_filestores/scandir.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_filestores/scandir.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/bx_gamls.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_gamls/html.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_gamls/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/bx_guis.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/bx_guis.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/constants.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/curses.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/curses.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/css/styles.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/index.html` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/index.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/bx_jobs.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_jobs/standard.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_jobs/standard.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/bx_launchers.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/island.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/island.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/popener.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/popener.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_launchers/qsubber.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_launchers/qsubber.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/bx_logstores.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_logstores/graylogger.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_logstores/graylogger.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/aio_pika.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aio_pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/bx_news.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/bx_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/constants.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/pika.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_news/zmq_pubsub.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/aiohttp.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/context.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/dask.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/dask.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/naive.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_schedulers/zocalo.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/boolean.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/boolean.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/bx_settings.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/bx_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/float.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/float.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/integer.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/integer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_settings/string.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_settings/string.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import copy
 import json
 import logging
 import sys
 
+# Exceptions.
+from dls_multiconf_lib.exceptions import NotFound
+
 # Utilities.
 from dls_utilpack.callsign import callsign
 from dls_utilpack.explain import explain2
 from dls_utilpack.require import require
 
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
-# Exceptions.
-from dls_bxflow_api.exceptions import NotFound
-
 # Remote execution.
 from dls_bxflow_api.remex import Clusters as RemexClusters
 from dls_bxflow_api.remex import Keywords as RemexKeywords
 
 # Configurator.
 from dls_bxflow_lib.bx_configurators.bx_configurators import (
     bx_configurators_get_default,
```

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/main.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/notebook_helper.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/bx_workflows/workflow_finder.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/dummies/writer.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/dummies/writer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/envvar.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/overall.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/overall.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/recipe_parser/parser1.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/recipe_parser/parser1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_lib/version.py` & `dls-bxflow-2.2.0/src/dls_bxflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_gates/bx_gates.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_gates/bx_gates.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/bx_tasks.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/constants.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn1.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn2.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dawn_base.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dawn_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/dummy.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/filename_classname.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/filename_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/jupyter.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/module_classname.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/module_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/pickled_class.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/pickled_class.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/shell.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_tasks/symlink.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_tasks/symlink.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/bx_variables/bx_variables.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/bx_variables/bx_variables.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/src/dls_bxflow_run/main_isolated.py` & `dls-bxflow-2.2.0/src/dls_bxflow_run/main_isolated.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/base.py` & `dls-bxflow-2.2.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/base_context_tester.py` & `dls-bxflow-2.2.0/tests/base_context_tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import logging
 import multiprocessing
 import os
 
 import pytest
+from dls_multiconf_lib.constants import ThingTypes as MulticonfThingTypes
 
 # Object managers we interact with.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Results composers.
 from dls_bxflow_lib.bx_composers.bx_composers import BxComposers
 
@@ -66,15 +67,15 @@
             pytest.fail(failure_message)
 
     # ----------------------------------------------------------------------------------------
     def get_bx_configurator(self):
 
         bx_configurator = BxConfigurators().build_object(
             {
-                "type": "dls_bxflow_lib.bx_configurators.yaml",
+                "type": MulticonfThingTypes.YAML,
                 "type_specific_tbd": {"filename": self.__configuration_file},
             }
         )
 
         # For convenience, always do these replacement.
         bx_configurator.substitute({"output_directory": self.__output_directory})
         bx_configurator.substitute({"temporary_directory": self.__output_directory})
```

### Comparing `dls-bxflow-2.1.2/tests/base_specification_tester.py` & `dls-bxflow-2.2.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/base_tester.py` & `dls-bxflow-2.2.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/configurations/backend.yaml` & `dls-bxflow-2.2.0/tests/configurations/backend.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/configurations/filestore.yaml` & `dls-bxflow-2.2.0/tests/configurations/filestore.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml` & `dls-bxflow-2.2.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/configurations/ptyrex_configfiles/region_p4_p6.json` & `dls-bxflow-2.2.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/conftest.py` & `dls-bxflow-2.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/datafiles/dawn2_configuration.json` & `dls-bxflow-2.2.0/tests/datafiles/dawn2_configuration.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/datafiles/i22-4996.nxs` & `dls-bxflow-2.2.0/tests/datafiles/i22-4996.nxs`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/gda_parser.py` & `dls-bxflow-2.2.0/tests/gda_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/gda_workflow.py` & `dls-bxflow-2.2.0/tests/gda_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/jupyter/jupyter1.ipynb` & `dls-bxflow-2.2.0/tests/jupyter/jupyter1.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/jupyter/jupyter_bad_cell.ipynb` & `dls-bxflow-2.2.0/tests/jupyter/jupyter_bad_cell.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/notebooks/c.ipynb` & `dls-bxflow-2.2.0/tests/notebooks/c.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/qacct` & `dls-bxflow-2.2.0/tests/qacct`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/qstat` & `dls-bxflow-2.2.0/tests/qstat`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/stub_commands/ptychotools.ptypy_mpi_recipe` & `dls-bxflow-2.2.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_catalog.py` & `dls-bxflow-2.2.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_collector.py` & `dls-bxflow-2.2.0/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_collector_scraper.py` & `dls-bxflow-2.2.0/tests/test_collector_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_composer.py` & `dls-bxflow-2.2.0/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_configurator.py` & `dls-bxflow-2.2.0/tests/test_configurator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import asyncio
 import logging
 import multiprocessing
 import os
 
 import pytest
 import yaml
+from dls_multiconf_lib.constants import ThingTypes as MulticonfThingTypes
+
+# Exceptions.
+from dls_multiconf_lib.exceptions import NotFound
 
 # Utilities.
 from dls_utilpack.describe import describe
 
-# Exceptions.
-from dls_bxflow_api.exceptions import NotFound
-
 # Configurator.
 from dls_bxflow_lib.bx_configurators.bx_configurators import BxConfigurators
 
 # Environment variables with some extra functionality.
 from dls_bxflow_lib.envvar import Envvar
 
 logger = logging.getLogger(__name__)
@@ -38,15 +39,15 @@
         with open(yaml_filename, "w") as yaml_stream:
             yaml.dump(
                 configuration, yaml_stream, default_flow_style=False, sort_keys=False
             )
 
         # This is the object type we want to run the test on.
         specification = {
-            "type": "dls_bxflow_lib.bx_configurators.yaml",
+            "type": MulticonfThingTypes.YAML,
             "type_specific_tbd": {"filename": yaml_filename},
         }
 
         # Run the test in a coroutine.
         GoodConfiguratorDirectTester().main(constants, specification, output_directory)
 
 
@@ -57,22 +58,22 @@
 
         # Run the bad tests in a coroutine.
         BadConfiguratorDirectTester("RuntimeError", "does not contain keyword").main(
             constants, {}, output_directory
         )
         BadConfiguratorDirectTester("RuntimeError", "unable to instantiate").main(
             constants,
-            {"type": "dls_bxflow_lib.bx_configurators.yaml"},
+            {"type": MulticonfThingTypes.YAML},
             output_directory,
         )
 
         # Another yaml file.
         bad_yaml_filename = f"{output_directory}/configuration.bad.yml"
         specification = {
-            "type": "dls_bxflow_lib.bx_configurators.yaml",
+            "type": MulticonfThingTypes.YAML,
             "type_specific_tbd": {"filename": bad_yaml_filename},
         }
 
         BadConfiguratorDirectTester("RuntimeError", "unable to read").main(
             constants,
             specification,
             output_directory,
```

### Comparing `dls-bxflow-2.1.2/tests/test_database.py` & `dls-bxflow-2.2.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_dataface.py` & `dls-bxflow-2.2.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_dawn1.py` & `dls-bxflow-2.2.0/tests/test_dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_dawn2.py` & `dls-bxflow-2.2.0/tests/test_dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_extract_error_lines_dawn.py` & `dls-bxflow-2.2.0/tests/test_extract_error_lines_dawn.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_extract_error_lines_dummy.py` & `dls-bxflow-2.2.0/tests/test_extract_error_lines_dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_filestore.py` & `dls-bxflow-2.2.0/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_gaml.py` & `dls-bxflow-2.2.0/tests/test_gaml.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_gui.py` & `dls-bxflow-2.2.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_job_a.py` & `dls-bxflow-2.2.0/tests/test_job_a.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_job_a_bc_d.py` & `dls-bxflow-2.2.0/tests/test_job_a_bc_d.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_job_pubcon.py` & `dls-bxflow-2.2.0/tests/test_job_pubcon.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_job_x.py` & `dls-bxflow-2.2.0/tests/test_job_x.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_jupyter.py` & `dls-bxflow-2.2.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_launcher.py` & `dls-bxflow-2.2.0/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_launcher_capacity.py` & `dls-bxflow-2.2.0/tests/test_launcher_capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import asyncio
 import copy
 import json
 import logging
 import os
 import time
 
-# Utilities.
-from dls_utilpack.qualname import qualname
-
 # Object managing datafaces.
 from dls_bxflow_api.bx_datafaces.bx_datafaces import bx_datafaces_get_default
 
 # Exceptions.
 from dls_bxflow_api.exceptions import CapacityReached
 
 # Remote execution.
@@ -175,21 +172,16 @@
                             await launcher.submit(
                                 bx_job_uuid,
                                 bx_job_specification,
                                 bx_task_uuid % (i),
                                 bx_task_specifications[i],
                             )
                             break
-                        except Exception as exception:
-                            if qualname(CapacityReached) in str(exception):
-                                logger.info(
-                                    f"general {exception}, will nap and try again"
-                                )
-                            else:
-                                raise
+                        except CapacityReached as exception:
+                            logger.info(f"general {exception}, will nap and try again")
 
                         await asyncio.sleep(nap)
 
                         if time.time() - time0 > timeout:
                             raise RuntimeError(
                                 f"bx_tasks submission not finished within {timeout} seconds"
                             )
```

### Comparing `dls-bxflow-2.1.2/tests/test_launcher_direct.py` & `dls-bxflow-2.2.0/tests/test_launcher_direct.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_launcher_multiple.py` & `dls-bxflow-2.2.0/tests/test_launcher_multiple.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_launcher_restart.py` & `dls-bxflow-2.2.0/tests/test_launcher_restart.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_logstore.py` & `dls-bxflow-2.2.0/tests/test_logstore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_news.py` & `dls-bxflow-2.2.0/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_protocolj.py` & `dls-bxflow-2.2.0/tests/test_protocolj.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_ptypy_mpi.py` & `dls-bxflow-2.2.0/tests/test_ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_ptyrex_mpi.py` & `dls-bxflow-2.2.0/tests/test_ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_scheduler_naive.py` & `dls-bxflow-2.2.0/tests/test_scheduler_naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_settings.py` & `dls-bxflow-2.2.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_shell.py` & `dls-bxflow-2.2.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_task.py` & `dls-bxflow-2.2.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_workflow.py` & `dls-bxflow-2.2.0/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/test_workflow_finder.py` & `dls-bxflow-2.2.0/tests/test_workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/a/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/a/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/b/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/b/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/base.py` & `dls-bxflow-2.2.0/tests/workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/c/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/c/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/e/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/e/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/f/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/f/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/g/workflow.py` & `dls-bxflow-2.2.0/tests/workflows/g/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.1.2/tests/workflows/utilities.py` & `dls-bxflow-2.2.0/tests/workflows/utilities.py`

 * *Files identical despite different names*

