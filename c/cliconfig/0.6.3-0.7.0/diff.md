# Comparing `tmp/cliconfig-0.6.3.tar.gz` & `tmp/cliconfig-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cliconfig-0.6.3.tar", last modified: Mon May 15 21:32:03 2023, max compression
+gzip compressed data, was "cliconfig-0.7.0.tar", last modified: Tue May 16 12:22:22 2023, max compression
```

## Comparing `cliconfig-0.6.3.tar` & `cliconfig-0.7.0.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.397621 cliconfig-0.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.373621 cliconfig-0.6.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.381621 cliconfig-0.6.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/flake.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/mypy.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/pydocstyle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/pylint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/ruff.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.markdownlint.json
--rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-15 21:31:41.000000 cliconfig-0.6.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-15 21:31:41.000000 cliconfig-0.6.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-15 21:31:41.000000 cliconfig-0.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-15 21:32:03.397621 cliconfig-0.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-05-15 21:31:41.000000 cliconfig-0.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6074 2023-05-15 21:31:41.000000 cliconfig-0.6.3/README_pypi.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.381621 cliconfig-0.6.3/cliconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7760 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     8190 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/process_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.385621 cliconfig-0.6.3/cliconfig/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/processing/_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/processing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    25816 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/processing/builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9902 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/processing/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/tag_routines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.385621 cliconfig-0.6.3/cliconfig/yaml_tags/
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-05-15 21:31:41.000000 cliconfig-0.6.3/cliconfig/yaml_tags/_yaml_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.381621 cliconfig-0.6.3/cliconfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-15 21:32:03.000000 cliconfig-0.6.3/cliconfig.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.385621 cliconfig-0.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.385621 cliconfig-0.6.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/_static/logo_extend.png
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/cliconfig.processing_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/cliconfig_api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/contribute.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/edge_cases.md
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    15754 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/processing.md
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-15 21:31:41.000000 cliconfig-0.6.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/github_actions_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 21:31:41.000000 cliconfig-0.6.3/github_actions_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 21:31:41.000000 cliconfig-0.6.3/github_actions_utils/color.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-15 21:31:41.000000 cliconfig-0.6.3/github_actions_utils/pydocstyle_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-15 21:31:41.000000 cliconfig-0.6.3/github_actions_utils/pylint_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-15 21:31:41.000000 cliconfig-0.6.3/github_actions_utils/pytest_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/licenses_tier/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-15 21:31:41.000000 cliconfig-0.6.3/licenses_tier/FLATTEN_DICT_LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-15 21:31:41.000000 cliconfig-0.6.3/pre-commit-checks.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-15 21:31:41.000000 cliconfig-0.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-15 21:31:41.000000 cliconfig-0.6.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 21:31:41.000000 cliconfig-0.6.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:32:03.397621 cliconfig-0.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-15 21:31:41.000000 cliconfig-0.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/tests/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/config2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/configtag1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/configtag2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/default2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/tests/configs/delete/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/delete/config1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/delete/config2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.377621 cliconfig-0.6.3/tests/configs/integration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.389621 cliconfig-0.6.3/tests/configs/integration/test1/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test1/main.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test1/sub1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test1/sub2.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.393621 cliconfig-0.6.3/tests/configs/integration/test2/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/data.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/default.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/exp1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/exp2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/exp3.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.393621 cliconfig-0.6.3/tests/configs/integration/test2/models/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/models/resnet100.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/models/resnet50.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/integration/test2/models/vit_b16.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.393621 cliconfig-0.6.3/tests/configs/merge/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/additional1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/additional2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/additional3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/default1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/default2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/merge/default3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/configs/multi_files_with_tags.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.393621 cliconfig-0.6.3/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/integration/test_inte_multiple_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.393621 cliconfig-0.6.3/tests/unit/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:32:03.397621 cliconfig-0.6.3/tests/unit/processing/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/processing/test_base_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11230 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/processing/test_builtin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/processing/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/processing/test_type_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_base_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_cli_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_config_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_dict_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_ex_docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_process_routines.py
--rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-15 21:31:41.000000 cliconfig-0.6.3/tests/unit/test_tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.856075 cliconfig-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.836075 cliconfig-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.844075 cliconfig-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/flake.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/pydocstyle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/pylint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/ruff.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.markdownlint.json
+-rw-r--r--   0 runner    (1001) docker     (123)    20457 2023-05-16 12:22:04.000000 cliconfig-0.7.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-16 12:22:04.000000 cliconfig-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 12:22:04.000000 cliconfig-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-16 12:22:22.856075 cliconfig-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-05-16 12:22:04.000000 cliconfig-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-16 12:22:04.000000 cliconfig-0.7.0/README_pypi.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.844075 cliconfig-0.7.0/cliconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15588 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8736 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/process_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.844075 cliconfig-0.7.0/cliconfig/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/processing/_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/processing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26940 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/processing/builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9885 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/processing/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/tag_routines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.844075 cliconfig-0.7.0/cliconfig/yaml_tags/
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-16 12:22:04.000000 cliconfig-0.7.0/cliconfig/yaml_tags/_yaml_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.844075 cliconfig-0.7.0/cliconfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6540 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 12:22:22.000000 cliconfig-0.7.0/cliconfig.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     5501 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/_static/logo_extend.png
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/cliconfig.processing_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/cliconfig_api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/contribute.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/edge_cases.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    16436 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/processing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-16 12:22:04.000000 cliconfig-0.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/github_actions_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 12:22:04.000000 cliconfig-0.7.0/github_actions_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 12:22:04.000000 cliconfig-0.7.0/github_actions_utils/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 12:22:04.000000 cliconfig-0.7.0/github_actions_utils/pydocstyle_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-16 12:22:04.000000 cliconfig-0.7.0/github_actions_utils/pylint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-16 12:22:04.000000 cliconfig-0.7.0/github_actions_utils/pytest_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/licenses_tier/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 12:22:04.000000 cliconfig-0.7.0/licenses_tier/FLATTEN_DICT_LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 12:22:04.000000 cliconfig-0.7.0/pre-commit-checks.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-16 12:22:04.000000 cliconfig-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-16 12:22:04.000000 cliconfig-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 12:22:04.000000 cliconfig-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:22:22.856075 cliconfig-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-16 12:22:04.000000 cliconfig-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.848075 cliconfig-0.7.0/tests/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/config2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/configtag1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/configtag2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/default2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/configs/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/delete/config1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/delete/config2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.840075 cliconfig-0.7.0/tests/configs/integration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/configs/integration/test1/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test1/main.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test1/sub1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test1/sub2.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/configs/integration/test2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/data.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/exp1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/exp2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/exp3.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/configs/integration/test2/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/models/resnet100.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/models/resnet50.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/integration/test2/models/vit_b16.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/configs/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/additional1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/additional2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/additional3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/default1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/default2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/merge/default3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/configs/multi_files_with_tags.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/integration/test_inte_multiple_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.852075 cliconfig-0.7.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:22:22.856075 cliconfig-0.7.0/tests/unit/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/processing/test_base_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/processing/test_builtin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/processing/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/processing/test_type_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_base_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_cli_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_config_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_dict_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_ex_docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_process_routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2137 2023-05-16 12:22:04.000000 cliconfig-0.7.0/tests/unit/test_tag_routines.py
```

### Comparing `cliconfig-0.6.3/.github/workflows/pipy_deployment.yaml` & `cliconfig-0.7.0/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/.github/workflows/pydocstyle.yaml` & `cliconfig-0.7.0/.github/workflows/pydocstyle.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/.github/workflows/pylint.yaml` & `cliconfig-0.7.0/.github/workflows/pylint.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/.github/workflows/tests.yaml` & `cliconfig-0.7.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/.pylintrc` & `cliconfig-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/CONTRIBUTING.md` & `cliconfig-0.7.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/LICENSE` & `cliconfig-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/PKG-INFO` & `cliconfig-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.6.3
+Version: 0.7.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -16,16 +16,16 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
-saving and config loading. It also contains many routines to manipulate the config as
-flatten or nested dicts.
+saving, config loading and at the end of config building. It also contains many
+routines to manipulate the config as flatten or nested dicts.
 
 ## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
 
 ## Source code: [github](https://github.com/valentingol/cliconfig)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
```

### Comparing `cliconfig-0.6.3/README.md` & `cliconfig-0.7.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 <p align="center">
   <img src="docs/_static/logo_extend.png" />
 </p>
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
-saving and config loading. It also contains many routines to manipulate the config as
-flatten or nested dicts.
+saving, config loading and at the end of config building. It also contains many
+routines to manipulate the config as flatten or nested dicts.
 
 ## Documentation :memo: [here](https://cliconfig.readthedocs.io/en/stable)
 
 ## Pypi :package: [here](https://pypi.org/project/cliconfig/)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
@@ -150,17 +150,15 @@
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config. The tagged key is not deleted if it is
   in the parent config.
-* `@delete`: This tag deletes the key from the config on pre-merge. It is useful
-  to activate a processing without having a good name for the key to add in
-  the default config.
+* `@delete`: This tag deletes the key from the config before merging.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
@@ -206,15 +204,15 @@
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config2.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
 
 These side effects are not visible in the config but stored on processing classes.
 They are objects that find the tags, remove them from config and apply a modification.
 These processing are powerful tools that can be used to highly customize the
-configuration process.
+configuration at each step of the process.
 
 You can easily create your own processing (associated to a tag or not).
 The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/stable/processing.html) section
 of the documentation.
 
 ## Edge cases
@@ -258,15 +256,15 @@
 Everyone can contribute to CLI Config, and we value everyone’s contributions.
 Please see our [contributing guidelines](CONTRIBUTING.md) for more information 🤗
 
 ## Todo
 
 Priority:
 
-* [ ] Add end-build processing that trigger at the end of `make_config` and `load_config`.
+* [x] Add end-build processing that trigger at the end of `make_config` and `load_config`.
 * [x] Continue `test_multi_tags2` integration test with cases that raise errors, and
   pre-save processing.
 * [x] Support multi-files in yaml file (with separator "---")
 * [ ] Fix mistakes in all docstrings (🚧  in progress)
 
 Secondary:
```

### Comparing `cliconfig-0.6.3/README_pypi.md` & `cliconfig-0.7.0/README_pypi.md`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
-saving and config loading. It also contains many routines to manipulate the config as
-flatten or nested dicts.
+saving, config loading and at the end of config building. It also contains many
+routines to manipulate the config as flatten or nested dicts.
 
 ## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
 
 ## Source code: [github](https://github.com/valentingol/cliconfig)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
```

### Comparing `cliconfig-0.6.3/cliconfig/__init__.py` & `cliconfig-0.7.0/cliconfig/__init__.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/cliconfig/base.py` & `cliconfig-0.7.0/cliconfig/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 """Base classes of Config object."""
-from typing import TYPE_CHECKING, Any, Dict, List
+from typing import TYPE_CHECKING, Any, Dict, List, Optional
 
 # Imports Processing for mypy type checking only
 if TYPE_CHECKING:
     from cliconfig.processing.base import Processing
 
 
 class Config:
     """Class for configuration.
 
     Config object contain the config dict and the processing list
     and no methods except ``__init__``, ``__repr__`` and ``__eq__``.
     The Config objects are mutable and not hashable.
+
+    Parameters
+    ----------
+    config_dict : Dict[str, Any]
+        The config dict.
+    process_list : Optional[List[Processing]], optional
+        The list of Processing objects. If None, an empty list is used.
+        The default is None.
     """
 
     def __init__(
-        self, config_dict: Dict[str, Any], process_list: List["Processing"]
+        self,
+        config_dict: Dict[str, Any],
+        process_list: Optional[List["Processing"]] = None
     ) -> None:
         self.dict = config_dict
-        self.process_list = process_list
+        self.process_list = process_list if process_list else []
 
     def __repr__(self) -> str:
         """Representation of Config object."""
         process_classes = [process.__class__.__name__ for process in self.process_list]
         return f"Config({self.dict}, {process_classes})"
 
     def __eq__(self, other: Any) -> bool:
```

### Comparing `cliconfig-0.6.3/cliconfig/cli_parser.py` & `cliconfig-0.7.0/cliconfig/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/cliconfig/config_routines.py` & `cliconfig-0.7.0/cliconfig/config_routines.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import sys
 from typing import List, Optional
 
 from cliconfig.base import Config
 from cliconfig.cli_parser import parse_cli
 from cliconfig.dict_routines import flatten, show_dict, unflatten
 from cliconfig.process_routines import (
+    end_build_processing,
     load_processing,
     merge_flat_paths_processing,
     merge_flat_processing,
     save_processing,
 )
 from cliconfig.processing.base import Processing
 from cliconfig.processing.builtin import DefaultProcessings
@@ -113,14 +114,16 @@
         config, cli_params_config, allow_new_keys=False, preprocess_first=False
     )
     print(
         f"[CONFIG] Info: Merged {len(default_config_paths)} default config(s), "
         f"{len(additional_config_paths)} additional config(s) and "
         f"{len(cli_params_dict)} CLI parameter(s)."
     )
+    # Apply end-build processing
+    config = end_build_processing(config)
     # Unflatten the config dict
     config.dict = unflatten(config.dict)
     return config
 
 
 def load_config(
     path: str,
@@ -187,14 +190,16 @@
     # if default configs are provided
     config = merge_flat_processing(
         config,
         loaded_config,
         allow_new_keys=default_config_paths is None,
         preprocess_first=False,
     )
+    # Apply end-build processing
+    config = end_build_processing(config)
     # Unflatten the config
     config.dict = unflatten(config.dict)
     return config
 
 
 def save_config(config: Config, path: str) -> None:
     """Save a config and apply pre-save processing before saving.
```

### Comparing `cliconfig-0.6.3/cliconfig/dict_routines.py` & `cliconfig-0.7.0/cliconfig/dict_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/cliconfig/process_routines.py` & `cliconfig-0.7.0/cliconfig/process_routines.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,7 +220,26 @@
     flat_config = Config(out_dict, process_list)
     # Get the post-load order
     order_list = sorted(process_list, key=lambda x: x.postload_order)
     # Apply the post-load processing
     for processing in order_list:
         flat_config = processing.postload(flat_config)
     return flat_config
+
+
+def end_build_processing(flat_config: Config) -> Config:
+    """Apply end-build processings to a flat config.
+
+    Parameters
+    ----------
+    flat_config : Config
+        The flat config to apply the end-build processings.
+
+    Returns
+    -------
+    flat_config : Config
+        The flat config after applying the end-build processings.
+    """
+    order_list = sorted(flat_config.process_list, key=lambda x: x.endbuild_order)
+    for processing in order_list:
+        flat_config = processing.endbuild(flat_config)
+    return flat_config
```

### Comparing `cliconfig-0.6.3/cliconfig/processing/_type_parser.py` & `cliconfig-0.7.0/cliconfig/processing/_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/cliconfig/processing/base.py` & `cliconfig-0.7.0/cliconfig/processing/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     That are applied in the order defined
     by the order attribute in case of multiple processing.
     """
 
     def __init__(self) -> None:
         self.premerge_order = 0.0
         self.postmerge_order = 0.0
+        self.endbuild_order = 0.0
         self.presave_order = 0.0
         self.postload_order = 0.0
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing.
 
         Function applied to the flat config to modify it
@@ -36,14 +37,23 @@
         """Post-merge processing.
 
         Function applied to the flat config to modify it
         after merging . It takes a flat config and returns a flat config.
         """
         return flat_config
 
+    def endbuild(self, flat_config: Config) -> Config:
+        """End-build processing.
+
+        Function applied to the flat config to modify it at the end of
+        a building process (typically :func:`.make_config` or :func:`.load_config`).
+        It takes a flat config and returns a flat config.
+        """
+        return flat_config
+
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing.
 
         Function applied to the flat config to modify it before
         saving. It takes a flat config and returns a flat config.
         """
         return flat_config
```

### Comparing `cliconfig-0.6.3/cliconfig/processing/builtin.py` & `cliconfig-0.7.0/cliconfig/processing/builtin.py`

 * *Files 2% similar despite different names*

```diff
@@ -164,20 +164,23 @@
 
 
 class ProcessCopy(Processing):
     """Copy a value with ``@copy`` tag. The copy is protected from direct updates.
 
     Tag your key with ``@copy`` and with value the name of the flat key to copy.
     The pre-merge processing removes the tag. The post-merge processing
-    sets the value (if the copied key exists) and occurs after most processings.
-    The pre-save processing restore the tag and the key to copy to keep the
-    information on future loads.
+    sets the value (if the copied key exists). The end-build processing checks
+    that the copied key exists or was already copied once. The pre-save processing
+    restore the tag and the key to copy to keep the information on future loads.
+    The post-merge and the end-build processings occurs after most processings to
+    allow the user to modify or add the copied key before the copy.
     Pre-merge order: 0.0
     Post-merge order: 10.0
-    Pre-save order: 10.0
+    End-build order: 10.0
+    Pre-save order: 0.0
 
     Examples
     --------
     .. code-block:: yaml
 
         # config.yaml
         a:
@@ -189,31 +192,30 @@
     .. code-block:: python
 
         {'a': {'b': 1, 'c': 1}}
 
     Note
     ----
 
-        The copy key is protected against any modification and will raise an error
-        if you try to modify it but will be updated if the copied key is updated.
-
-    Warning
-    -------
-
-        If the key to copy does not exist in the config on post-merge, the
-        processing will NOT raise an error to let the user the possibility
-        to add the key later via merge. However, the value still be protected.
+        * The copy key is protected against any modification and will raise an error
+          if you try to modify it but will be updated if the copied key is updated.
+        * If the key to copy does not exist in the config on post-merge, no error
+          is raised to let the user the possibility to add the key later via merge.
+          However, if the key still does not exist at the end of the build
+          (and the key was never copied), an error is raised.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
         self.postmerge_order = 10.0
-        self.presave_order = 10.0
+        self.endbuild_order = 10.0
+        self.presave_order = 0.0
         self.keys_to_copy: Dict[str, str] = {}
+        self.copied_keys: Set[str] = set()
         self.current_value: Dict[str, Any] = {}
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, val in items:
             if is_tag_in(flat_key, "copy"):
@@ -247,25 +249,42 @@
             # NOTE: Do not raise an error if the key to copy does not exist
             # yet because it can be added later in a future merge
             if key in flat_config.dict and val in flat_config.dict:
                 if flat_config.dict[key] != self.current_value[key]:
                     # The key has been modified
                     raise ValueError(
                         "Found attempt to modify a key with '@copy' tag. The key "
-                        "is then protected against updates (except the copied "
-                        f"value or the original key to copy). Found key: {key} of "
+                        f"is protected against direct updates. Found key: {key} of "
                         f"value {flat_config.dict[key]} that copy {val} of value "
                         f"{flat_config.dict[val]}"
                     )
                 # Copy the value
                 flat_config.dict[key] = flat_config.dict[val]
+                self.copied_keys.add(key)
                 # Update the current value
                 self.current_value[key] = flat_config.dict[val]
         return flat_config
 
+    def endbuild(self, flat_config: Config) -> Config:
+        """End-build processing."""
+        for key, val in self.keys_to_copy.items():
+            if key in flat_config.dict and key not in self.copied_keys:
+                if val in flat_config.dict:
+                    # Copy the value
+                    flat_config.dict[key] = flat_config.dict[val]
+                    self.copied_keys.add(key)
+                else:
+                    raise ValueError(
+                        "A key with '@copy' tag has been found but the key to copy "
+                        "does not exist at the end of the build and it has been "
+                        f"never copied. Found key: {key} that would copy the "
+                        f"key: {val}."
+                    )
+        return flat_config
+
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         # Restore the tag with the key to copy to keep the information
         # on further loading
         keys = list(flat_config.dict.keys())
         for key in keys:
             clean_key = clean_all_tags(key)
@@ -283,26 +302,26 @@
     nested dicts, unions (with Union or the '|' symbol) and Optional.
     The type description is lowercased and spaces are removed.
 
     For instance: ``@type:None|List[Dict[str, int|float]]`` is valid and force
     the type to be None or a list containing dicts with str keys and int or float
     values.
 
-    the processing stores the type in pre-merge and check alls forced types on
-    post-merge. It restore the tag in pre-save to keep the information on
-    future loads. The post-merge processing occurs after almost all processings.
+    The processing stores the type in pre-merge and check alls forced types on
+    end-build. It restore the tag in pre-save to keep the information on
+    future loads. The end-build processing occurs after almost all processings.
     Pre-merge order: 0.0
-    Post-merge order: 20.0
+    End-build order: 20.0
     Pre-save order: 0.0
 
     Note
     ----
-        The type is not checked on pre-merge to allow the parameter to be
-        updated (by a copy or a merge for instance). The goal of this
-        processing is to ensure the type at the end of the post-merge.
+        The type is not checked on pre-merge or ost-merge to allow the parameter
+        to be updated (by a copy or a merge for instance). The goal of this
+        processing is to ensure the type at the end of the build.
 
     Examples
     --------
     ::
 
         in_dict = {"param@type:None|List[int|float]": None}
         dict1 = {param: [0, 1, 2.0]}  # no error
@@ -317,15 +336,15 @@
     doesn't raise an error in the first case because the type checking is
     evaluated after the merge with ``dict2``.
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.premerge_order = 0.0
-        self.postmerge_order = 20.0
+        self.endbuild_order = 20.0
         self.presave_order = 0.0
         self.forced_types: Dict[str, tuple] = {}
         self.type_desc: Dict[str, str] = {}  # For error messages
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
@@ -350,16 +369,16 @@
                 del flat_config.dict[flat_key]
                 flat_config.dict[clean_tag(flat_key, f"type:{type_desc}")] = val
                 # Store the forced type
                 self.forced_types[clean_key] = expected_type
                 self.type_desc[clean_key] = type_desc
         return flat_config
 
-    def postmerge(self, flat_config: Config) -> Config:
-        """Post-merge processing."""
+    def endbuild(self, flat_config: Config) -> Config:
+        """End-build processing."""
         for key, expected_type in self.forced_types.items():
             if key in flat_config.dict and not _isinstance(
                 flat_config.dict[key], expected_type
             ):
                 type_desc = self.type_desc[key]
                 raise ValueError(
                     f"Key previously tagged with '@type:{type_desc}' must be "
@@ -507,15 +526,15 @@
     """Delete the parameters tagged with ``@delete`` on pre-merge.
 
     This processing is usefull to activate a processing without adding
     an additional parameter in the default configuration to avoid the error
     on merge with ``allow_new_keys=False``. This processing is applied very
     late on pre-merge to allow the others processing to be applied before
     deleting the parameters.
-    Pre-merge order: 25.0
+    Pre-merge order: 30.0
 
     Examples
     --------
     .. code-block:: yaml
 
         # main.yaml
         1@select@delete: configs.config1
@@ -544,15 +563,15 @@
         this parameter will be remain as it is. This processing is more used
         to delete parameter that is NOT present in the default configuration.
     """
 
     def __init__(self) -> None:
         super().__init__()
         # After all pre-merge processing
-        self.premerge_order = 25.0
+        self.premerge_order = 30.0
 
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         keys = list(flat_config.dict.keys())
         for key in keys:
             if is_tag_in(key, "delete"):
                 del flat_config.dict[key]
```

### Comparing `cliconfig-0.6.3/cliconfig/processing/create.py` & `cliconfig-0.7.0/cliconfig/processing/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,28 +175,28 @@
     -------
     processing : Processing
         The processing object with the pre-merge method.
 
 
     Examples
     --------
-    With the following 2 processing and the following config:
-
-    ::
-
-        proc2 = create_processing_value(lambda x: -x, regex="neg_number.*", order=0.0)
-        proc1 = create_processing_value(lambda x: x + 1, tag_name="add1", order=1.0)
+    With the following config and 2 processings:
 
     .. code_block: yaml
 
-        --- # config.yaml
+        # config.yaml
         neg_number1: 1
         neg_number2: 1
         neg_number3@add1: 1
 
+    ::
+
+        proc2 = create_processing_value(lambda x: -x, regex="neg_number.*", order=0.0)
+        proc1 = create_processing_value(lambda x: x + 1, tag_name="add1", order=1.0)
+
     When config.yaml is merged with an other config, it will be considered
     before merging as:
 
     ::
 
         {'number1': -1, 'number2': -1, 'number3': 0}
     """
```

### Comparing `cliconfig-0.6.3/cliconfig/tag_routines.py` & `cliconfig-0.7.0/cliconfig/tag_routines.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/cliconfig/yaml_tags/_yaml_tags.py` & `cliconfig-0.7.0/cliconfig/yaml_tags/_yaml_tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,20 +9,14 @@
     """Node class for tagged tree (with yaml tags)."""
 
     def __init__(self, value: Any, tag: str, *, is_config: bool) -> None:
         self.tag = tag
         self.value = value
         self.is_config = is_config
 
-    def items(self) -> Any:
-        """Items method."""
-        if self.is_config:
-            return self.value.items()
-        return None
-
 
 def tagged_constructor(
     loader: yaml.SafeLoader, tag_suffix: str, node: yaml.Node
 ) -> Any:
     """Build a tagged tree node from yaml node."""
     if isinstance(node, yaml.ScalarNode):
         return TaggedNode(loader.construct_scalar(node), tag_suffix, is_config=False)
@@ -59,20 +53,16 @@
             value = yaml.safe_load(tagged_tree.value)
         else:
             value = tagged_tree.value
         return value, tag
     return tagged_tree, None
 
 
-def build_tree_from_dict(in_dict: Any) -> Dict[str, Any]:
-    """Build a dict with cliconfig tag from tagged tree.
-
-    The input can be either a tagged tree that implements the items method
-    or a dict.
-    """
+def build_tree_from_dict(in_dict: Dict) -> Dict[str, Any]:
+    """Build a dict with cliconfig tag from a dict of tagged trees."""
     out_dict: Dict[str, Any] = {}
     for key, value in in_dict.items():
         tree, tag = insert_tags(value)
         if tag:
             subtag = tag.replace("!", "")
             key = f"{key}@{subtag}"
         out_dict[key] = tree
```

### Comparing `cliconfig-0.6.3/cliconfig.egg-info/PKG-INFO` & `cliconfig-0.7.0/cliconfig.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cliconfig
-Version: 0.6.3
+Version: 0.7.0
 Summary: Merge your config files and set parameters from the command line in a simple way.
 Author-email: Valentin Goldite <valentin.goldite@gmail.com>
 Project-URL: Source, https://github.com/valentingol/cliconfig
 Keywords: logging,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -16,16 +16,16 @@
 <p align="center">
   <img src="https://raw.githubusercontent.com/valentingol/cliconfig/main/docs/_static/logo_extend.png" />
 </p>
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
-saving and config loading. It also contains many routines to manipulate the config as
-flatten or nested dicts.
+saving, config loading and at the end of config building. It also contains many
+routines to manipulate the config as flatten or nested dicts.
 
 ## Documentation: [read-the-docs](https://cliconfig.readthedocs.io/en/stable)
 
 ## Source code: [github](https://github.com/valentingol/cliconfig)
 
 [![Release](https://img.shields.io/github/v/tag/valentingol/cliconfig?label=Pypi&logo=pypi&logoColor=yellow)](https://pypi.org/project/cliconfig/)
 ![PythonVersion](https://img.shields.io/badge/Python-3.7%20%7E%203.11-informational)
```

### Comparing `cliconfig-0.6.3/cliconfig.egg-info/SOURCES.txt` & `cliconfig-0.7.0/cliconfig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/Makefile` & `cliconfig-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/_static/logo.png` & `cliconfig-0.7.0/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/_static/logo_extend.png` & `cliconfig-0.7.0/docs/_static/logo_extend.png`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/cliconfig_api.rst` & `cliconfig-0.7.0/docs/cliconfig_api.rst`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/conf.py` & `cliconfig-0.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/edge_cases.md` & `cliconfig-0.7.0/docs/edge_cases.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/index.rst` & `cliconfig-0.7.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
   :alt: CLI config logo
 
 |
 
 *CLI Config*: Lightweight library that provides routines to merge nested configs
 and set parameters from command line. It is also provide processing functions
 that can change the whole configuration before and after each config merge, config
-saving and config loading. It also contains many routines to manipulate the config as
-flatten or nested dicts.
+saving, config loading and at the end of config building. It also contains many
+routines to manipulate the config as flatten or nested dicts.
 
 `Pypi project <https://pypi.org/project/cliconfig/>`_
 
 `Github project <https://github.com/valentingol/cliconfig>`_
 
 
 |PyPI version| |PythonVersion| |License|
```

### Comparing `cliconfig-0.6.3/docs/license.md` & `cliconfig-0.7.0/docs/license.md`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/make.bat` & `cliconfig-0.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/docs/processing.md` & `cliconfig-0.7.0/docs/processing.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Processing
 
 Processings are powerful tools to modify the config at each step of the lifecycle of
 a configuration. More precisely, you can use processings to modify the full
 configuration before and after each merge, after loading, and before saving the config.
 
-The processings are applied via a processing object that have four methods
-(called "processing" to simplify): `premerge`, `postmerge`, `postload` and `presave`.
-These names correspond to the timing they are applied. Each processing have
-the signature:
+The processings are applied via a processing object that have five methods
+(called "processing" to simplify): `premerge`, `postmerge`, `endbuild`, `postload`
+and `presave`. These names correspond to the timing they are applied. Each processing
+have the signature:
 
 ```python
 def premerge(self, flat_config: Config) -> Config:
     ...
 ```
 
-Where `Config` is a simple dataclass containing only two fields: `dict` that is the
-configuration dict and `process_list`, the list of processing objects
+Where `Config` is a simple class containing only two attributes (and no methods):
+`dict` that is the configuration dict and `process_list`, the list of processing objects
 (we discuss about this in a section below). Note that it is
 also the class of the object returned by the `make_config` function.
 
 They only take a flat config as input i.e a config containing a dict of depth 1 with
 dot-separated keys and return the modified flat dict (and keep it flat!).
 
 In this section, you will learn how they work and how to create your own to make
@@ -45,45 +45,61 @@
 However, it's important to note that after building your config with `make_config`,
 the dict will be unflattened to its normal nested configuration structure.
 
 ## Processing order
 
 The order in which the processings are triggered is crucial because they modify
 the config and consequently affect the behavior of subsequent processings.
-To manage this order, the processing class have four float attributes representing
-the order of the four processing methods: premerge, postmerge, postload, and presave.
+To manage this order, the processing class have five float attributes representing
+the order of the five processing methods: premerge, postmerge, endbuild, postload,
+and presave.
 
 Here's a basic example to illustrate the significance of the order:
 
 ```yaml
-# config.yaml
-param1@type:int@copy: 'param2'
-param2@type:int: 1
+# config1.yaml
+merge@merge_add@delete: config2.yaml
+param: 1
+# config2.yaml
+param2: 2
 ```
 
-In this example, we want to enforce the types of the parameters. Additionally, `param1`
-is intended to be a copy of `param2` and naturally, it is forced to have the same type.
+In this example, we want to build a global config using `config1.yaml`. This file contains only
+half of the paramers, and the other half is in `config2.yaml`. Then, we add a key
+with the name of our choice, here "merge", tagged with `@merge_add` to merge
+`config2.yaml` before the global config update. We add the `@delete` tag to delete
+the key "merge" before merging with the global config because in this case, there is
+no key with the name "merge" in the global config and it would raise an error as
+it is not possible to ass new keys.
+
+`@merge_add` and `@delete` has both only a pre-merge effect. Let's check the orders.
+It is `-20.0` for merge and `30.0` for delete. So merge trigger first, add `param2` and
+the "merge" key is deleted after it. If the orders were reversed, the key would have been
+deleted before merge processing and so the `param2` would not have been updated with the
+value of 2 and the resulting configuration would potentially not have been
+the expected one at all.
 
-During the pre-merge processing, the tags are removed, and information about the
-enforced types and the copy operation is gathered on processing attributes.
-Then, a merge is performed (assuming no modifications to our parameters at
-this point to simplify), followed by the post-merge processing.
-
-Now, what happens if the type post-merge processing triggers before the
-copy post-merge processing? It will check the value, which is `"param2"`,
-and raise an error because it is not an integer (the forced type got during pre-merge).
-However, if the copy processing triggers before the type processing, it will copy the
-value of `param2` (which is `1`) to `param1`, and then the type processing will not
-encounter a wrong value.
-
-Fortunately, the post-merge orders are set as follows: `20.0` for the type processing
-and `10.0` for the copy processing. As a result, the copy processing triggers first.
 Therefore, it is crucial to carefully manage the order when creating your own
 processings!
 
+Some useful ranges to choose your order:
+
+* not important: order = 0 (default)
+* if it check/modify the config before applying any processing: order < -25
+* if it add new parameters: -25 < order < -5
+* if it update a value based on itself: -5 < order < 5
+* if it update a value based on other keys: 5 < order < 15
+* if it checks a property on a value: 15 < order < 25
+* if it delete other key(s) but you want to trigger the tags before: 25 < order < 35
+* final check/modification after all processings: order > 35
+
+Note: a pre-merge order should not be greater than 1000, the order of the default
+processing `ProcessCheckTags` that raise an error if tags still exist at the end
+of the pre-merge step.
+
 ## Create basic processing
 
 ### Pre-merge processing that modify a single value
 
 The pre-merge processing is particularly useful as it allows you to modify the input
 config provided by the user and create the resulting Python dictionary that stores the
 configuration for your experiment. It serves as the interface between the user config
```

### Comparing `cliconfig-0.6.3/docs/quickstart.md` & `cliconfig-0.7.0/docs/quickstart.md`

 * *Files 4% similar despite different names*

```diff
@@ -105,17 +105,15 @@
 * `@type:<my type>`: This tag checks if the key matches the specified type `<my type>`
   after each update, even if the tag is no longer present. It supports basic types
   (except for tuples and sets, which are not handled by YAML) as well as unions
   (using "Union" or "|"), optional values, nested list, and nested dict.
   For instance: `@type:List[Dict[str, int|float]]`.
 * `@select`: This tag select sub-config(s) to keep and delete the other
   sub-configs in the same parent config
-* `@delete`: This tag deletes the key from the config on pre-merge. It is useful
-  to activate a processing without having a good name for the key to add in
-  the default config.
+* `@delete`: This tag deletes the key from the config before merging.
 
 The tags are applied in the following order: `@merge`, `@select`, `@copy`, `@type`
 and then `@delete`.
 
 Please note that the tags serve as triggers for internal processing and will be
 automatically removed from the key after processing.
 
@@ -161,13 +159,13 @@
 Then, all the parameters in `config1` and `config2` have enforced types
 (`config1.param` can also be None) and changing `config2.param` will also update
 `config1.param` accordingly (which is protected by direct update).
 
 These side effects are not visible in the config but stored on processing classes.
 They are objects that find the tags, remove them from config and apply a modification.
 These processing are powerful tools that can be used to highly customize the
-configuration process.
+configuration at each step of the process.
 
 You can easily create your own processing (associated to a tag or not).
 The way to do it and a further explanation of them is available in the
 [*Processing*](https://cliconfig.readthedocs.io/en/latest/processing.html) section
 of the documentation.
```

### Comparing `cliconfig-0.6.3/github_actions_utils/pydocstyle_manager.py` & `cliconfig-0.7.0/github_actions_utils/pydocstyle_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/github_actions_utils/pylint_manager.py` & `cliconfig-0.7.0/github_actions_utils/pylint_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/github_actions_utils/pytest_manager.py` & `cliconfig-0.7.0/github_actions_utils/pytest_manager.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/licenses_tier/FLATTEN_DICT_LICENSE` & `cliconfig-0.7.0/licenses_tier/FLATTEN_DICT_LICENSE`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/pre-commit-checks.sh` & `cliconfig-0.7.0/pre-commit-checks.sh`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/pyproject.toml` & `cliconfig-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/configs/integration/test2/default.yaml` & `cliconfig-0.7.0/tests/configs/integration/test2/default.yaml`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/conftest.py` & `cliconfig-0.7.0/tests/conftest.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,24 +7,28 @@
 from cliconfig.processing.base import Processing
 from cliconfig.tag_routines import clean_all_tags, clean_tag, is_tag_in
 
 
 class ProcessAdd1(Processing):
     """Add 1 to values with tag "@add1"."""
 
-    # pylint: disable=unused-argument
     def premerge(self, flat_config: Config) -> Config:
         """Pre-merge processing."""
         items = list(flat_config.dict.items())
         for flat_key, value in items:
             if is_tag_in(flat_key, "add1"):
                 flat_config.dict[clean_tag(flat_key, "add1")] = value + 1
                 del flat_config.dict[flat_key]
         return flat_config
 
+    def endbuild(self, flat_config: Config) -> Config:
+        """End-build processing."""
+        flat_config.dict["processing name"] = "ProcessAdd1"
+        return flat_config
+
     def presave(self, flat_config: Config) -> Config:
         """Pre-save processing."""
         return self.premerge(flat_config)
 
 
 class ProcessKeep(Processing):
     """Prevent a value from being changed after the merge."""
```

### Comparing `cliconfig-0.6.3/tests/integration/test_inte_multiple_tags.py` & `cliconfig-0.7.0/tests/integration/test_inte_multiple_tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,22 +36,23 @@
         },
         "config3": {
             "select": "config3.param1",
             "param1": 0,
         },
     }
     check.equal(config.dict, expected_config)
+    config = merge_flat_processing(
+        config,
+        Config({"config2.param": 5.6}, []),
+        preprocess_first=False,
+    )
     with pytest.raises(
         ValueError, match="Key previously tagged with '@type:None|int'.*"
     ):
-        merge_flat_processing(
-            config,
-            Config({"config2.param": 5.6}, []),
-            preprocess_first=False,
-        )
+        config.process_list[3].endbuild(config)
     sys.argv = sys_argv
 
 
 def test_multiple_tags2() -> None:
     """2nd integration test for multiple tags."""
     sys_argv = sys.argv.copy()
     sys.argv = [
@@ -138,25 +139,27 @@
         saved_dict["data"]["augmentation@type:List[str]"],
         ["RandomHorizontalFlip", "RandomVerticalFlip"],
     )
     check.equal(
         saved_dict["models"]["archi_name@type:None|str@select"], "models.vit_b16"
     )
     check.equal(
-        saved_dict["models"]["vit_b16"]["in_size@type:int@copy"], "data.data_size"
+        saved_dict["models"]["vit_b16"]["in_size@copy@type:int"], "data.data_size"
     )
     config = load_config(
         "tests/tmp/config.yaml",
         ["tests/configs/integration/test2/default.yaml"],
         config.process_list,
     )
     del config.dict["run_id"]
     check.equal(config.dict, expected_dict)
     with pytest.raises(ValueError, match="Key previously tagged with '@type:int.*"):
-        merge_flat_processing(config, Config({"models.vit_b16.n_blocks": 5.6}, []))
+        config.process_list[7].endbuild(
+            Config({"models.vit_b16.n_blocks": 5.6}, config.process_list)
+        )
     with pytest.raises(
         ValueError, match="Found attempt to modify a key with '@copy' tag.*"
     ):
         merge_flat_processing(config, Config({"models.vit_b16.in_size": 224}, []))
 
     shutil.rmtree("tests/tmp")
     sys.argv = sys_argv
```

### Comparing `cliconfig-0.6.3/tests/unit/processing/test_base_processing.py` & `cliconfig-0.7.0/tests/unit/processing/test_base_processing.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 
     config = Config({"a.b": 1, "b": 2, "c.d.e": 3, "c.d.f": [2, 3]}, [])
     base_process = Processing()
     check.equal(
         (
             base_process.premerge(config),
             base_process.postmerge(config),
+            base_process.endbuild(config),
             base_process.presave(config),
             base_process.postload(config),
         ),
-        (config, config, config, config),
+        (config, config, config, config, config),
     )
     # Check equality of Processing objects
     proc1 = _ProcessingTest()
     proc1.attr = 0
     proc2 = _ProcessingTest()
     proc2.attr = 0
     check.equal(proc1, proc2)
```

### Comparing `cliconfig-0.6.3/tests/unit/processing/test_builtin.py` & `cliconfig-0.7.0/tests/unit/processing/test_builtin.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     flat_config = processing.premerge(flat_config)
     check.equal(
         flat_config.dict, {"config1.param1": 1, "config2.param2": "config1.param1"}
     )
     flat_config.dict["config1.param1"] = 2
     flat_config = processing.postmerge(flat_config)
     check.equal(flat_config.dict, {"config1.param1": 2, "config2.param2": 2})
+    check.equal(processing.copied_keys, {"config2.param2"})
     flat_config = processing.presave(flat_config)
     check.equal(processing.current_value, {"config2.param2": 2})
     check.equal(
         flat_config.dict, {"config1.param1": 2, "config2.param2@copy": "config1.param1"}
     )
     check.equal(processing.keys_to_copy, {"config2.param2": "config1.param1"})
     check.equal(flat_config.process_list, [processing])
@@ -142,22 +143,34 @@
             "with value: c, previous value to copy: b"
         ),
     ):
         processing.premerge(Config({"a@copy@tag": "c"}, [processing]))
     # Case of non-existing key (on post-merge): do not raise error
     processing.keys_to_copy = {"a": "b"}
     processing.postmerge(Config({"a": "b"}, [processing]))
+    # Case of non-existing key (on end-build): raise error
+    with pytest.raises(
+        ValueError,
+        match=re.escape(
+            "A key with '@copy' tag has been found but the key to copy does not "
+            "exist at the end of the build and it has been never copied. Found key: "
+            "a that would copy the key: b."
+        ),
+    ):
+        processing.endbuild(Config({"a": "b"}, [processing]))
+    # Copy if it appears on end-build
+    config = processing.endbuild(Config({"a": "b", "b": 3}, [processing]))
+    check.equal(config.dict["a"], 3)
     # Case overwriting a key
     processing.current_value = {"a": 2}
     with pytest.raises(
         ValueError,
-        match=re.escape(
+        match=(
             "Found attempt to modify a key with '@copy' tag. The key is "
-            "then protected against updates (except the copied value or "
-            "the original key to copy). Found key: a of value c that copy "
+            "protected against direct updates. Found key: a of value c that copy "
             "b of value 1"
         ),
     ):
         processing.postmerge(Config({"a": "c", "b": 1}, [processing]))
 
 
 def test_process_typing() -> None:
@@ -183,14 +196,15 @@
             "param2": (("list", ((type(None), ("dict", (str,), (int, float))),)),),
         },
     )
     check.equal(
         flat_config.process_list[0].type_desc,  # type: ignore
         {"param1": "int", "param2": "List[Optional[Dict[str, int|float]]]"},
     )
+    flat_config = processing.endbuild(flat_config)  # no error
     flat_config = processing.presave(flat_config)
     check.equal(
         flat_config.dict,
         {"param1@type:int": 3, "param2.a": None, "param2.b": [{"c": 1}]},
     )
     processing.forced_types = {}  # Reset forced types
     processing.type_desc = {}  # Reset type description
@@ -206,26 +220,28 @@
         match=(
             "Find the tag '@type:str' on a key that has already been associated "
             "to an other type: int. Find problem at key: param@type:str"
         ),
     ):
         processing.premerge(Config({"param@type:str": "str"}, [processing]))
 
-    # Case of wrong type in postmerge
+    # Case of wrong type in post-merge: no error
     processing.forced_types = {"param": (int,)}
     processing.type_desc = {"param": "int"}
+    processing.postmerge(Config({"param": "mystr"}, [processing]))
+    # Case of wrong type in end-build: raise error
     with pytest.raises(
         ValueError,
         match=(
             "Key previously tagged with '@type:int' must be "
             "associated to a value of type int. Find the "
             "value: mystr of type <class 'str'> at key: param"
         ),
     ):
-        processing.postmerge(Config({"param": "mystr"}, [processing]))
+        processing.endbuild(Config({"param": "mystr"}, [processing]))
 
 
 def test_process_select() -> None:
     """Test ProcessSelect."""
     processing = ProcessSelect()
     flat_dict = {
         "models.model_names@select": ["models.model1", "models.model3"],
@@ -322,10 +338,10 @@
     config = Config({}, DefaultProcessings().list)
     for proc in [
         ProcessCheckTags(),
         ProcessMerge(),
         ProcessCopy(),
         ProcessTyping(),
         ProcessDelete(),
-        ProcessSelect()
+        ProcessSelect(),
     ]:
         check.is_in(proc, config.process_list)
```

### Comparing `cliconfig-0.6.3/tests/unit/processing/test_create.py` & `cliconfig-0.7.0/tests/unit/processing/test_create.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/unit/processing/test_type_parser.py` & `cliconfig-0.7.0/tests/unit/processing/test_type_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/unit/test_base_config.py` & `cliconfig-0.7.0/tests/unit/test_base_config.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/unit/test_cli_parser.py` & `cliconfig-0.7.0/tests/unit/test_cli_parser.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/unit/test_config_routines.py` & `cliconfig-0.7.0/tests/unit/test_config_routines.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,15 @@
         "param3": 3,
         "letters": {
             "letter1": "f",
             "letter2": "e",
             "letter3": "c",
             "letter4": "d",
         },
+        "processing name": "ProcessAdd1",
     }
     expected_out = (
         "[CONFIG] Warning: New keys found in CLI parameters that will not be merged:\n"
         "  - unknown\n"
         "  - unknown2\n"
         "[CONFIG] Info: Merged 2 default config(s), "
         "2 additional config(s) and 1 CLI parameter(s).\n"
@@ -92,14 +93,15 @@
         "param3": 3,
         "letters": {
             "letter1": "a",
             "letter2": "e",
             "letter3": "c",
             "letter4": "d",
         },
+        "processing name": "ProcessAdd1",
     }
     check.equal(config.dict, expected_config)
     # Additional keys when allow_new_keys=False
     with pytest.raises(ValueError, match="New parameter found 'param3'.*"):
         load_config(
             "tests/configs/default2.yaml",
             default_config_paths=[
```

### Comparing `cliconfig-0.6.3/tests/unit/test_dict_routines.py` & `cliconfig-0.7.0/tests/unit/test_dict_routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,25 +161,23 @@
     dict2 = load_dict("tests/tmp/config.yaml")
     check.equal(dict1, dict2)
     # Case multiple files and yaml tags
     out_dict = load_dict("tests/configs/multi_files_with_tags.yaml")
     expected_dict = {
         "config@cfg": {
             "param1@par@other": 1,
-            "param2": {"a": 1.0, "b@par2": 2.1},
+            "param2": {"a": 1.0, "b@par2": "2.1"},
         },
         "config2": {
             "param3@par3": 3.2,
-            "param4@par4": [4, 5, {'6': 6}],
-            "param5": [True, 8]
+            "param4@par4": [4, 5, {"6": 6}],
+            "param5": [True, 8],
         },
-        "config3@cfg3": {
-            "param6": {"param7@par7": None}, "param8": "True"
-        },
-        "config4@cfg4": {"config5@cfg5": {"param9": "11"}}
+        "config3@cfg3": {"param6": {"param7@par7": None}, "param8": "True"},
+        "config4@cfg4": {"config5@cfg5": {"param9": "11"}},
     }
     check.equal(out_dict, expected_dict)
     shutil.rmtree("tests/tmp")
 
 
 def test_show_dict() -> None:
     """Test show_dict."""
```

### Comparing `cliconfig-0.6.3/tests/unit/test_ex_docs.py` & `cliconfig-0.7.0/tests/unit/test_ex_docs.py`

 * *Files identical despite different names*

### Comparing `cliconfig-0.6.3/tests/unit/test_process_routines.py` & `cliconfig-0.7.0/tests/unit/test_process_routines.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import pytest
 import pytest_check as check
 import yaml
 
 from cliconfig.base import Config
 from cliconfig.process_routines import (
+    end_build_processing,
     load_processing,
     merge_flat_paths_processing,
     merge_flat_processing,
     save_processing,
 )
 from cliconfig.processing.base import Processing
 from tests.conftest import ProcessAdd1, ProcessKeep
@@ -123,7 +124,14 @@
         ValueError,
         match=("config_or_path must be a Config instance or a path to a yaml file."),
     ):
         merge_flat_paths_processing(
             Config({"a": 1}, []),
             ("not a path",),  # type: ignore
         )
+
+
+def test_end_build_processing(process_add1: ProcessAdd1) -> None:
+    """Test end_build_processing."""
+    config = Config({"param1@add1": 0}, [process_add1])
+    config = end_build_processing(config)
+    check.equal(config.dict, {"param1@add1": 0, "processing name": "ProcessAdd1"})
```

### Comparing `cliconfig-0.6.3/tests/unit/test_tag_routines.py` & `cliconfig-0.7.0/tests/unit/test_tag_routines.py`

 * *Files identical despite different names*

