# Comparing `tmp/ansible-navigator-3.2.0.tar.gz` & `tmp/ansible-navigator-3.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-navigator-3.2.0.tar", last modified: Fri Apr 28 20:08:58 2023, max compression
+gzip compressed data, was "ansible-navigator-3.3.0.tar", last modified: Tue May 16 14:53:23 2023, max compression
```

## Comparing `ansible-navigator-3.2.0.tar` & `ansible-navigator-3.3.0.tar`

### file list

```diff
@@ -1,251 +1,251 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.362619 ansible-navigator-3.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.326619 ansible-navigator-3.2.0/.config/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/dictionary.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.config/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.darglint
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.326619 ansible-navigator-3.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/documentation_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/security_bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/chronographer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.markdownlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.prettierrc.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/bindep.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/cspell.config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/.generated/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/.generated/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/_ext/regenerate_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.330618 ansible-navigator-3.2.0/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/code-of-conduct.md
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/guidelines.md
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/contributing/security.md
--rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/settings.md
--rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/docs/subcommands.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.dark_vs.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.json.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.shell.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.source.yaml.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.basic.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.derivative.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.html.markdown.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/licenses/LICENSE.text.log.json.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)    13708 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 20:08:58.362619 ansible-navigator-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.322618 ansible-navigator-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/src/ansible_navigator/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 20:08:57.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/_version_doc_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/action_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/_actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/back.py
--rw-r--r--   0 runner    (1001) docker     (123)     3768 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    27490 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)    14294 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10752 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5729 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/help_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/images.py
--rw-r--r--   0 runner    (1001) docker     (123)    21232 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)    17737 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     7126 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/open_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/quit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/replay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/rerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    36394 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_form.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_notification.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/select.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/actions/write_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/app_public.py
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/command_runner/command_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.342619 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19832 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
--rw-r--r--   0 runner    (1001) docker     (123)    31546 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    49134 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7281 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7466 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6985 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/content_defs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.346619 ansible-navigator-3.2.0/src/ansible_navigator/data/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24616 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/ansible-navigator.json
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/catalog_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.346619 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.json.json
--rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.shell.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.yaml.json
--rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.basic.json
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.derivative.json
--rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.markdown.json
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.log.json
--rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/help.md
--rw-r--r--   0 runner    (1001) docker     (123)    13323 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/image_introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/images_dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/settings-sample.template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/settings-schema.partial.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/
--rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/dark_vs.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/themes/terminal_colors.json
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/data/welcome.md
--rw-r--r--   0 runner    (1001) docker     (123)    13688 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/diagnostics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/image_manager/puller.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/initialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.350619 ansible-navigator-3.2.0/src/ansible_navigator/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/runner/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/steps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.354619 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/fchainmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/grammars.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/reg.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    13042 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/tokenize.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15005 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/colorize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_curses_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_information.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_radio.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_working.py
--rw-r--r--   0 runner    (1001) docker     (123)    16158 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_working.py
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9282 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/menu_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/sentinels.py
--rw-r--r--   0 runner    (1001) docker     (123)    33890 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9911 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/ansi.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/dict_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/dot_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/packaged_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/print.py
--rw-r--r--   0 runner    (1001) docker     (123)    11852 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.358619 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/src/ansible_navigator/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 20:08:58.334619 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-28 20:08:58.000000 ansible-navigator-3.2.0/src/ansible_navigator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-04-28 20:08:33.000000 ansible-navigator-3.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.637551 ansible-navigator-3.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.605551 ansible-navigator-3.3.0/.config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/dictionary.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.config/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.darglint
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/documentation_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/security_bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/chronographer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.markdownlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.prettierrc.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/bindep.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/cspell.config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/.generated/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/.generated/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     6542 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/_ext/regenerate_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.609551 ansible-navigator-3.3.0/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/code-of-conduct.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/guidelines.md
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/contributing/security.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/settings.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1571 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/docs/subcommands.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.asottile_tm_tokenize.all.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.dark_vs.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.json.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.shell.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.source.yaml.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.basic.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.derivative.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.html.markdown.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/licenses/LICENSE.text.log.json.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    17811 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:53:23.637551 ansible-navigator-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.601551 ansible-navigator-3.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/src/ansible_navigator/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/_version_doc_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/action_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/back.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3849 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27507 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14363 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10841 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5810 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/help_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21528 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21313 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7261 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/open_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/quit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/replay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/rerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36365 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_form.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_notification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7410 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/actions/write_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/app_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/command_runner/command_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19986 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15202 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6813 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31712 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48249 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7509 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/content_defs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.621551 ansible-navigator-3.3.0/src/ansible_navigator/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24878 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/ansible-navigator.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23583 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/catalog_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/log.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.json.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48664 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.yaml.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60462 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.basic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.derivative.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50792 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.markdown.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.log.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/help.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13348 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/image_introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/images_dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/settings-sample.template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/settings-schema.partial.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/dark_vs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/themes/terminal_colors.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/data/welcome.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/diagnostics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12845 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/image_manager/puller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/initialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.625551 ansible-navigator-3.3.0/src/ansible_navigator/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8359 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/runner/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/steps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.629551 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/fchainmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/grammars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/tokenize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14939 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/colorize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_curses_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_radio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16065 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_button.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_working.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8201 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9315 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/menu_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/sentinels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33458 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/ansi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/dict_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/dot_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17966 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/packaged_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/print.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.633551 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/src/ansible_navigator/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:53:23.613551 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 14:53:23.000000 ansible-navigator-3.3.0/src/ansible_navigator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-05-16 14:52:59.000000 ansible-navigator-3.3.0/tox.ini
```

### Comparing `ansible-navigator-3.2.0/.config/dictionary.txt` & `ansible-navigator-3.3.0/.config/dictionary.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.flake8` & `ansible-navigator-3.3.0/.flake8`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.git_archival.txt` & `ansible-navigator-3.3.0/.git_archival.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.github/CONTRIBUTING.md` & `ansible-navigator-3.3.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `ansible-navigator-3.3.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.github/SECURITY.md` & `ansible-navigator-3.3.0/.github/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.github/dependabot.yml` & `ansible-navigator-3.3.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.github/workflows/tox.yml` & `ansible-navigator-3.3.0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.gitignore` & `ansible-navigator-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.pre-commit-config.yaml` & `ansible-navigator-3.3.0/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   - repo: https://github.com/psf/black.git
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.263"
+    rev: "v0.0.267"
     hooks:
       - id: ruff
         args:
           - "--exit-non-zero-on-fix"
 
   - repo: https://github.com/streetsidesoftware/cspell-cli
     rev: v6.31.0
@@ -80,15 +80,15 @@
     # Allow json comments, trailing commas
     # https://github.com/pre-commit/pre-commit-hooks/issues/395
     rev: v1.0.0
     hooks:
       - id: check-json5
 
   - repo: https://github.com/igorshubovych/markdownlint-cli
-    rev: v0.33.0
+    rev: v0.34.0
     hooks:
       - id: markdownlint
         exclude: >
           (?x)^
             (
               \.github/ISSUE_TEMPLATE/\w+|
               docs/(
@@ -131,20 +131,20 @@
         language_version: python3
         additional_dependencies:
           - darglint
           - flake8-docstrings # uses pydocstyle
 
   - repo: https://github.com/asottile/pyupgrade
     # keep it after flake8
-    rev: v3.3.1
+    rev: v3.4.0
     hooks:
       - id: pyupgrade
         args: ["--py39-plus"]
   - repo: https://github.com/pre-commit/mirrors-mypy.git
-    rev: v1.2.0
+    rev: v1.3.0
     hooks:
       - id: mypy
         additional_dependencies:
           - jinja2
           - libtmux
           - pytest
           - pytest-mock
```

### Comparing `ansible-navigator-3.2.0/.prettierignore` & `ansible-navigator-3.3.0/.prettierignore`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.vscode/launch.json` & `ansible-navigator-3.3.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/.vscode/settings.json` & `ansible-navigator-3.3.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/LICENSE` & `ansible-navigator-3.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/PKG-INFO` & `ansible-navigator-3.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.2.0
+Version: 3.3.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.2.0/README.md` & `ansible-navigator-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/cspell.config.yaml` & `ansible-navigator-3.3.0/cspell.config.yaml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/_ext/regenerate_docs.py` & `ansible-navigator-3.3.0/docs/_ext/regenerate_docs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/contributing/guidelines.md` & `ansible-navigator-3.3.0/docs/contributing/guidelines.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/contributing/security.md` & `ansible-navigator-3.3.0/docs/contributing/security.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/faq.md` & `ansible-navigator-3.3.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/index.md` & `ansible-navigator-3.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/installation.md` & `ansible-navigator-3.3.0/docs/installation.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/settings.md` & `ansible-navigator-3.3.0/docs/settings.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/docs/subcommands.md` & `ansible-navigator-3.3.0/docs/subcommands.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.asottile_tm_tokenize.all.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.asottile_tm_tokenize.all.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.dark_vs.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.dark_vs.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.source.json.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.source.json.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.source.shell.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.source.shell.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.source.yaml.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.source.yaml.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.text.html.markdown.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.text.html.markdown.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/licenses/LICENSE.text.log.json.txt` & `ansible-navigator-3.3.0/licenses/LICENSE.text.log.json.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/mkdocs.yml` & `ansible-navigator-3.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/mypy.ini` & `ansible-navigator-3.3.0/mypy.ini`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/requirements.txt` & `ansible-navigator-3.3.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #
 # This file is autogenerated by pip-compile with python 3.9
 # To update, run:
 #
 #    pip-compile --extra=docs --extra=test --no-annotate --output-file=requirements.txt --strip-extras setup.cfg
 #
-ansible-builder==3.0.0rc1
+ansible-builder==3.0.0
 ansible-core==2.14.3
 ansible-runner==2.3.2
 attrs==22.2.0
 beautifulsoup4==4.12.0
 bindep==2.11.0
 cairocffi==1.5.0
 cairosvg==2.7.0
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/_version_doc_cache.py` & `ansible-navigator-3.3.0/src/ansible_navigator/_version_doc_cache.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/action_base.py` & `ansible-navigator-3.3.0/src/ansible_navigator/action_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,28 +74,28 @@
                 name=self._name,
                 rerun=self.rerun,
                 stdout=self.stdout,
                 steps=self.steps,
                 update=self.update,
                 write_artifact=self.write_artifact,
             )
-        raise AttributeError("app passed without args initialized")
+        msg = "app passed without args initialized"
+        raise AttributeError(msg)
 
     def no_interactive_mode(self, interaction: Interaction, app: AppPublic) -> None:
-        # pylint: disable=unused-argument
         """Show a warning notification that the user interactive mode is not supported.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         """
         warning = warning_notification(
             messages=[
                 f"The '{self._name}' subcommand is not available while using interactive mode.",
                 "[HINT] Start an additional instance of ansible-navigator"
-                + " in a new terminal with mode 'stdout'.",
+                " in a new terminal with mode 'stdout'.",
                 f"      e.g. 'ansible-navigator {self._name} --mode stdout",
             ],
         )
         interaction.ui.show_form(warning)
 
     @staticmethod
     def _copy_args(args: ApplicationConfiguration) -> ApplicationConfiguration:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/action_defs.py` & `ansible-navigator-3.3.0/src/ansible_navigator/action_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/action_runner.py` & `ansible-navigator-3.3.0/src/ansible_navigator/action_runner.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/__init__.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,18 +14,19 @@
 """
 from __future__ import annotations
 
 from typing import Any
 from typing import Callable
 from typing import Optional
 
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 get: Callable[[str], Any] = actions.get_factory(__package__)
 
 names = actions.names_factory(__package__)
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/_actions.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 import re
 
 from collections import namedtuple
 from collections.abc import Generator
 from typing import Any
 from typing import Callable
 
-from ..action_defs import RunStdoutReturn
-from ..ui_framework import error_notification
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.ui_framework import error_notification
 
 
 logger = logging.getLogger(__name__)
 
 # Basic structure for storing information about one action
 ActionT = namedtuple("ActionT", ("name", "cls", "kegex"))
 
@@ -39,18 +39,16 @@
 
 def _import_all(package: str) -> None:
     """Import all actions in a package.
 
     :param package: The name of the package
     """
     for entry in importlib_resources.files(package).iterdir():
-        if entry.is_file():
-            if entry.name.endswith(".py"):
-                if not entry.name.startswith("_"):
-                    _import(package, entry.name[0:-3])
+        if entry.is_file() and entry.name.endswith(".py") and not entry.name.startswith("_"):
+            _import(package, entry.name[0:-3])
 
 
 def register(cls: Any) -> Any:
     """Register an action, used as a decorator.
 
     :param cls: The class to register
     :returns: The class after registration
@@ -150,15 +148,15 @@
     # Allow tracebacks to bring down the UI, used in tests
     if os.getenv("ANSIBLE_NAVIGATOR_ALLOW_UI_TRACEBACK") == "true":
         return run_action(app=app, interaction=interaction)
 
     # Capture and show a UI notification
     try:
         return run_action(app=app, interaction=interaction)
-    except Exception:  # pylint: disable=broad-except
+    except Exception:
         logger.critical("Subcommand '%s' encountered a fatal error.", action)
         logger.exception("Logging an uncaught exception")
         warn_msg = [f"Unexpected errors were encountered while running '{action}'."]
         warn_msg.append("Please log an issue with the log file contents.")
         warning = error_notification(warn_msg)
         interaction.ui.show_form(warning)
         return None
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/back.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/back.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """``:back`` command implementation.
 
 Additionally triggered by the escape key.
 """
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..steps import Step
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:back`` command implementation."""
 
@@ -33,18 +34,22 @@
         """
         self._logger.debug("back requested")
         interaction.ui.scroll(0)
         interaction.ui.clear()
         this = app.steps.back_one()  # pop this
         step = app.steps.back_one()  # pop current
 
-        if app.steps:
-            if isinstance(step, Step) and isinstance(app.steps.current, Step):
-                if step.type == "menu" and app.steps.current.type == "menu":
-                    interaction.ui.menu_filter(None)
+        if (
+            app.steps
+            and isinstance(step, Step)
+            and isinstance(app.steps.current, Step)
+            and step.type == "menu"
+            and app.steps.current.type == "menu"
+        ):
+            interaction.ui.menu_filter(None)
             self._logger.debug(
                 "Stepping back in %s from %s to %s",
                 app.name,
                 step.name,
                 app.steps.current.name,
             )
         else:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/builder.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 global subcommand registry.
 """
 from __future__ import annotations
 
 import os
 import shutil
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..configuration_subsystem.definitions import Constants
-from ..runner import Command
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.configuration_subsystem.definitions import Constants
+from ansible_navigator.runner import Command
+
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
     """Run the builder subcommand."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/collections.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,37 @@
 
 from copy import deepcopy
 from json.decoder import JSONDecodeError
 from pathlib import Path
 from typing import Any
 from typing import cast
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..runner import Command
-from ..steps import Step
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Interaction
-from ..ui_framework import nonblocking_notification
-from ..ui_framework import warning_notification
-from ..utils.functions import path_is_relative_to
-from ..utils.functions import remove_dbl_un
-from ..utils.key_value_store import KeyValueStore
-from ..utils.print import print_to_stdout
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.runner import Command
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import nonblocking_notification
+from ansible_navigator.ui_framework import warning_notification
+from ansible_navigator.utils.functions import path_is_relative_to
+from ansible_navigator.utils.functions import remove_dbl_un
+from ansible_navigator.utils.key_value_store import KeyValueStore
+from ansible_navigator.utils.print import print_to_stdout
+
 from . import _actions as actions
 from . import run_action
 
 
 def color_menu(colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
-    # pylint: disable=unused-argument
     """Provide a color for a collections menu entry in one column.
 
     :param colno: The column number
     :param colname: The column name
     :param entry: The menu entry
     :returns: The color and decoration
     """
@@ -184,26 +184,26 @@
         args_updated = self._update_args(params=[], attach_cdc=True)
         if not args_updated or not isinstance(
             self._args.internals.collection_doc_cache,
             KeyValueStore,
         ):
             msg = (
                 "Failed to create collections cache, "
-                + "Please review the ansible-navigator log file for errors."
+                "Please review the ansible-navigator log file for errors."
             )
             return RunStdoutReturn(message=msg, return_code=1)
 
         self._collection_cache = self._args.internals.collection_doc_cache
         self._collection_cache_path = self._args.collection_doc_cache_path
 
         self._run_runner()
         if not self._collections:
             msg = (
                 "Failed to catalog collections, "
-                + "Please review the ansible-navigator log file for errors."
+                "Please review the ansible-navigator log file for errors."
             )
             return RunStdoutReturn(message=msg, return_code=1)
 
         collections_info = self._parse_collection_info_stdout()
 
         print_to_stdout(
             content=collections_info,
@@ -287,15 +287,15 @@
         )
 
     def _build_collection_content_menu(self):
         """Build the menu of plugins.
 
         :returns: The plugin menu definition
         """
-        self._collection_cache.open()
+        self._collection_cache.open_()
         selected_collection = self._collections[self.steps.current.index]
         collection_name = f"__{selected_collection['known_as']}"
         collection_contents = []
         for plugin_checksum, details in selected_collection["plugin_checksums"].items():
             try:
                 plugin_json = self._collection_cache[plugin_checksum]
                 loaded = json.loads(plugin_json)
@@ -365,16 +365,14 @@
             name="collection_content",
             step_type="content",
             value=self.steps.current.value,
             index=self.steps.current.index,
         )
 
     def _run_runner(self) -> None:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
         # pylint: disable=too-many-locals
         """Use the runner subsystem to catalog collections."""
         if isinstance(self._args.set_environment_variable, dict):
             set_environment_variable = deepcopy(self._args.set_environment_variable)
         else:
             set_environment_variable = {}
         set_environment_variable["ANSIBLE_NOCOLOR"] = "True"
@@ -508,17 +506,16 @@
 
     def _parse(self, output) -> None:
         """Load and process the ``json`` output from the collection cataloging process.
 
         :param output: The output from the collection cataloging process
         :returns: Nothing
         """
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
+
         try:
             if not output.startswith("{"):
                 _warnings, json_str = output.split("{", 1)
                 json_str = "{" + json_str
             else:
                 json_str = output
             parsed = json.loads(json_str)
@@ -559,17 +556,17 @@
             dest_volume_mounts = tuple()
 
         for collection in self._collections:
             collection["__name"] = collection["known_as"]
             collection["__version"] = collection["collection_info"].get("version", "missing")
             collection["__shadowed"] = bool(collection["hidden_by"])
             if self._args.execution_environment:
-                if collection["path"].startswith(dest_volume_mounts):
-                    collection["__type"] = "bind_mount"
-                elif collection["path"].startswith(self._adjacent_collection_dir):
+                if collection["path"].startswith(dest_volume_mounts) or collection[
+                    "path"
+                ].startswith(self._adjacent_collection_dir):
                     collection["__type"] = "bind_mount"
                 elif collection["path"].startswith(os.path.dirname(self._adjacent_collection_dir)):
                     collection["__type"] = "bind_mount"
                     error = (
                         f"{collection['known_as']} was mounted and catalogued in the"
                         " execution environment but was outside the adjacent 'collections'"
                         " directory. This may cause issues outside the local development"
@@ -650,15 +647,15 @@
             "meta_source",
             "plugin_checksums",
             "runtime",
         ]
         roles_exclude_keys = ["readme"]
         self._collection_cache = cast(KeyValueStore, self._collection_cache)
 
-        self._collection_cache.open()
+        self._collection_cache.open_()
         for collection in self._collections:
             plugins_details = self._get_collection_plugins_details(collection)
 
             collection_stdout: dict = {}
             for info_name, info_value in collection.items():
                 info_name = remove_dbl_un(info_name)
                 if info_name in collection_exclude_keys:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/config.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/config.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import os
 import re
 import shlex
 import shutil
 
 from typing import Any
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..runner import AnsibleConfig
-from ..runner import Command
-from ..steps import Step
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Interaction
-from ..ui_framework import nonblocking_notification
-from ..ui_framework import warning_notification
-from ..utils.serialize import Loader
-from ..utils.serialize import yaml
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.runner import AnsibleConfig
+from ansible_navigator.runner import Command
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import nonblocking_notification
+from ansible_navigator.ui_framework import warning_notification
+from ansible_navigator.utils.serialize import Loader
+from ansible_navigator.utils.serialize import yaml
+
 from . import _actions as actions
 from . import run_action
 
 
 def color_menu(colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
-    # pylint: disable=unused-argument
     """Provide a color for a collections menu entry in one column.
 
     :param colno: The column number
     :param colname: The column name
     :param entry: The menu entry
     :returns: The color and decoration
     """
@@ -205,16 +205,14 @@
             name="option_content",
             step_type="content",
             value=self._config,
             index=self.steps.current.index,
         )
 
     def _run_runner(self) -> tuple | None:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
         """Use the runner subsystem to retrieve the configuration.
 
         :raises RuntimeError: When the ansible-config command cannot be found with execution
             environment support disabled.
         :returns: For mode interactive nothing. For mode stdout the
             output, errors and return code from runner.
         """
@@ -304,15 +302,14 @@
     def _parse_and_merge(self, list_output, dump_output) -> None:
         """Parse the list and dump output. Merge dump into list.
 
         :param list_output: The output from config list
         :param dump_output: The output from config dump
         :returns: Nothing
         """
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
         try:
             parsed = yaml.load(list_output, Loader=Loader)
             self._logger.debug("yaml loading list output succeeded")
         except yaml.YAMLError as exc:
             self._logger.debug("error yaml loading list output: '%s'", str(exc))
             return None
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/doc.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/doc.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import json
 import os
 import shlex
 import shutil
 
 from typing import Any
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem import Constants as C
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..runner import AnsibleDoc
-from ..runner import Command
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Interaction
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem import Constants as C
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.runner import AnsibleDoc
+from ansible_navigator.runner import Command
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
     """Doc subcommand implementation."""
 
@@ -129,15 +130,14 @@
         if response is None:
             self._logger.error("Unexpected response: %s", response)
             return RunStdoutReturn(message="Please review the log for errors.", return_code=1)
         _out, error, return_code = response
         return RunStdoutReturn(message=error, return_code=return_code)
 
     def _run_runner(self) -> dict | tuple[str, str, int] | None:
-        # pylint: disable=too-many-branches
         # pylint: disable=no-else-return
         """Use the runner subsystem to retrieve the configuration.
 
         :raises RuntimeError: When the ansible-doc command cannot be found with execution
             environment support disabled.
         :returns: For mode interactive nothing or the plugin's doc. For mode stdout the
             output, errors and return code from runner.
@@ -234,15 +234,14 @@
     ) -> dict[Any, Any] | None:
         """Extract the plugin's documentation from the runner output.
 
         :param out: The output from runner
         :param err: Any runner errors
         :returns: The plugin's doc or errors
         """
-        # pylint: disable=too-many-branches
         plugin_doc = {}
         if self._args.execution_environment:
             error_key_name = "execution_environment_errors"
         else:
             error_key_name = "local_errors"
 
         if out:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/exec.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/exec.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 
 import logging
 import os
 import shlex
 
 from typing import Optional
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..configuration_subsystem.definitions import Constants
-from ..runner import Command
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.configuration_subsystem.definitions import Constants
+from ansible_navigator.runner import Command
+
 from . import _actions as actions
 
 
 GeneratedCommand = tuple[str, Optional[list[str]]]
 
 logger = logging.getLogger(__name__)
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/filter.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """``:filter`` command implementation."""
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:filter`` command implementation."""
 
@@ -17,15 +18,14 @@
         """Initialize the ``:filter`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
-    # pylint: disable=unused-argument
     def run(self, interaction: Interaction, app: AppPublic) -> None:
         """Execute the ``:filter`` request.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         """
         self._logger.debug("filter requested")
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/help_doc.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/help_doc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """``:help`` command implementation."""
 
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
 from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.utils.packaged_data import retrieve_content
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
-from ..utils.packaged_data import retrieve_content
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
     """``:help`` command implementation."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/images.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/images.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 import json
 import shlex
 
 from copy import deepcopy
 from functools import partial
 from typing import Any
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem import Constants
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..image_manager import inspect_all
-from ..runner import Command
-from ..steps import Step
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Interaction
-from ..ui_framework import nonblocking_notification
-from ..ui_framework import warning_notification
-from ..utils.print import print_to_stdout
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem import Constants
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.image_manager import inspect_all
+from ansible_navigator.runner import Command
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import nonblocking_notification
+from ansible_navigator.ui_framework import warning_notification
+from ansible_navigator.utils.print import print_to_stdout
+
 from . import _actions as actions
 from . import run_action
 
 
 def filter_content_keys(obj: dict[Any, Any]) -> dict[Any, Any]:
     """Filter out some keys when showing image content.
 
@@ -65,15 +66,14 @@
             step_type="menu",
             columns=["__image", "tag", "execution_environment", "created", "size"],
             value=[],
             select_func=self._build_image_menu,
         )
 
     def color_menu(self, colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
-        # pylint: disable=unused-argument
         """Provide a color for a images menu entry in one column.
 
         :param colno: The column number
         :param colname: The column name
         :param entry: The menu entry
         :returns: The color and decoration
         """
@@ -562,15 +562,15 @@
             "navigator_mode": "interactive",
         }
 
         if isinstance(self._args.container_options, list):
             kwargs.update({"container_options": self._args.container_options})
 
         self._logger.debug(
-            f"Invoke runner with executable_cmd: {python_exec_path}" + f" and kwargs: {kwargs}",
+            "Invoke runner with executable_cmd: %s and kwargs: %s", python_exec_path, kwargs
         )
         _runner = Command(executable_cmd=python_exec_path, **kwargs)
         output, error, return_code = _runner.run()
         return output, error, return_code
 
     def notify_failed(self):
         """Notify image introspection failed."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/inventory.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/inventory.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 import os
 import shlex
 import shutil
 
 from pathlib import Path
 from typing import Any
 
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
 from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.runner import AnsibleInventory
+from ansible_navigator.runner import Command
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import Color
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Decoration
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import warning_notification
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..runner import AnsibleInventory
-from ..runner import Command
-from ..steps import Step
-from ..ui_framework import Color
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Decoration
-from ..ui_framework import Interaction
-from ..ui_framework import warning_notification
 from . import _actions as actions
 from . import run_action
 
 
 def color_menu(colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
     """Provide a color for a inventory menu entry in one column.
 
@@ -134,15 +134,15 @@
         :param value: The inventory data
         """
         self.__inventory = value
         self._host_vars = {
             k: {**v, "inventory_hostname": k}
             for k, v in value.get("_meta", {}).get("hostvars", {}).items()
         }
-        for group in self._inventory.keys():
+        for group in self._inventory:
             for host in self._inventory[group].get("hosts", []):
                 if host in self._host_vars:
                     continue
                 self._host_vars[host] = {"inventory_hostname": host}
 
     @property
     def _show_columns(self) -> list:
@@ -316,15 +316,16 @@
         :raises IndexError: When the index does not correspond to a menu entry
         :returns: Either the group or host menu
         """
         if self.steps.current.index == 0:
             return self._build_group_menu("all")
         if self.steps.current.index == 1:
             return self._build_host_menu()
-        raise IndexError("broken modules somewhere?")
+        msg = "broken modules somewhere?"
+        raise IndexError(msg)
 
     def _build_group_menu(self, key=None) -> Step:
         """Build the menu for inventory groups.
 
         :param key: The optional menu name
         :returns: The inventory group menu definition
         """
@@ -428,21 +429,21 @@
         :raises TypeError: When the step type is unknown
         :returns: The group or host menu definition
         """
         if self.steps.current.selected["__type"] == "group":
             return self._build_group_menu()
         if self.steps.current.selected["__type"] == "host":
             return self._build_host_content()
-        raise TypeError("unknown step type")
+        msg = "unknown step type"
+        raise TypeError(msg)
 
     def _collect_inventory_details_interactive(
         self,
         kwargs: dict[str, Any],
     ) -> None:
-        # pylint: disable=too-many-branches
         """Use the runner subsystem to collect inventory details for mode interactive.
 
         :param kwargs: The arguments for the runner call
         """
         try:
             # Extract the playbook dir the user may have provided
             index = self._args.cmdline.index("--playbook-dir")
@@ -464,23 +465,16 @@
         inventory_output, inventory_err = self._runner.fetch_inventory(
             action="list",
             inventories=self._inventories,
             playbook_dir=playbook_dir,
         )
         if inventory_output:
             parts = inventory_output.split("{", 1)
-            if inventory_err:
-                inventory_err = parts[0] + inventory_err
-            else:
-                inventory_err = parts[0]
-
-            if len(parts) == 2:
-                inventory_output = "{" + parts[1]
-            else:
-                inventory_output = ""
+            inventory_err = parts[0] + inventory_err if inventory_err else parts[0]
+            inventory_output = "{" + parts[1] if len(parts) == 2 else ""
         preface = ["Errors were encountered while gathering the inventory:"]
         notify = ("ERROR!", "Error", "Unable to parse")
         if any(string in inventory_err for string in notify):
             if "[WARNING]" in inventory_err:
                 parts = inventory_err.split("[WARNING]")
                 messages = [part.replace("\n", " ").strip() for part in parts if part]
                 present = preface + [f"[WARNING]{message}" for message in messages]
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/lint.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/lint.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,32 +21,33 @@
 import shlex
 
 from collections.abc import Mapping
 from datetime import datetime
 from enum import IntEnum
 from typing import Any
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..runner.command import Command
-from ..steps import Step
-from ..ui_framework import Color
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Decoration
-from ..ui_framework import Interaction
-from ..ui_framework import error_notification
-from ..ui_framework import nonblocking_notification
-from ..ui_framework import success_notification
-from ..utils.functions import abs_user_path
-from ..utils.functions import remove_ansi
-from ..utils.functions import time_stamp_for_file
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.runner.command import Command
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import Color
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Decoration
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import error_notification
+from ansible_navigator.ui_framework import nonblocking_notification
+from ansible_navigator.ui_framework import success_notification
+from ansible_navigator.utils.functions import abs_user_path
+from ansible_navigator.utils.functions import remove_ansi
+from ansible_navigator.utils.functions import time_stamp_for_file
+
 from . import _actions as actions
 from . import run_action
 
 
 class Severity(IntEnum):
     """A mapping from ansible-lint severity to an integer represented internally.
 
@@ -87,15 +88,14 @@
         return Color.RED
     if severity == "info":
         return Color.CYAN
     return Color.BLACK
 
 
 def color_menu(colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
-    # pylint: disable=unused-argument
     """Color the menu.
 
     :param colno: The column number
     :param colname: The column name
     :param entry: The current content entry
     :returns: The foreground and background color
     """
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/log.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/stdout.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,56 +1,58 @@
-"""``:log`` command implementation."""
+"""``:stdout`` command implementation."""
+
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
 from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
-    """``:log`` command implementation."""
+    """``:stdout`` command implementation."""
 
-    KEGEX = r"^l(?:og)?$"
+    KEGEX = r"^st(?:dout)?$"
 
     def __init__(self, args: ApplicationConfiguration):
-        """Initialize the ``:log`` action.
+        """Initialize the ``:stdout`` action.
 
         :param args: The current settings for the application
         """
-        super().__init__(args=args, logger_name=__name__, name="log")
+        super().__init__(args=args, logger_name=__name__, name="stdout")
 
     def run(self, interaction: Interaction, app: AppPublic) -> Interaction:
-        """Execute the ``:log`` request for mode interactive.
+        """Execute the ``:stdout`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         :returns: The pending :class:`~ansible_navigator.ui_framework.ui.Interaction`
         """
-        self._logger.debug("log requested")
+        self._logger.debug("stdout requested")
         self._prepare_to_run(app, interaction)
 
         auto_scroll = True
         while True:
             self._calling_app.update()
-            with open(self._args.log_file, encoding="utf-8") as fh:
-                log_contents = fh.read()
 
-            new_scroll = len(log_contents.splitlines())
+            new_scroll = len(self._calling_app.stdout)
             if auto_scroll:
                 interaction.ui.scroll(new_scroll)
-
-            interaction = interaction.ui.show(obj=log_contents, content_format=ContentFormat.LOG)
-            if interaction.name != "refresh":
+            obj = "\n".join(app.stdout)
+            next_interaction: Interaction = interaction.ui.show(
+                obj=obj,
+                content_format=ContentFormat.ANSI,
+            )
+            if next_interaction.name != "refresh":
                 break
 
             if interaction.ui.scroll() < new_scroll and auto_scroll:
                 self._logger.debug("auto_scroll disabled")
                 auto_scroll = False
             elif interaction.ui.scroll() >= new_scroll and not auto_scroll:
                 self._logger.debug("auto_scroll enabled")
                 auto_scroll = True
 
         self._prepare_to_exit(interaction)
-        return interaction
+        return next_interaction
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/open_file.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/open_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,25 +6,26 @@
 import os
 
 from pathlib import Path
 from typing import Any
 from typing import Callable
 from typing import Optional
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentBase
-from ..content_defs import ContentFormat
-from ..content_defs import ContentType
-from ..content_defs import ContentView
-from ..content_defs import SerializationFormat
-from ..ui_framework import Interaction
-from ..ui_framework import Menu
-from ..utils.functions import remove_dbl_un
-from ..utils.serialize import serialize_write_temp_file
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentBase
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.content_defs import ContentType
+from ansible_navigator.content_defs import ContentView
+from ansible_navigator.content_defs import SerializationFormat
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import Menu
+from ansible_navigator.utils.functions import remove_dbl_un
+from ansible_navigator.utils.serialize import serialize_write_temp_file
+
 from . import _actions as actions
 
 
 class SuspendCurses:
     """Context Manager to temporarily leave curses mode."""
 
     def __enter__(self):
@@ -145,15 +146,14 @@
             content=content,
             content_view=ContentView.NORMAL,
             content_format=content_format,
         )
         return file_name
 
     def run(self, interaction: Interaction, app: AppPublic) -> None:
-        # pylint: disable=unused-argument
         """Execute the ``:open`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         :returns: Nothing
         """
         self._logger.debug("open requested")
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/quit.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/quit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """``:quit`` command implementation."""
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:quit`` command implementation."""
 
@@ -17,15 +18,14 @@
         """Initialize the ``:quit`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
-    # pylint: disable=unused-argument
     def run(self, interaction: Interaction, app: AppPublic) -> Interaction:
         """Handle a request to quit the application from the user interface.
 
         The application exit is ultimately handled by
         :class:`~ansible_navigator.action_runner.ActionRunner` so return immediately,
         passing the ``:quit`` request backwards through the stack of actions that are on the stack.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/refresh.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/rerun.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-"""Screen refresh implementation."""
+"""``:rerun`` command implementation."""
+import copy
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
-    """Screen refresh implementation."""
+    """``:rerun`` command implementation."""
 
-    KEGEX = r"^KEY_F\(5\)$"
+    KEGEX = r"^rr|rerun?$"
 
     def __init__(self, args: ApplicationConfiguration):
-        """Initialize the refresh action.
+        """Initialize the ``:rerun`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
     def run(self, interaction: Interaction, app: AppPublic) -> None:
-        """Execute the screen refresh request for mode interactive.
+        """Execute the ``:rerun`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         """
-        # Just in case the user switched tasks with +,- etc
-        # change previous, since this interaction is on the stack
-        if interaction.content:
-            app.steps.previous.index = interaction.action.value
+        self._logger.debug("rerun requested")
+        this = copy.copy(app.steps.current)
+        app.rerun()
+        # ensure we are last on the stack
+        if app.steps.current != this:
+            app.steps.append(this)
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/run.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,40 +14,41 @@
 from math import floor
 from operator import itemgetter
 from pathlib import Path
 from queue import Queue
 from typing import Any
 from typing import Callable
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem import to_effective
-from ..configuration_subsystem import to_sources
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentView
-from ..content_defs import SerializationFormat
-from ..runner import CommandAsync
-from ..steps import Step
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Interaction
-from ..ui_framework import dict_to_form
-from ..ui_framework import form_to_dict
-from ..ui_framework import nonblocking_notification
-from ..ui_framework import warning_notification
-from ..utils.functions import abs_user_path
-from ..utils.functions import check_playbook_type
-from ..utils.functions import human_time
-from ..utils.functions import is_jinja
-from ..utils.functions import now_iso
-from ..utils.functions import remove_ansi
-from ..utils.functions import round_half_up
-from ..utils.serialize import serialize_write_file
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem import to_effective
+from ansible_navigator.configuration_subsystem import to_sources
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentView
+from ansible_navigator.content_defs import SerializationFormat
+from ansible_navigator.runner import CommandAsync
+from ansible_navigator.steps import Step
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import dict_to_form
+from ansible_navigator.ui_framework import form_to_dict
+from ansible_navigator.ui_framework import nonblocking_notification
+from ansible_navigator.ui_framework import warning_notification
+from ansible_navigator.utils.functions import abs_user_path
+from ansible_navigator.utils.functions import check_playbook_type
+from ansible_navigator.utils.functions import human_time
+from ansible_navigator.utils.functions import is_jinja
+from ansible_navigator.utils.functions import now_iso
+from ansible_navigator.utils.functions import remove_ansi
+from ansible_navigator.utils.functions import round_half_up
+from ansible_navigator.utils.serialize import serialize_write_file
+
 from . import _actions as actions
 from . import run_action
 from .stdout import Action as stdout_action
 
 
 RESULT_TO_COLOR = [
     ("(?i)^failed$", 9),
@@ -67,15 +68,14 @@
     return next(  # noqa: E731
         (x[1] for x in RESULT_TO_COLOR if re.match(x[0], word)),
         0,
     )
 
 
 def color_menu(_colno: int, colname: str, entry: dict[str, Any]) -> tuple[int, int]:
-    # pylint: disable=too-many-branches
     """Find matching color for word.
 
     :param colname: The column name
     :param entry: The menu entry
     :returns: The color and decoration
     """
     colval = entry[colname]
@@ -97,23 +97,20 @@
         else:
             color = get_color(colname[2:])
 
         if colname == "__progress" and entry["__progress"].strip().lower() == "complete":
             decoration = curses.A_BOLD
 
     elif "task" in entry:
-        if entry["__result"].lower() == "in progress":
-            color = get_color(entry["__result"])
-        elif colname in ["__result", "__host", "__number", "__task", "__task_action"]:
+        if entry["__result"].lower() == "in progress" or (
+            colname in ["__result", "__host", "__number", "__task", "__task_action"]
+        ):
             color = get_color(entry["__result"])
         elif colname == "__changed":
-            if colval is True:
-                color = 11
-            else:
-                color = get_color(entry["__result"])
+            color = 11 if colval is True else get_color(entry["__result"])
         elif colname == "__duration":
             color = 12
 
     return color, decoration
 
 
 def content_heading(obj: Any, screen_w: int) -> CursesLines | None:
@@ -345,15 +342,14 @@
                     self._prepare_to_exit(interaction)
                     return self.steps.current
                 self.steps.back_one()
 
         self._prepare_to_exit(interaction)
         return None
 
-    # pylint: disable=too-many-branches
     def _init_run(self) -> bool:
         """In the case of :run, check the user input.
 
         :returns: True
         """
         # Ensure the playbook and inventory are valid
 
@@ -486,23 +482,17 @@
     def _prompt_for_playbook(self) -> dict[Any, Any]:
         """Pre-populate a form to confirm the playbook details.
 
         :returns: Dict with playbook and inventory detail entries
         """
         self._logger.debug("Inventory/Playbook not set, provided, or valid, prompting")
 
-        if isinstance(self._args.playbook, str):
-            playbook = self._args.playbook
-        else:
-            playbook = ""
+        playbook = self._args.playbook if isinstance(self._args.playbook, str) else ""
 
-        if isinstance(self._args.cmdline, list):
-            cmdline = " ".join(self._args.cmdline)
-        else:
-            cmdline = ""
+        cmdline = " ".join(self._args.cmdline) if isinstance(self._args.cmdline, list) else ""
 
         FType = dict[str, Any]
         form_dict: FType = {
             "title": "Playbook not found, please confirm the following",
             "fields": [],
         }
         form_field = {
@@ -569,18 +559,15 @@
     def _run_runner(self) -> None:
         """Spin up runner.
 
         :raises RuntimeError: If no ansible-playbook executable
         """
         executable_cmd: str | None
 
-        if self.mode == "stdout_w_artifact":
-            mode = "interactive"
-        else:
-            mode = self.mode
+        mode = "interactive" if self.mode == "stdout_w_artifact" else self.mode
 
         if isinstance(self._args.set_environment_variable, dict):
             set_env_vars = {**self._args.set_environment_variable}
         else:
             set_env_vars = {}
 
         if self._args.display_color is False:
@@ -646,18 +633,15 @@
             message = self._queue.get()
             self._handle_message(message)
             drain_count += 1
         if drain_count:
             self._logger.debug("Drained %s events", drain_count)
 
     def _handle_message(self, message: dict) -> None:
-        # pylint: disable=too-many-branches
-        # pylint: disable=too-many-statements
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-return-statements
         """Handle a runner message.
 
         :param message: The message from runner
         :type message: dict
         """
         # Collect any stdout
         if "stdout" in message and message["stdout"]:
@@ -925,15 +909,15 @@
                     file=Path(filename),
                     serialization_format=SerializationFormat.JSON,
                 )
                 self._logger.info("Saved artifact as %s", filename)
 
             except OSError as exc:
                 error = (
-                    f"Saving the artifact file failed, resulted in the following error: f{str(exc)}"
+                    f"Saving the artifact file failed, resulted in the following error: f{exc!s}"
                 )
                 self._logger.error(error)
 
     def rerun(self) -> None:
         """Rerun the current playbook.
 
         Since we're not reinstating run, drain the queue,
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_form.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """``:sample_form`` command implementation."""
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
-from ..ui_framework import dict_to_form
-from ..ui_framework import form_to_dict
-from ..utils.serialize import yaml
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import dict_to_form
+from ansible_navigator.ui_framework import form_to_dict
+from ansible_navigator.utils.serialize import yaml
+
 from . import _actions as actions
 
 
 FORM = """
 form:
   title:  Please confirm the following information
   fields:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/sample_notification.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/sample_notification.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """``:sample_notification`` command implementation."""
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
-from ..ui_framework import dict_to_form
-from ..ui_framework import form_to_dict
-from ..utils.serialize import yaml
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import dict_to_form
+from ansible_navigator.ui_framework import form_to_dict
+from ansible_navigator.utils.serialize import yaml
+
 from . import _actions as actions
 
 
 # cspell:disable
 FORM = """
 form:
   title:  BLOCKING NOTIFICATION
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/save.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/save.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """``:save`` command implementation."""
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:save`` command implementation."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/select.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/select.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 Processor of a menu selection from a numeric key press
 or entry at the single line prompt. e.g ``:42``
 """
 
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """Menu selection implementation."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_json.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_json.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """``:json`` command implementation."""
 import logging
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..ui_framework import Interaction
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
+
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:json`` command implementation."""
 
@@ -18,15 +19,14 @@
         """Initialize the ``:json`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
-    # pylint: disable=unused-argument
     def run(self, interaction: Interaction, app: AppPublic) -> None:
         """Execute the ``:json`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         """
         self._logger.debug("json requested")
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/serialize_yaml.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/serialize_yaml.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """``:yaml`` command implementation."""
 import logging
 
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
 from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..ui_framework import Interaction
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:yaml`` command implementation."""
 
@@ -19,15 +19,14 @@
         """Initialize the ``:yaml`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
-    # pylint: disable=unused-argument
     def run(self, interaction: Interaction, app: AppPublic) -> None:
         """Execute the ``:yaml`` request for mode interactive.
 
         :param interaction: The interaction from the user, action and value
         :param app: The app instance
         """
         self._logger.debug("yaml requested")
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/settings.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/settings.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 """The ``settings`` subcommand action."""
 from __future__ import annotations
 
 from dataclasses import asdict
 from functools import partial
 
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.action_defs import RunStdoutReturn
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem import PresentableSettingsEntries
+from ansible_navigator.configuration_subsystem import PresentableSettingsEntry
+from ansible_navigator.configuration_subsystem import to_effective
+from ansible_navigator.configuration_subsystem import to_presentable
+from ansible_navigator.configuration_subsystem import to_sample
+from ansible_navigator.configuration_subsystem import to_schema
+from ansible_navigator.configuration_subsystem import to_sources
 from ansible_navigator.configuration_subsystem.definitions import Constants
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.steps import StepType
+from ansible_navigator.steps import TypedStep
+from ansible_navigator.ui_framework import Color
+from ansible_navigator.ui_framework import CursesLine
+from ansible_navigator.ui_framework import CursesLinePart
+from ansible_navigator.ui_framework import CursesLines
+from ansible_navigator.ui_framework import Decoration
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.utils.print import print_to_stdout
 
-from ..action_base import ActionBase
-from ..action_defs import RunStdoutReturn
-from ..app_public import AppPublic
-from ..configuration_subsystem import PresentableSettingsEntries
-from ..configuration_subsystem import PresentableSettingsEntry
-from ..configuration_subsystem import to_effective
-from ..configuration_subsystem import to_presentable
-from ..configuration_subsystem import to_sample
-from ..configuration_subsystem import to_schema
-from ..configuration_subsystem import to_sources
-from ..content_defs import ContentFormat
-from ..steps import StepType
-from ..steps import TypedStep
-from ..ui_framework import Color
-from ..ui_framework import CursesLine
-from ..ui_framework import CursesLinePart
-from ..ui_framework import CursesLines
-from ..ui_framework import Decoration
-from ..ui_framework import Interaction
-from ..utils.print import print_to_stdout
 from . import _actions as actions
 from . import run_action
 
 
 def color_menu(colno: int, colname: str, entry: PresentableSettingsEntry) -> tuple[int, int]:
-    # pylint: disable=unused-argument
     """Color the menu.
 
     :param colno: Column number
     :param colname: Column name
     :param entry: Column value
     :returns: Constants that curses uses to color a line of text
     """
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/stdout.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,57 +1,56 @@
-"""``:stdout`` command implementation."""
+"""``:log`` command implementation."""
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..ui_framework import Interaction
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
-    """``:stdout`` command implementation."""
+    """``:log`` command implementation."""
 
-    KEGEX = r"^st(?:dout)?$"
+    KEGEX = r"^l(?:og)?$"
 
     def __init__(self, args: ApplicationConfiguration):
-        """Initialize the ``:stdout`` action.
+        """Initialize the ``:log`` action.
 
         :param args: The current settings for the application
         """
-        super().__init__(args=args, logger_name=__name__, name="stdout")
+        super().__init__(args=args, logger_name=__name__, name="log")
 
     def run(self, interaction: Interaction, app: AppPublic) -> Interaction:
-        """Execute the ``:stdout`` request for mode interactive.
+        """Execute the ``:log`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         :returns: The pending :class:`~ansible_navigator.ui_framework.ui.Interaction`
         """
-        self._logger.debug("stdout requested")
+        self._logger.debug("log requested")
         self._prepare_to_run(app, interaction)
 
         auto_scroll = True
         while True:
             self._calling_app.update()
+            with open(self._args.log_file, encoding="utf-8") as fh:
+                log_contents = fh.read()
 
-            new_scroll = len(self._calling_app.stdout)
+            new_scroll = len(log_contents.splitlines())
             if auto_scroll:
                 interaction.ui.scroll(new_scroll)
-            obj = "\n".join(app.stdout)
-            next_interaction: Interaction = interaction.ui.show(
-                obj=obj,
-                content_format=ContentFormat.ANSI,
-            )
-            if next_interaction.name != "refresh":
+
+            interaction = interaction.ui.show(obj=log_contents, content_format=ContentFormat.LOG)
+            if interaction.name != "refresh":
                 break
 
             if interaction.ui.scroll() < new_scroll and auto_scroll:
                 self._logger.debug("auto_scroll disabled")
                 auto_scroll = False
             elif interaction.ui.scroll() >= new_scroll and not auto_scroll:
                 self._logger.debug("auto_scroll enabled")
                 auto_scroll = True
 
         self._prepare_to_exit(interaction)
-        return next_interaction
+        return interaction
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/template.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,22 +4,23 @@
 """
 from __future__ import annotations
 
 import html
 
 from collections.abc import Mapping
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..ui_framework import Interaction
-from ..ui_framework import warning_notification
-from ..utils.functions import remove_dbl_un
-from ..utils.functions import templar
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.ui_framework import warning_notification
+from ansible_navigator.utils.functions import remove_dbl_un
+from ansible_navigator.utils.functions import templar
+
 from . import _actions as actions
 
 
 @actions.register
 class Action(ActionBase):
     """Template command implementation."""
 
@@ -36,15 +37,14 @@
         """Execute the templating request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         :returns: The pending :class:`~ansible_navigator.ui_framework.ui.Interaction` or
             :data:`None`
         """
-        # pylint: disable=too-many-branches
         self._logger.debug("template requested '%s'", interaction.action.value)
         self._prepare_to_run(app, interaction)
 
         type_msgs = ["Current content passed for templating is not a dictionary."]
         type_msgs.append("[HINT] Use 'this' to reference it (e.g. {{ this[0] }}")
 
         if interaction.content:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/welcome.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/welcome.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """Welcome subcommand implementation."""
 
-from ..action_base import ActionBase
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import ContentFormat
-from ..ui_framework import Interaction
-from ..utils.packaged_data import retrieve_content
+from ansible_navigator.action_base import ActionBase
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.utils.packaged_data import retrieve_content
+
 from . import _actions as actions
 
 
 WELCOME = """
 
 """
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/actions/write_file.py` & `ansible-navigator-3.3.0/src/ansible_navigator/actions/write_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """``:write`` command implementation."""
 import logging
 import os
 import re
 
 from pathlib import Path
 
+from ansible_navigator.app_public import AppPublic
+from ansible_navigator.configuration_subsystem.definitions import ApplicationConfiguration
 from ansible_navigator.content_defs import ContentView
+from ansible_navigator.content_defs import SerializationFormat
+from ansible_navigator.ui_framework import Interaction
+from ansible_navigator.utils.functions import remove_dbl_un
+from ansible_navigator.utils.serialize import serialize_write_file
 
-from ..app_public import AppPublic
-from ..configuration_subsystem.definitions import ApplicationConfiguration
-from ..content_defs import SerializationFormat
-from ..ui_framework import Interaction
-from ..utils.functions import remove_dbl_un
-from ..utils.serialize import serialize_write_file
 from . import _actions as actions
 
 
 @actions.register
 class Action:
     """``:write`` command implementation."""
 
@@ -26,23 +26,21 @@
         """Initialize the ``:write`` action.
 
         :param args: The current settings for the application
         """
         self._args = args
         self._logger = logging.getLogger(__name__)
 
-    # pylint: disable=unused-argument
     def run(self, interaction: Interaction, app: AppPublic) -> None:
         """Execute the ``:write`` request for mode interactive.
 
         :param interaction: The interaction from the user
         :param app: The app instance
         :returns: Nothing
         """
-        # pylint: disable=too-many-branches
         self._logger.debug("write requested as %s", interaction.action.value)
         match = interaction.action.match.groupdict()
         filename = os.path.abspath(match["filename"])
         if match["append"]:
             if not os.path.exists(filename) and not match["force"]:
                 self._logger.warning(
                     "Append operation failed because %s does not exist, force with !",
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/app_public.py` & `ansible-navigator-3.3.0/src/ansible_navigator/app_public.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/cli.py` & `ansible-navigator-3.3.0/src/ansible_navigator/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,18 +77,15 @@
     pkgs = []
     found = []
     for _python_name, pkg_names in importlib_metadata.packages_distributions().items():
         for pkg_name in pkg_names:
             if pkg_name not in found:
                 found.append(pkg_name)
                 spec = find_spec(pkg_name)
-                if spec:
-                    _location = spec.origin
-                else:
-                    _location = ""
+                _location = spec.origin if spec else ""
                 _version = version(pkg_name)
                 pkgs.append(f"{pkg_name}=={_version} {_location}")
 
     pkgs.sort()
     messages = [LogMessage(level=logging.DEBUG, message=pkg) for pkg in pkgs]
     return messages
 
@@ -167,18 +164,18 @@
         exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.NOTE))
         exit_msg = "Review the hints and log file to see what went wrong."
         exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
 
     try:
         Path(args.log_file).touch()
         setup_logger(args)
-    except Exception as exc:  # pylint: disable=broad-except
+    except Exception as exc:  # noqa: BLE001
         exit_msg = "The log file path or logging engine could not be setup."
         exit_msg += " No log file will be available, please check the log file"
-        exit_msg += f" path setting. The error was {str(exc)}"
+        exit_msg += f" path setting. The error was {exc!s}"
         exit_messages.append(ExitMessage(message=exit_msg))
         error_and_exit_early(exit_messages=exit_messages)
 
     for entry in messages:
         logger.log(level=entry.level, msg=entry.message)
 
     if exit_messages:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/command_runner/command_runner.py` & `ansible-navigator-3.3.0/src/ansible_navigator/command_runner/command_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 
 from dataclasses import dataclass
 from dataclasses import field
 from queue import Queue
 from typing import Callable
 
-from ..utils.definitions import LogMessage
+from ansible_navigator.utils.definitions import LogMessage
 
 
 PROCESSES = (multiprocessing.cpu_count() - 1) or 1
 
 
 @dataclass(frozen=False)
 class Command:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/__init__.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/configurator.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/configurator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 from __future__ import annotations
 
 import logging
 import os
 
 from copy import deepcopy
 
-from ..utils.definitions import ExitMessage
-from ..utils.definitions import ExitPrefix
-from ..utils.definitions import LogMessage
-from ..utils.functions import oxfordcomma
-from ..utils.functions import shlex_join
-from ..utils.json_schema import validate
-from ..utils.serialize import SafeLoader
-from ..utils.serialize import yaml
-from ..utils.version_migration.migrate import MigrationType
-from ..utils.version_migration.migrate import run_all_migrations
+from ansible_navigator.utils.definitions import ExitMessage
+from ansible_navigator.utils.definitions import ExitPrefix
+from ansible_navigator.utils.definitions import LogMessage
+from ansible_navigator.utils.functions import oxfordcomma
+from ansible_navigator.utils.functions import shlex_join
+from ansible_navigator.utils.json_schema import validate
+from ansible_navigator.utils.serialize import SafeLoader
+from ansible_navigator.utils.serialize import yaml
+from ansible_navigator.utils.version_migration.migrate import MigrationType
+from ansible_navigator.utils.version_migration.migrate import run_all_migrations
+
 from .definitions import ApplicationConfiguration
 from .definitions import Constants as C
 from .definitions import SettingsEntry
 from .parser import Parser
 from .transform import to_schema
 from .utils import parse_ansible_cfg
 
@@ -56,17 +57,19 @@
     def _sanity_check(self) -> None:
         """Sanity check the configuration.
 
         :raises ValueError: If apply_previous_cli is used while initializing
         """
         if self._apply_previous_cli_entries is not C.NONE:
             if self._config.internals.initializing:
-                raise ValueError("'apply_previous_cli' cannot be used while initializing")
+                msg = "'apply_previous_cli' cannot be used while initializing"
+                raise ValueError(msg)
             if not self._config.initial:
-                raise ValueError("'apply_previous_cli' enabled prior to an initialization")
+                msg = "'apply_previous_cli' enabled prior to an initialization"
+                raise ValueError(msg)
 
     def _roll_back(self) -> None:
         """In the case of a rollback, log the configuration state prior to roll back."""
         if self._skip_rollback:
             return
         message = "Configuration errors encountered, rolling back to previous configuration."
         self._messages.append(LogMessage(level=logging.WARNING, message=message))
@@ -152,15 +155,14 @@
                     entry.value.source = C.DEFAULT_CFG
             else:
                 message = f"'{entry.name}' cannot be reconfigured. (apply defaults)"
                 self._messages.append(LogMessage(level=logging.INFO, message=message))
 
     def _apply_settings_file(self) -> None:
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
         """Apply the settings file.
 
         :raises ValueError: If the settings file is empty
         """
         settings_filesystem_path = self._config.internals.settings_file_path
 
         if not isinstance(settings_filesystem_path, str):
@@ -175,15 +177,16 @@
             try:
                 config = yaml.load(fh, Loader=SafeLoader)
                 if config is None:
                     # In the case of ansible-navigator settings --sample > ansible-navigator.yml
                     # the file will be empty, but we shouldn't exit.
                     if self._params in (["settings", "--sample"], ["settings", "--gs"]):
                         return
-                    raise ValueError("Settings file cannot be empty.")
+                    msg = "Settings file cannot be empty."
+                    raise ValueError(msg)
             except (yaml.scanner.ScannerError, yaml.parser.ParserError, ValueError) as exc:
                 exit_msg = f"Settings file found {settings_filesystem_path}, but failed to load it."
                 self._exit_messages.append(ExitMessage(message=exit_msg))
                 exit_msg = f"  error was: '{' '.join(str(exc).splitlines())}'"
                 self._exit_messages.append(ExitMessage(message=exit_msg))
                 exit_msg = (
                     f"Try checking the settings file '{settings_filesystem_path}'"
@@ -238,15 +241,15 @@
                     message = f"'{entry.name}' cannot be reconfigured. (settings file)"
                     self._messages.append(LogMessage(level=logging.INFO, message=message))
             except TypeError as exc:
                 exit_msg = (
                     "Errors encountered when loading settings file:"
                     f" {settings_filesystem_path}"
                     f" while loading entry {entry.name}, attempted: {settings_file_path}."
-                    f"The resulting error was {str(exc)}"
+                    f"The resulting error was {exc!s}"
                 )
                 self._exit_messages.append(ExitMessage(message=exit_msg))
                 exit_msg = (
                     f"Try checking the settings file '{settings_filesystem_path}'"
                     "and ensure it is properly formatted"
                 )
                 self._exit_messages.append(
@@ -348,26 +351,24 @@
     def _check_choice(self, entry: SettingsEntry, value: bool | str):
         """Check the choice for a single settings entry.
 
         :param entry: The settings entry to check.
         :param value: The value to check.
         :return: True if the value is invalid and an error message was logged.
         """
-        if entry.cli_parameters and entry.choices:
-            if value not in entry.choices:
-                self._exit_messages.append(ExitMessage(message=entry.invalid_choice))
-                choices = [
-                    f"{entry.cli_parameters.short} {str(choice).lower()}"
-                    for choice in entry.choices
-                ]
-                exit_msg = f"Try again with {oxfordcomma(choices, 'or')}"
-                self._exit_messages.append(
-                    ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT),
-                )
-                return True
+        if entry.cli_parameters and entry.choices and value not in entry.choices:
+            self._exit_messages.append(ExitMessage(message=entry.invalid_choice))
+            choices = [
+                f"{entry.cli_parameters.short} {str(choice).lower()}" for choice in entry.choices
+            ]
+            exit_msg = f"Try again with {oxfordcomma(choices, 'or')}"
+            self._exit_messages.append(
+                ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT),
+            )
+            return True
         return False
 
     def _apply_previous_cli_to_current(self) -> None:
         """Apply eligible previous CLI values to current not set by the CLI."""
         # _apply_previous_cli_entries must be ALL or a list of entries
         if self._apply_previous_cli_entries is not C.ALL and not isinstance(
             self._apply_previous_cli_entries,
@@ -406,17 +407,19 @@
                 continue
 
             # skip if the previous entry not eligible for reapplication
             if previous_entry.apply_to_subsequent_cli not in [C.ALL, C.SAME_SUBCOMMAND]:
                 continue
 
             # skip if the same subcommand is required for reapplication
-            if current_entry.apply_to_subsequent_cli is C.SAME_SUBCOMMAND:
-                if current_subcommand != previous_subcommand:
-                    continue
+            if (
+                current_entry.apply_to_subsequent_cli is C.SAME_SUBCOMMAND
+                and current_subcommand != previous_subcommand
+            ):
+                continue
 
             # skip if the previous entry was not set by the CLI
             if previous_entry.value.source is not C.USER_CLI:
                 continue
 
             current_entry.value.current = previous_entry.value.current
             current_entry.value.source = C.PREVIOUS_CLI
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/definitions.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/definitions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 from pathlib import Path
 from typing import TYPE_CHECKING
 from typing import Any
 from typing import NewType
 from typing import TypeVar
 from typing import Union
 
-from ..utils.functions import abs_user_path
-from ..utils.functions import oxfordcomma
+from ansible_navigator.utils.functions import abs_user_path
+from ansible_navigator.utils.functions import oxfordcomma
 
 
 if TYPE_CHECKING:
     from .navigator_configuration import Internals
     from .navigator_post_processor import NavigatorPostProcessor
 
 
@@ -188,15 +188,16 @@
         """Generate an invalid choice message for this entry.
 
         :raises ValueError: If source is not set for that entry
         :returns: Constructed message
         """
         name = self.name.replace("_", "-")
         if self.value.source is Constants.NOT_SET:
-            raise ValueError(f"Current source not set for {self.name}")
+            msg = f"Current source not set for {self.name}"
+            raise ValueError(msg)
 
         choices = [str(choice).lower() for choice in self.choices]
         current = self.value.current
         if isinstance(current, list):
             choices_str = oxfordcomma(choices, "and/or")
             current = oxfordcomma(current, "and")
             prefix = f"The setting '{name}' must be one or more of"
@@ -218,18 +219,15 @@
 
     def settings_file_path(self, prefix: str) -> str:
         """Generate an effective settings file path for this entry.
 
         :param prefix: The prefix for the settings file path
         :returns: Settings file path
         """
-        if prefix:
-            prefix_str = f"{prefix}."
-        else:
-            prefix_str = prefix
+        prefix_str = f"{prefix}." if prefix else prefix
 
         if self.settings_file_path_override is not None:
             sfp = f"{prefix_str}{self.settings_file_path_override}"
         else:
             sfp = f"{prefix_str}{self.name}"
 
         return sfp.replace("_", "-")
@@ -326,24 +324,24 @@
     keep in mind that we support both runtimes.
     """
 
     # Overlay
     OVERLAY = "O"
 
     # Read Only
-    ro = "ro"  # pylint: disable=invalid-name
+    ro = "ro"
 
     # Read Write
-    rw = "rw"  # pylint: disable=invalid-name
+    rw = "rw"
 
     # Relabel as private
     Z = "Z"
 
     # Relabel as shared.
-    z = "z"  # pylint: disable=invalid-name
+    z = "z"
 
 
 V = TypeVar("V", bound="VolumeMount")
 
 
 class VolumeMountError(Exception):
     """Custom exception raised when building VolumeMounts."""
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/defs_presentable.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from dataclasses import dataclass
 from typing import ClassVar
 from typing import NewType
 from typing import TypeVar
 from typing import Union
 
-from ..content_defs import ContentBase
+from ansible_navigator.content_defs import ContentBase
+
 from .definitions import CliParameters
 from .definitions import Constants as C
 from .definitions import SettingsEntry
 from .navigator_configuration import Internals
 from .utils import create_settings_file_sample
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,21 +4,22 @@
 import logging
 import os
 
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 
-from ..utils.definitions import ExitMessage
-from ..utils.definitions import LogMessage
-from ..utils.functions import abs_user_path
-from ..utils.functions import generate_cache_path
-from ..utils.functions import oxfordcomma
-from ..utils.key_value_store import KeyValueStore
-from ..utils.packaged_data import ImageEntry
+from ansible_navigator.utils.definitions import ExitMessage
+from ansible_navigator.utils.definitions import LogMessage
+from ansible_navigator.utils.functions import abs_user_path
+from ansible_navigator.utils.functions import generate_cache_path
+from ansible_navigator.utils.functions import oxfordcomma
+from ansible_navigator.utils.key_value_store import KeyValueStore
+from ansible_navigator.utils.packaged_data import ImageEntry
+
 from .definitions import ApplicationConfiguration
 from .definitions import CliParameters
 from .definitions import Constants as C
 from .definitions import SettingsEntry
 from .definitions import SettingsEntryValue
 from .definitions import SubCommand
 from .navigator_post_processor import NavigatorPostProcessor
@@ -32,21 +33,25 @@
 
 PLUGIN_TYPES = (
     "become",
     "cache",
     "callback",
     "cliconf",
     "connection",
+    "filter",
     "httpapi",
     "inventory",
+    "keyword",
     "lookup",
     "module",
     "netconf",
+    "role",
     "shell",
     "strategy",
+    "test",
     "vars",
 )
 
 
 def generate_editor_command() -> str:
     """Generate a default for editor_command if EDITOR is set.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/navigator_post_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # pylint: disable=too-many-lines
 """Post processing of ansible-navigator configuration."""
 from __future__ import annotations
 
+import contextlib
 import importlib
 import logging
 import os
 import shlex
 import shutil
 import sys
 import zoneinfo
 
 from functools import partialmethod
 from itertools import chain
 from itertools import repeat
 from pathlib import Path
 from string import Formatter
 
-from ..utils.definitions import ExitMessage
-from ..utils.definitions import ExitPrefix
-from ..utils.definitions import LogMessage
-from ..utils.functions import abs_user_path
-from ..utils.functions import check_for_ansible
-from ..utils.functions import check_playbook_type
-from ..utils.functions import flatten_list
-from ..utils.functions import oxfordcomma
-from ..utils.functions import str2bool
-from ..utils.functions import to_list
+from ansible_navigator.utils.definitions import ExitMessage
+from ansible_navigator.utils.definitions import ExitPrefix
+from ansible_navigator.utils.definitions import LogMessage
+from ansible_navigator.utils.functions import abs_user_path
+from ansible_navigator.utils.functions import check_for_ansible
+from ansible_navigator.utils.functions import check_playbook_type
+from ansible_navigator.utils.functions import flatten_list
+from ansible_navigator.utils.functions import oxfordcomma
+from ansible_navigator.utils.functions import str2bool
+from ansible_navigator.utils.functions import to_list
+
 from .definitions import ApplicationConfiguration
 from .definitions import CliParameters
 from .definitions import Constants as C
 from .definitions import Mode
 from .definitions import ModeChangeRequest
 from .definitions import PaeChangeRequest
 from .definitions import SettingsEntry
@@ -81,38 +83,33 @@
         self._requested_pae: list[PaeChangeRequest] = []
 
     @staticmethod
     def _true_or_false(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process a boolean value.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
-        try:
+        with contextlib.suppress(ValueError):
             entry.value.current = str2bool(entry.value.current)
-        except ValueError:
-            # No error message here because the schema and/or choices will catch it
-            pass
 
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def ansible_runner_artifact_dir(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process ansible_runner_artifact_dir path.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -123,79 +120,75 @@
 
     @staticmethod
     @_post_processor
     def ansible_runner_rotate_artifacts_count(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process ansible_runner_rotate_artifacts_count.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
         if entry.value.current is not C.NOT_SET:
             try:
                 entry.value.current = int(entry.value.current)
             except ValueError as exc:
-                exit_msg = f"Value should be valid integer. Failed with error {str(exc)}"
+                exit_msg = f"Value should be valid integer. Failed with error {exc!s}"
                 exit_messages.append(ExitMessage(message=exit_msg))
         return messages, exit_messages
 
     # Post process ansible_runner_write_job_events.
     ansible_runner_write_job_events = _true_or_false
 
     @staticmethod
     @_post_processor
     def ansible_runner_timeout(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process ansible_runner_timeout.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
         if entry.value.current is not C.NOT_SET:
             try:
                 entry.value.current = int(entry.value.current)
             except ValueError as exc:
-                exit_msg = f"Value should be valid integer. Failed with error {str(exc)}"
+                exit_msg = f"Value should be valid integer. Failed with error {exc!s}"
                 exit_messages.append(ExitMessage(message=exit_msg))
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def collection_doc_cache_path(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process collection doc cache path.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
         entry.value.current = abs_user_path(entry.value.current)
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def cmdline(entry: SettingsEntry, config: ApplicationConfiguration) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process cmdline.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -206,15 +199,14 @@
 
     @staticmethod
     @_post_processor
     def container_engine(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process container_engine.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -250,17 +242,15 @@
         return self._true_or_false(entry, config)
 
     # Post process editor_console.
     editor_console = _true_or_false
 
     @_post_processor
     def execution_environment(self, entry: SettingsEntry, config) -> PostProcessorReturn:
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
         """Post process execution_environment.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages, exit_messages = self._true_or_false(entry, config)
@@ -335,15 +325,14 @@
 
     @staticmethod
     @_post_processor
     def execution_environment_image(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process execution_environment_image.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -360,16 +349,14 @@
     ) -> PostProcessorReturn:
         """Post process set_environment_variable.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :return: An instance of the standard post process return object
         """
-        # pylint: disable=unused-argument
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
 
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
         entry_name = entry.settings_file_path(prefix="")
         entry_source = entry.value.source
         volume_mounts: list[VolumeMount] = []
@@ -399,15 +386,15 @@
                             settings_entry=entry_name,
                             source=entry_source,
                         ),
                     )
                 except VolumeMountError as exc:
                     exit_msg = (
                         f"The following {entry_name} entry could not be parsed:"
-                        f" {mount_str} ({entry.value.source.value}). Errors were found: {str(exc)}"
+                        f" {mount_str} ({entry.value.source.value}). Errors were found: {exc!s}"
                     )
                     exit_messages.append(ExitMessage(message=exit_msg))
                     exit_messages.append(ExitMessage(message=hint, prefix=ExitPrefix.HINT))
 
         elif entry.value.source is C.USER_CFG:
             hint = (
                 "The value of execution-environment.volume-mounts should be a list"
@@ -429,15 +416,15 @@
                                 settings_entry=entry_name,
                                 source=entry_source,
                             ),
                         )
                     except (AttributeError, VolumeMountError) as exc:
                         exit_msg = (
                             f"The following {entry_name} entry could not be parsed:  {volume_mount}"
-                            f" ({entry_source.value}). Errors were found: {str(exc)}"
+                            f" ({entry_source.value}). Errors were found: {exc!s}"
                         )
                         exit_messages.append(ExitMessage(message=exit_msg))
                         exit_messages.append(ExitMessage(message=hint, prefix=ExitPrefix.HINT))
 
         # Get out fast if we had any errors
         if exit_messages:
             return messages, exit_messages
@@ -461,15 +448,14 @@
 
     @staticmethod
     @_post_processor
     def container_options(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process container_options.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -547,15 +533,14 @@
 
     @_post_processor
     def images_details(
         self,
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process execution_environment_image_details.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -623,15 +608,14 @@
 
     @staticmethod
     @_post_processor
     def inventory_column(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process inventory_columns.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -697,15 +681,14 @@
 
     # Post process log_append.
     log_append = _true_or_false
 
     @staticmethod
     @_post_processor
     def log_file(entry: SettingsEntry, config: ApplicationConfiguration) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process log_file.
 
         If the parent directory for the log file cannot be created and is writable.
         If not restore to default, this will allow the writing of log messages
         even if application initialization results in a sys.exit condition
 
         :param entry: The current settings entry
@@ -721,15 +704,15 @@
         except (OSError, FileNotFoundError) as exc:
             exit_msgs = [
                 (
                     f"Failed to create log file {entry.value.current}"
                     f" specified in '{entry.value.source.value}'"
                 ),
             ]
-            exit_msgs.append(f"The error was: {str(exc)}")
+            exit_msgs.append(f"The error was: {exc!s}")
             exit_messages.extend(ExitMessage(message=exit_msg) for exit_msg in exit_msgs)
             entry.value.current = entry.value.default
             entry.value.source = C.DEFAULT_CFG
             exit_msg = f"Log file set to default location: {entry.value.current}."
             exit_messages.append(ExitMessage(message=exit_msg))
             if entry.cli_parameters:
                 exit_msg = (
@@ -759,25 +742,25 @@
         if not config.internals.initializing:
             return messages, exit_messages
 
         for action_package_name in config.internals.action_packages:
             try:
                 action_package = importlib.import_module(action_package_name)
             except ImportError as exc:
-                message = f"Unable to load action package: '{action_package_name}': {str(exc)}"
+                message = f"Unable to load action package: '{action_package_name}': {exc!s}"
                 messages.append(LogMessage(level=logging.ERROR, message=message))
                 continue
             try:
                 if hasattr(action_package, "get"):
                     valid_pkg_name = subcommand_name.replace("-", "_")
                     subcommand_action = action_package.get(valid_pkg_name)  # type: ignore
                 break
             except (AttributeError, ModuleNotFoundError) as exc:
                 message = f"Unable to load subcommand '{subcommand_name}' from"
-                message += f" action package: '{action_package_name}': {str(exc)}"
+                message += f" action package: '{action_package_name}': {exc!s}"
                 messages.append(LogMessage(level=logging.DEBUG, message=message))
 
         if subcommand_action is None:
             exit_msg = f"Unable to find an action for '{subcommand_name}', tried: "
             exit_msg += oxfordcomma(config.internals.action_packages, "and")
             exit_messages.append(ExitMessage(message=exit_msg))
             return messages, exit_messages
@@ -817,15 +800,16 @@
                 )
                 messages.extend(
                     LogMessage(level=logging.INFO, message=msg) for msg in entry_mode_change_msgs
                 )
                 entry.value.current = auto_mode
                 entry.value.source = C.AUTO
         elif len(mode_set) > 1:
-            raise ValueError(f"Conflicting mode requests: {self._requested_mode}")
+            msg = f"Conflicting mode requests: {self._requested_mode}"
+            raise ValueError(msg)
         return messages, exit_messages
 
     # Post process osc4.
     osc4 = _true_or_false
 
     @_post_processor
     def plugin_name(
@@ -882,15 +866,14 @@
 
     @staticmethod
     @_post_processor
     def pass_environment_variable(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process pass_environment_variable.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -906,24 +889,28 @@
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
-        if config.app == "run" and entry.value.current is C.NOT_SET:
-            if config.entry("help_playbook").value.current is False:
-                exit_msg = "A playbook is required when using the run subcommand"
-                exit_messages.append(ExitMessage(message=exit_msg))
-                exit_msg = "Try again with 'run <playbook name>'"
-                exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
-                return messages, exit_messages
-        if check_playbook_type(entry.value.current) == "file":
-            if isinstance(entry.value.current, str):
-                entry.value.current = abs_user_path(entry.value.current)
+        if (
+            config.app == "run"
+            and entry.value.current is C.NOT_SET
+            and config.entry("help_playbook").value.current is False
+        ):
+            exit_msg = "A playbook is required when using the run subcommand"
+            exit_messages.append(ExitMessage(message=exit_msg))
+            exit_msg = "Try again with 'run <playbook name>'"
+            exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
+            return messages, exit_messages
+        if check_playbook_type(entry.value.current) == "file" and isinstance(
+            entry.value.current, str
+        ):
+            entry.value.current = abs_user_path(entry.value.current)
         return messages, exit_messages
 
     @_post_processor
     def playbook_artifact_enable(
         self,
         entry: SettingsEntry,
         config: ApplicationConfiguration,
@@ -931,15 +918,14 @@
         """Post process playbook_artifact_enable.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :raises ValueError: When more than 1 pae changes requests are present, shouldn't happen
         :returns: An instance of the standard post process return object
         """
-        # pylint: disable=unused-argument
         messages: list[LogMessage] = []
         exit_messages: list[ExitMessage] = []
 
         # Check if any other entry has requested a pae change different than current
         pae_set = {request.playbook_artifact_enable for request in self._requested_pae}
         if len(pae_set) == 1:
             requested = self._requested_pae[0]
@@ -950,19 +936,19 @@
                     f"Pae will be set to '{auto_pae}'",
                 )
                 messages.extend(
                     LogMessage(level=logging.INFO, message=msg) for msg in pae_change_msgs
                 )
                 entry.value.current = auto_pae
         elif len(pae_set) > 1:
-            raise ValueError(f"Conflicting pae requests: {self._requested_pae}")
-        try:
+            msg = f"Conflicting pae requests: {self._requested_pae}"
+            raise ValueError(msg)
+        with contextlib.suppress(ValueError):
             entry.value.current = str2bool(entry.value.current)
-        except ValueError:
-            pass
+
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def playbook_artifact_replay(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
@@ -981,32 +967,28 @@
             exit_msg = "Try again with 'replay <path to playbook artifact>'"
             exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
             return messages, exit_messages
 
         if isinstance(entry.value.current, str):
             entry.value.current = abs_user_path(entry.value.current)
 
-        if config.app == "replay":
-            if not os.path.isfile(entry.value.current):
-                exit_msg = (
-                    f"The specified playbook artifact could not be found: {entry.value.current}"
-                )
-                exit_messages.append(ExitMessage(message=exit_msg))
-                exit_msg = "Try again with 'replay <valid path to playbook artifact>'"
-                exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
-                return messages, exit_messages
+        if config.app == "replay" and not os.path.isfile(entry.value.current):
+            exit_msg = f"The specified playbook artifact could not be found: {entry.value.current}"
+            exit_messages.append(ExitMessage(message=exit_msg))
+            exit_msg = "Try again with 'replay <valid path to playbook artifact>'"
+            exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
+            return messages, exit_messages
         return messages, exit_messages
 
     @staticmethod
     @_post_processor
     def playbook_artifact_save_as(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process playbook_artifact_save_as.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -1032,15 +1014,14 @@
 
     @staticmethod
     @_post_processor
     def pull_arguments(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process ``pull_arguments``.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -1079,15 +1060,14 @@
 
     @staticmethod
     @_post_processor
     def set_environment_variable(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process set_environment_variable.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
@@ -1118,15 +1098,14 @@
 
     @staticmethod
     @_post_processor
     def time_zone(
         entry: SettingsEntry,
         config: ApplicationConfiguration,
     ) -> PostProcessorReturn:
-        # pylint: disable=unused-argument
         """Post process ``time_zone``.
 
         :param entry: The current settings entry
         :param config: The full application configuration
         :returns: An instance of the standard post process return object
         """
         messages: list[LogMessage] = []
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/parser.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,17 +89,19 @@
         :raises ValueError: if zero or more than one subcommand is found
         :returns: The subparsers action
         """
         subcommand_value = [
             entry for entry in self._config.entries if entry.subcommand_value is True
         ]
         if len(subcommand_value) == 0:
-            raise ValueError("No entry with subparser value defined")
+            msg = "No entry with subparser value defined"
+            raise ValueError(msg)
         if len(subcommand_value) > 1:
-            raise ValueError("Multiple entries with subparser value defined")
+            msg = "Multiple entries with subparser value defined"
+            raise ValueError(msg)
         entry = subcommand_value[0]
         return self.parser.add_subparsers(
             title=entry.short_description,
             dest=entry.name,
             metavar="{subcommand} --help",
         )
 
@@ -177,17 +179,18 @@
             return metavar
 
         if len(action.option_strings) == 1:
             return action.option_strings[0]
 
         if len(action.option_strings) == 2:
             # Account for a --1234 --long-option-name
-            return f"{action.option_strings[0].ljust(6)} {action.option_strings[1]}"
-
-        raise ValueError("Too many option strings")
+            msg = f"{action.option_strings[0].ljust(6)} {action.option_strings[1]}"
+            return msg
+        msg = "Too many option strings"
+        raise ValueError(msg)
 
     def _format_usage(self, usage, actions, groups, prefix):
         """Format the usage.
 
         :param usage: The usage
         :param actions: The actions
         :param groups: The groups
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/transform.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/transform.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 from __future__ import annotations
 
 import json
 import textwrap
 
 from typing import Any
 
-from ..utils.dict_merge import in_place_list_replace
-from ..utils.functions import shlex_join
-from ..utils.packaged_data import retrieve_content
+from ansible_navigator.utils.dict_merge import in_place_list_replace
+from ansible_navigator.utils.functions import shlex_join
+from ansible_navigator.utils.packaged_data import retrieve_content
+
 from .definitions import ApplicationConfiguration
 from .definitions import Constants
 from .definitions import SettingsEntry
 from .definitions import SettingsFileType
 from .defs_presentable import PresentableSettingsEntries
 from .defs_presentable import PresentableSettingsEntry
 from .utils import create_settings_file_sample
@@ -129,16 +130,16 @@
         elif entry.value.default is not Constants.NOT_SET:
             subschema[dot_parts[-1]]["default"] = entry.value.default
 
     if isinstance(settings.application_version, Constants):
         version = settings.application_version.value
     else:
         version = settings.application_version
-    # get only major.minor version info for the schema:
-    version = ".".join(version.split(".")[:2])
+    # get only major version info for the schema:
+    version = ".".join(version.split(".")[:1])
 
     partial_schema["version"] = version
     partial_schema["title"] = partial_schema["title"].format(version=version)
 
     return partial_schema
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/configuration_subsystem/utils.py` & `ansible-navigator-3.3.0/src/ansible_navigator/configuration_subsystem/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from configparser import ConfigParser
 from configparser import ParsingError
 from dataclasses import dataclass
 from dataclasses import field
 from pathlib import Path
 from typing import Any
 
-from ..command_runner import Command
-from ..command_runner import CommandRunner
-from ..utils.definitions import ExitMessage
-from ..utils.definitions import LogMessage
+from ansible_navigator.command_runner import Command
+from ansible_navigator.command_runner import CommandRunner
+from ansible_navigator.utils.definitions import ExitMessage
+from ansible_navigator.utils.definitions import LogMessage
+
 from .definitions import Constants
 from .definitions import SettingsFileType
 
 
 def create_settings_file_sample(
     settings_path: str,
     placeholder: bool | int | str | dict | list = "",
@@ -95,15 +96,14 @@
     If running without an EE, use ansible to get it.
     If running with an EE only look in the CWD.
     In the future user-specified volume mounts might be considered as locations.
 
     :param ee_enabled: Indicates if EE support is enabled
     :returns: The ansible.cfg contents
     """
-    # pylint: disable=too-many-return-statements
     response = ParseAnsibleCfgResponse(messages=[], exit_messages=[])
     response.config.path = Constants.NONE
     response.config.text = Constants.NONE
     response.config.contents = Constants.NONE
 
     if ee_enabled:
         msg = "EE support enabled: using current working directory for 'ansible.cfg'"
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/constants.py` & `ansible-navigator-3.3.0/src/ansible_navigator/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/content_defs.py` & `ansible-navigator-3.3.0/src/ansible_navigator/content_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,14 @@
 
 class SerializationFormat(Enum):
     """The serialization format."""
 
     YAML = "YAML"
     JSON = "JSON"
 
-    def repr(self) -> str:
-        """Return a string representation.
-
-        :return: A string
-        """
-        return self.value
-
 
 @dataclass
 class ContentBase(Generic[T]):
     r"""The base class for all content dataclasses presented in the UI.
 
     It should be noted, that while the return type is defined as ``T``
     for the serialization functions below, mypy will not catch in incorrect
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/ansible-navigator.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/ansible-navigator.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8571428560930608%*

 * *Differences: {"'properties'": "{'ansible-navigator': {'properties': {'ansible': {'properties': {'doc': "*

 * *                 "{'properties': {'plugin': {'properties': {'type': {'description': "*

 * *                 '"Specify the plugin type, \'become\', \'cache\', \'callback\', \'cliconf\', '*

 * *                 "'connection', 'filter', 'httpapi', 'inventory', 'keyword', 'lookup', 'module', "*

 * *                 '\'netconf\', \'role\', \'shell\', \'strategy\', \'test\' or \'vars\'", \'enum\': '*

 * *                 "{insert: [(5, 'filte […]*

```diff
@@ -47,28 +47,32 @@
                                     "properties": {
                                         "name": {
                                             "description": "Specify the plugin name",
                                             "type": "string"
                                         },
                                         "type": {
                                             "default": "module",
-                                            "description": "Specify the plugin type, 'become', 'cache', 'callback', 'cliconf', 'connection', 'httpapi', 'inventory', 'lookup', 'module', 'netconf', 'shell', 'strategy' or 'vars'",
+                                            "description": "Specify the plugin type, 'become', 'cache', 'callback', 'cliconf', 'connection', 'filter', 'httpapi', 'inventory', 'keyword', 'lookup', 'module', 'netconf', 'role', 'shell', 'strategy', 'test' or 'vars'",
                                             "enum": [
                                                 "become",
                                                 "cache",
                                                 "callback",
                                                 "cliconf",
                                                 "connection",
+                                                "filter",
                                                 "httpapi",
                                                 "inventory",
+                                                "keyword",
                                                 "lookup",
                                                 "module",
                                                 "netconf",
+                                                "role",
                                                 "shell",
                                                 "strategy",
+                                                "test",
                                                 "vars"
                                             ],
                                             "type": "string"
                                         }
                                     },
                                     "type": "object"
                                 }
@@ -516,11 +520,11 @@
                 }
             }
         }
     },
     "required": [
         "ansible-navigator"
     ],
-    "title": "ansible-navigator settings v3.1",
+    "title": "ansible-navigator settings v3",
     "type": "object",
-    "version": "3.1"
+    "version": "3"
 }
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/catalog_collections.py` & `ansible-navigator-3.3.0/src/ansible_navigator/data/catalog_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 
     def _catalog_roles(self, collection: dict[str, Any]) -> None:
         """Catalog the roles within a collection.
 
         :param collection: Details describing the collection
         """
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
 
         collection_name: str = collection["known_as"]
         collection["roles"] = []
         roles_directory = Path(collection["path"], "roles")
         if not roles_directory.is_dir():
             return
 
@@ -376,16 +375,16 @@
             else:
                 (doc, examples, returndocs, metadata) = get_docstring(
                     filename=str(plugin_path),
                     fragment_loader=fragment_loader,
                     collection_name=collection_name,
                 )
 
-        except Exception as exc:  # pylint: disable=broad-except
-            err_message = f"{type(exc).__name__} (get_docstring): {str(exc)}"
+        except Exception as exc:  # noqa: BLE001
+            err_message = f"{type(exc).__name__} (get_docstring): {exc!s}"
             completed_queue.put(("error", (checksum, plugin_path, err_message)))
             continue
 
         try:
             q_message = {
                 "plugin": {
                     "doc": doc,
@@ -393,15 +392,15 @@
                     "returndocs": returndocs,
                     "metadata": metadata,
                 },
                 "timestamp": datetime.utcnow().isoformat(),
             }
             completed_queue.put(("plugin", (checksum, json.dumps(q_message, default=str))))
         except JSONDecodeError as exc:
-            err_message = f"{type(exc).__name__} (json_decode_doc): {str(exc)}"
+            err_message = f"{type(exc).__name__} (json_decode_doc): {exc!s}"
             completed_queue.put(("error", (checksum, plugin_path, err_message)))
 
 
 def identify_missing(collections: dict, collection_cache: KeyValueStore) -> tuple[set, list, int]:
     """Identify plugins missing from the cache.
 
     :param collections: All plugins found across all collections
@@ -448,18 +447,15 @@
         dest="collection_cache_path",
         help="path to collection cache",
         required=True,
     )
     parsed_args = parser.parse_args()
 
     adjacent = vars(parsed_args).get("adjacent")
-    if adjacent:
-        directories = [adjacent] + parsed_args.dirs
-    else:
-        directories = parsed_args.dirs
+    directories = [adjacent] + parsed_args.dirs if adjacent else parsed_args.dirs
 
     directories.extend(reversed(sys.path))
 
     resolved = []
     for directory in directories:
         realpath = Path(directory).resolve()
         if realpath not in resolved:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/JSON.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html-derivative.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/html.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/html.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/log.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/log.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/markdown.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/shell-unix-bash.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.json.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.json.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.shell.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.shell.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/source.yaml.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/source.yaml.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.basic.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.basic.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.derivative.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.derivative.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.html.markdown.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.html.markdown.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/text.log.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/text.log.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/grammar/yaml.tmLanguage.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/help.md` & `ansible-navigator-3.3.0/src/ansible_navigator/data/help.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/image_introspect.py` & `ansible-navigator-3.3.0/src/ansible_navigator/data/image_introspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,23 +9,21 @@
 
 from queue import Queue
 from types import SimpleNamespace
 from typing import Any
 from typing import Callable
 
 
-# pylint: disable=broad-except
-
 PROCESSES = (multiprocessing.cpu_count() - 1) or 1
 
 
 class Command(SimpleNamespace):
     """Abstraction for a details about a shell command."""
 
-    id: str
+    id_: str
     command: str
     parse: Callable
     stdout: str = ""
     stderr: str = ""
     details: list | dict | str = ""
     errors: list = []
 
@@ -58,15 +56,15 @@
     while True:
         command = pending_queue.get()
         if command is None:
             break
         run_command(command)
         try:
             command.parse(command)
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             command.errors = command.errors + [str(exc)]
         completed_queue.put(command)
 
 
 class CommandRunner:
     """A command runner.
 
@@ -89,15 +87,15 @@
             command for command_class in command_classes for command in command_class.commands
         )
         results = []
         for command in all_commands:
             run_command(command)
             try:
                 command.parse(command)
-            except Exception as exc:
+            except Exception as exc:  # noqa: BLE001
                 command.errors = command.errors + [str(exc)]
             results.append(command)
         return results
 
     def run_multi_process(self, command_classes):
         """Run commands with multiple processes.
 
@@ -205,15 +203,15 @@
         """Define the ansible-galaxy command to list ansible collections.
 
         :returns: The defined command
         """
         command = "ansible-galaxy collection list"
         return [
             Command(
-                id="ansible_collections",
+                id_="ansible_collections",
                 command=command,
                 parse=self.parse,
             ),
         ]
 
     @staticmethod
     def parse(command: Command):
@@ -237,15 +235,15 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the ansible command to get the version.
 
         :returns: The defined command
         """
-        return [Command(id="ansible_version", command="ansible --version", parse=self.parse)]
+        return [Command(id_="ansible_version", command="ansible --version", parse=self.parse)]
 
     @staticmethod
     def parse(command: Command) -> None:
         """Parse the output of the ansible command.
 
         :param command: The result of running the command
         """
@@ -258,15 +256,15 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the command to collect os release information.
 
         :returns: The defined command
         """
-        return [Command(id="os_release", command="cat /etc/os-release", parse=self.parse)]
+        return [Command(id_="os_release", command="cat /etc/os-release", parse=self.parse)]
 
     def parse(self, command) -> None:
         """Parse the output of the cat command.
 
         :param command: The result of running the command
         """
         parsed = self.splitter(command.stdout.splitlines(), "=")
@@ -278,20 +276,20 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the pip command to list installed pip packages.
 
         :returns: The defined command
         """
-        pre = Command(id="pip_freeze", command="python3 -m pip freeze", parse=self.parse_freeze)
+        pre = Command(id_="pip_freeze", command="python3 -m pip freeze", parse=self.parse_freeze)
         run_command(pre)
         pre.parse(pre)
         pkgs = " ".join(pkg for pkg in pre.details[0])
         return [
-            Command(id="python_packages", command=f"python3 -m pip show {pkgs}", parse=self.parse),
+            Command(id_="python_packages", command=f"python3 -m pip show {pkgs}", parse=self.parse),
         ]
 
     def parse(self, command):
         """Parse the output of the pip command.
 
         :param command: The result of running the command
         """
@@ -319,15 +317,15 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the command to get the redhat release information.
 
         :returns: The defined command
         """
-        return [Command(id="redhat_release", command="cat /etc/redhat-release", parse=self.parse)]
+        return [Command(id_="redhat_release", command="cat /etc/redhat-release", parse=self.parse)]
 
     @staticmethod
     def parse(command):
         """Parse the output of the cat redhat release command.
 
         :param command: The result of running the command
         """
@@ -340,15 +338,15 @@
 
     @property
     def commands(self) -> list[Command]:
         """Define the command to list system packages.
 
         :returns: The defined command
         """
-        return [Command(id="system_packages", command="rpm -qai", parse=self.parse)]
+        return [Command(id_="system_packages", command="rpm -qai", parse=self.parse)]
 
     def parse(self, command):
         """Parse the output of the rpm command.
 
         :param command: The result of running the command
         """
         packages = []
@@ -408,15 +406,15 @@
         for result in results:
             result_as_dict = vars(result)
             result_as_dict.pop("parse")
             for key in list(result_as_dict.keys()):
                 if key not in ["details", "errors"]:
                     result_as_dict[f"__{key}"] = result_as_dict[key]
                     result_as_dict.pop(key)
-            response[result_as_dict["__id"]] = result_as_dict
-    except Exception as exc:
+            response[result_as_dict["__id_"]] = result_as_dict
+    except Exception as exc:  # noqa: BLE001
         response["errors"].append(str(exc))
     print(json.dumps(response))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/settings-sample.template.yml` & `ansible-navigator-3.3.0/src/ansible_navigator/data/settings-sample.template.yml`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/settings-schema.partial.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/settings-schema.partial.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/themes/dark_vs.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/themes/dark_vs.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/themes/terminal_colors.json` & `ansible-navigator-3.3.0/src/ansible_navigator/data/themes/terminal_colors.json`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/data/welcome.md` & `ansible-navigator-3.3.0/src/ansible_navigator/data/welcome.md`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/diagnostics.py` & `ansible-navigator-3.3.0/src/ansible_navigator/diagnostics.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 @dataclass
 class Diagnostics:
     """Data class for the diagnostics."""
 
     # pylint: disable=too-many-instance-attributes
 
-    __WARNING__: dict[str, JSONTypes]  # pylint: disable=invalid-name
+    __WARNING__: dict[str, JSONTypes]
     basics: dict[str, JSONTypes]
     container_engines: dict[str, JSONTypes]
     execution_environment: dict[str, JSONTypes]
     initialization: dict[str, JSONTypes]
     local_system: dict[str, JSONTypes]
     logs: dict[str, JSONTypes]
     python_packages: dict[str, JSONTypes]
@@ -111,15 +111,15 @@
 
     return decorator
 
 
 DIAGNOSTIC_FAILURES = 0
 
 
-class FailedCollection(Exception):
+class FailedCollectionError(Exception):
     """Exception for a failed collection."""
 
     def __init__(self, errors):
         """Initialize the exception.
 
         :param errors: The errors
         """
@@ -137,30 +137,30 @@
     def wrapper(*args, **kwargs):
         """Wrap and run the collector.
 
         :param args: The positional arguments
         :param kwargs: The keyword arguments
         :returns: The result of the function with elapsed or error information
         """
-        global DIAGNOSTIC_FAILURES  # pylint: disable=global-statement
+        global DIAGNOSTIC_FAILURES
         start = datetime.datetime.now()
         color = args[0].color
         collector = func.__collector__
         collector.start(color=color)
         try:
             result = func(*args, **kwargs)
             duration = (datetime.datetime.now() - start).total_seconds()
             collector.finish(color=color, duration=duration)
-        except FailedCollection as error:
+        except FailedCollectionError as error:
             # A collector exception, has data
             result = error.errors
             duration = (datetime.datetime.now() - start).total_seconds()
             collector.fail(color=color, duration=duration)
             DIAGNOSTIC_FAILURES += 1
-        except Exception as error:  # pylint: disable=broad-except
+        except Exception as error:  # noqa: BLE001
             # Any other exception, has no data
             result = {"error": str(error) + "\n" + traceback.format_exc()}
             duration = (datetime.datetime.now() - start).total_seconds()
             collector.fail(color=color, duration=duration)
             DIAGNOSTIC_FAILURES += 1
         result["duration"] = round(duration)
         return result
@@ -277,27 +277,27 @@
         return engines
 
     @diagnostic_runner
     @register(Collector(name="execution environment"))
     def _execution_environment(self) -> dict[str, JSONTypes]:
         """Add execution environment information.
 
-        :raises FailedCollection: If the collection process fails
+        :raises FailedCollectionError: If the collection process fails
         :returns: The execution environment information
         """
         if self._args.entry("container_engine").value.source is Constants.DEFAULT_CFG:
             return {"errors": "No container engine available or found"}
 
         details, errors, return_code = introspector.run(
             image_name=self._args.execution_environment_image,
             container_engine=self._args.container_engine,
         )
         details = {"details": details, "errors": errors, "return_code": return_code}
         if errors or not details:
-            raise FailedCollection(details)
+            raise FailedCollectionError(details)
         return details
 
     @diagnostic_runner
     @register(Collector(name="initialization"))
     def _initialization(self) -> dict[str, JSONTypes]:
         """Add initialization information.
 
@@ -337,22 +337,22 @@
         return {"found": bool(logs), "logs": logs}
 
     @diagnostic_runner
     @register(Collector(name="local system"))
     def _local_system(self) -> dict[str, JSONTypes]:
         """Add local system information.
 
-        :raises FailedCollection: If the collection process fails
+        :raises FailedCollectionError: If the collection process fails
         :returns: The local system information
         """
         results = introspect.main(serialize=False)
         if not results:
-            raise FailedCollection(results)
+            raise FailedCollectionError(results)
         if results.get("errors"):
-            raise FailedCollection(results["errors"])
+            raise FailedCollectionError(results["errors"])
         return {"details": results}
 
     @diagnostic_runner
     @register(Collector(name="python packages"))
     def _python_packages(self) -> dict[str, JSONTypes]:
         """Add python packages information.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/inspector.py` & `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/inspector.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Definitions for image inspection."""
 from __future__ import annotations
 
 import json
 import re
 
-from ..command_runner import Command
-from ..command_runner import CommandRunner
-from ..utils.functions import pascal_to_snake
+from ansible_navigator.command_runner import Command
+from ansible_navigator.command_runner import CommandRunner
+from ansible_navigator.utils.functions import pascal_to_snake
 
 
 class ImagesInspect:
     """Functionality for inspecting container images."""
 
     def __init__(self, container_engine, ids):
         """Initialize the container image inspector.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspect.py` & `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspect.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,23 +10,21 @@
 
 from queue import Queue
 from types import SimpleNamespace
 from typing import Callable
 from typing import Union
 
 
-# pylint: disable=broad-except
-
 JSONTypes = Union[bool, int, str, dict, list]
 
 
 class Command(SimpleNamespace):
     """Abstraction for a details about a shell command."""
 
-    id: str
+    id_: str
     command: str
     parse: Callable
     stdout: str = ""
     stderr: str = ""
     details: list | dict | str = ""
     errors: list = []
 
@@ -59,15 +57,15 @@
     while True:
         command = pending_queue.get()
         if command is None:
             break
         run_command(command)
         try:
             command.parse(command)
-        except Exception as exc:
+        except Exception as exc:  # noqa: BLE001
             command.errors = command.errors + [str(exc)]
         completed_queue.put(command)
 
 
 class CommandRunner:
     """A command runner.
 
@@ -397,15 +395,15 @@
             result_as_dict = vars(result)
             result_as_dict.pop("parse")
             for key in list(result_as_dict.keys()):
                 if key not in ["details", "errors"]:
                     result_as_dict[f"__{key}"] = result_as_dict[key]
                     result_as_dict.pop(key)
             response[result_as_dict["__id"]] = result_as_dict
-    except Exception as exc:
+    except Exception as exc:  # noqa: BLE001
         response["errors"].append(str(exc))
     if serialize:
         print(json.dumps(response))
         return None
     return response
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/introspector.py` & `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/introspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import inspect
 import json
 import logging
 import tempfile
 
 from pathlib import Path
 
-from ..runner import Command
+from ansible_navigator.runner import Command
+
 from . import introspect
 
 
 logger = logging.getLogger(__name__)
 
 
 def run(image_name: str, container_engine: str) -> tuple[dict, list[str], int]:
@@ -59,12 +60,12 @@
             _warnings, json_str = output.split("{", 1)
             json_str = "{" + json_str
         else:
             json_str = output
         parsed = json.loads(json_str)
     except (json.decoder.JSONDecodeError, ValueError) as exc:
         errors.append("Unable to extract introspection from stdout")
-        errors.append(f"error json loading output: '{str(exc)}'")
+        errors.append(f"error json loading output: '{exc!s}'")
         errors.append(output)
         return errors, {}
 
     return errors, parsed
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/image_manager/puller.py` & `ansible-navigator-3.3.0/src/ansible_navigator/image_manager/puller.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 
 import logging
 import shlex
 import subprocess
 
 from dataclasses import dataclass
 
-from ..configuration_subsystem import Constants
-from ..utils.definitions import ExitMessage
-from ..utils.definitions import ExitPrefix
-from ..utils.definitions import LogMessage
-from ..utils.functions import shlex_join
+from ansible_navigator.configuration_subsystem import Constants
+from ansible_navigator.utils.definitions import ExitMessage
+from ansible_navigator.utils.definitions import ExitPrefix
+from ansible_navigator.utils.definitions import LogMessage
+from ansible_navigator.utils.functions import shlex_join
 
 
 @dataclass(frozen=False)
 class ImageAssessment:
     """Data structure containing the image assessment.
 
     An ``ImageAssessment`` gets updated after instantiation
@@ -113,19 +113,19 @@
                 message = "Image inspection failed, image assumed to be corrupted or missing"
                 self._log_message(level=logging.WARNING, message=message)
                 self._log_message(level=logging.WARNING, message=f"stdout: {stdout}")
                 self._log_message(level=logging.WARNING, message=f"stderr: {stderr}")
 
     def _determine_pull(self):
         """Determine if a pull is required."""
-        if self._pull_policy == "missing" and self._image_present is False:
+        if self._pull_policy == "missing" and self._image_present is False:  # noqa: SIM114
             pull = True
-        elif self._pull_policy == "always":
+        elif self._pull_policy == "always":  # noqa: SIM114
             pull = True
-        elif self._pull_policy == "tag" and self._image_tag == "latest":
+        elif self._pull_policy == "tag" and self._image_tag == "latest":  # noqa: SIM114
             pull = True
         elif self._pull_policy == "tag" and self._image_present is False:
             pull = True
         else:
             pull = False
         self._pull_required = pull
         self._assessment.pull_required = pull
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/initialization.py` & `ansible-navigator-3.3.0/src/ansible_navigator/initialization.py`

 * *Files 6% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     path_errors = []
     doc_cache_dir = os.path.dirname(collection_doc_cache_path)
     try:
         os.makedirs(doc_cache_dir, exist_ok=True)
     except OSError as exc:
         path_errors.append(f"Problem making directory: {doc_cache_dir}")
-        path_errors.append(f"Error was: {str(exc)}")
+        path_errors.append(f"Error was: {exc!s}")
 
     if not os.access(os.path.dirname(collection_doc_cache_path), os.W_OK):
         path_errors.append("Directory not writable")
 
     if not os.access(os.path.dirname(collection_doc_cache_path), os.R_OK):
         path_errors.append("Directory not readable")
 
@@ -119,18 +119,15 @@
         exit_msgs.extend(path_errors)
         exit_messages.extend([ExitMessage(message=exit_msg) for exit_msg in exit_msgs])
         exit_msg = "Try again without '--cdcp' or try '--cdcp ~/collection_doc_cache.db"
         exit_messages.append(ExitMessage(message=exit_msg, prefix=ExitPrefix.HINT))
         return messages, exit_messages, None
 
     collection_cache: KeyValueStore = KeyValueStore(collection_doc_cache_path)
-    if "version" in collection_cache:
-        cache_version = collection_cache["version"]
-    else:
-        cache_version = None
+    cache_version = collection_cache["version"] if "version" in collection_cache else None
     message = f"Collection doc cache: 'current version' is '{cache_version}'"
     messages.append(LogMessage(level=logging.DEBUG, message=message))
     if cache_version is None or cache_version != VERSION_CDC:
         message = "Collection doc cache: version was empty or incorrect, rebuilding"
         messages.append(LogMessage(level=logging.INFO, message=message))
         collection_cache.close()
         os.remove(collection_doc_cache_path)
@@ -139,15 +136,14 @@
         cache_version = collection_cache["version"]
         message = f"Collection doc cache: 'current version' is '{cache_version}'"
         messages.append(LogMessage(level=logging.INFO, message=message))
     collection_cache.close()
     return messages, exit_messages, collection_cache
 
 
-# pylint: disable=inconsistent-return-statements
 def _diagnose(
     args: ApplicationConfiguration,
     exit_messages: list[ExitMessage],
     messages: list[LogMessage],
     should_diagnose: bool,
 ):
     """Direct to the diagnostic information writer or return.
@@ -160,17 +156,14 @@
     """
     if should_diagnose:
         DiagnosticsCollector(args=args, messages=messages, exit_messages=exit_messages).run()
     else:
         return messages, exit_messages
 
 
-# pylint: enable=inconsistent-return-statements
-
-
 def parse_and_update(
     params: list,
     args: ApplicationConfiguration,
     apply_previous_cli_entries: C | list[str] = C.NONE,
     attach_cdc=False,
 ) -> tuple[list[LogMessage], list[ExitMessage]]:
     """Build a configuration.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/logger.py` & `ansible-navigator-3.3.0/src/ansible_navigator/logger.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_config.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_doc.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_doc.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/ansible_inventory.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/base.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/command.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/command.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/command_async.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/command_async.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/runner/command_base.py` & `ansible-navigator-3.3.0/src/ansible_navigator/runner/command_base.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/steps.py` & `ansible-navigator-3.3.0/src/ansible_navigator/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,16 @@
         """Check some expected type against a value's type.
 
         :param value: Some value for comparison
         :param want: The desired type for value
         :raises ValueError: If value type doesn't match wanted type
         """
         if not isinstance(value, want):
-            raise ValueError(f"wanted {want}, got {type(value)}")
+            msg = f"wanted {want}, got {type(value)}"
+            raise ValueError(msg)
 
 
 class StepType(Enum):
     """Type of step, either menu or content."""
 
     MENU = "menu"
     CONTENT = "content"
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/LICENSE` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/compiler.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,16 @@
             elif rule.match is not None:
                 ret_regs.append(rule.match)
                 ret_rules.append(self._visit_rule(grammar, rule))
             elif rule.begin is not None:
                 ret_regs.append(rule.begin)
                 ret_rules.append(self._visit_rule(grammar, rule))
             else:
-                raise AssertionError(f"unreachable {rule}")
+                msg = f"unreachable {rule}"
+                raise AssertionError(msg)
         return ret_regs, tuple(ret_rules)
 
     def _captures_ref(self, grammar: Grammar, captures: Captures) -> Captures:
         return tuple((n, self._visit_rule(grammar, r)) for n, r in captures)
 
     def _compile_root(self, grammar: Grammar) -> PatternRule:
         regs, rules = self._patterns(grammar, grammar.patterns)
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/fchainmap.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/fchainmap.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/grammars.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/grammars.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/reg.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/reg.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/rules.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/rules.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,30 +224,32 @@
         compiler: Compiler,
         state: State,
         line: str,
         pos: int,
         first_line: bool,
         boundary: bool,
     ) -> tuple[State, int, bool, Regions] | None:
-        raise AssertionError(f"unreachable {self}")
+        msg = f"unreachable {self}"
+        raise AssertionError(msg)
 
 
 @uniquely_constructed
 class PatternRule(NamedTuple):
     name: tuple[str, ...]
     regset: _RegSet
     u_rules: tuple[_Rule, ...]
 
     def start(
         self,
         compiler: Compiler,
         match: Match[str],
         state: State,
     ) -> tuple[State, bool, Regions]:
-        raise AssertionError(f"unreachable {self}")
+        msg = f"unreachable {self}"
+        raise AssertionError(msg)
 
     def search(
         self,
         compiler: Compiler,
         state: State,
         line: str,
         pos: int,
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/state.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/state.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/tm_tokenize/tokenize.py` & `ansible-navigator-3.3.0/src/ansible_navigator/tm_tokenize/tokenize.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/__init__.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/colorize.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/colorize.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 import json
 import logging
 import re
 
 from importlib.abc import Traversable
 from itertools import chain
 
-from ..tm_tokenize.grammars import Grammars
-from ..tm_tokenize.region import Regions
-from ..tm_tokenize.tokenize import tokenize
+from ansible_navigator.tm_tokenize.grammars import Grammars
+from ansible_navigator.tm_tokenize.region import Regions
+from ansible_navigator.tm_tokenize.tokenize import tokenize
+
 from .curses_defs import CursesLine
 from .curses_defs import CursesLinePart
 from .curses_defs import CursesLines
 from .curses_defs import RgbTuple
 from .curses_defs import SimpleLinePart
 from .ui_constants import Color
 from .ui_constants import Decoration
@@ -129,15 +130,15 @@
             state = compiler.root_state
             lines = []
             for line_idx, line in enumerate(doc.splitlines()):
                 line += "\n"
                 first_line = line_idx == 0
                 try:
                     state, regions = tokenize(compiler, state, line, first_line)
-                except Exception as exc:  # pylint: disable=broad-except
+                except Exception as exc:  # noqa: BLE001
                     self._logger.critical(
                         (
                             "An unexpected error occurred within the tokenization"
                             " subsystem.  Please log an issue with the following:"
                         ),
                     )
                     self._logger.critical(
@@ -252,15 +253,14 @@
     return ansi
 
 
 def columns_and_colors(
     lines: list[tuple[Regions, str]],
     schema: ColorSchema,
 ) -> list[list[SimpleLinePart]]:
-    # pylint: disable=too-many-branches
     """Convert to colors and columns.
 
     :param lines: Lines of text and their regions
     :param schema: An instance of the ColorSchema
     :returns: Lines of text, each broken into sections
     """
     results: list[list[SimpleLinePart]] = []
@@ -341,17 +341,15 @@
         part = parts.pop(0)
         if part:
             match = color_regex.match(part)
             if match:
                 cap = match.groupdict()
                 one = cap["one"]
                 two = cap["two"]
-                if cap["fg_action"] == "39;":
-                    pass  # default color
-                elif one == "0" and two is None:
+                if cap["fg_action"] == "39;" or (one == "0" and two is None):
                     pass  # default color
                 elif cap["fg_action"] == "38;5;":
                     color = int(one)
                     if two:
                         style = CURSES_STYLES.get(int(two), None) or 0
                 elif not cap["fg_action"]:
                     ansi_16 = list(chain(range(30, 38), range(90, 98)))
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_defs.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_defs.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/curses_window.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/curses_window.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_button.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_button.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_checks.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_checks.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_curses_information.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_curses_information.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,14 @@
                 max((line_part for line_part in line), key=lambda lp: len(lp.string)).string
                 for line in self.information
             ),
             key=len,
         )
 
     def validate(self, response: str) -> None:
-        # pylint: disable=unused-argument
         """No validation required for information field.
 
         :param response: The response to validate
         """
         self.valid = True
 
     def conditional_validation(self, response: str) -> None:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_information.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_information.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         the largest 'prompt'.
 
         :returns: Max width information
         """
         return max(self.information)
 
     def validate(self, response: str) -> None:
-        # pylint: disable=unused-argument
         """No validation required for information field.
 
         :param response: Field data
         """
         self.valid = True
 
     def conditional_validation(self, response: str) -> None:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_option.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_option.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_radio.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_radio.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_text.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_text.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/field_working.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/field_working.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,14 @@
         is based on the largest 'prompt'.
 
         :returns: Max width information message
         """
         return max(self.messages)
 
     def validate(self, response: str) -> None:
-        # pylint: disable=unused-argument
         """No validation required for working field.
 
         :param response: Field response
         """
         self.valid = True
 
     def conditional_validation(self, response: str) -> None:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 from .validators import FormValidators
 
 
 @dataclass
 class Form:
     """Simple abstraction to hold the fields of the form and a convenience method to present it."""
 
-    type: FormType
+    type_: FormType
     cancelled: bool = False
     fields: list = field(default_factory=list)
     submitted: bool = False
     title: str = ""
     title_color: int = 0
 
     _dict: dict = field(default_factory=dict)
@@ -40,34 +40,34 @@
     def present(self, screen, ui_config):
         """Present the form the to user and return the results.
 
         :returns: Results from the form
         :param screen: A curses window
         :param ui_config: The current user interface configuration
         """
-        if self.type is FormType.FORM:
+        if self.type_ is FormType.FORM:
             self.fields.append(
                 FieldButton(
                     name="submit",
                     text="Submit",
                     validator=FormValidators.all_true,
                     color=10,
                 ),
             )
             self.fields.append(FieldButton(name="cancel", text="Cancel", color=9))
-        elif self.type is FormType.NOTIFICATION:
+        elif self.type_ is FormType.NOTIFICATION:
             self.fields.append(
                 FieldButton(
                     name="submit",
                     text=" Ok ",
                     validator=FormValidators.no_validation,
                     color=10,
                 ),
             )
-        elif self.type is FormType.WORKING:
+        elif self.type_ is FormType.WORKING:
             pass
 
         FormPresenter(form=self, screen=screen, ui_config=ui_config).present()
         try:
             self.submitted = next(field for field in self.fields if field.name == "submit").pressed
         except StopIteration:
             self.submitted = False
@@ -138,17 +138,17 @@
                 widths.extend(len(option.text) + self._input_start for option in form_field.options)
             if hasattr(form_field, "information"):
                 widths.append(max(len(info) for info in form_field.information))
             if hasattr(form_field, "messages"):
                 widths.append(max(len(msg) for msg in form_field.messages))
             widths.append(len(form_field.validator(hint=True)) + self._input_start)
 
-        if self._form.type is FormType.FORM:
+        if self._form.type_ is FormType.FORM:
             self._form_width = max(widths) + BUTTON_SPACE
-        elif self._form.type in (FormType.NOTIFICATION, FormType.WORKING):
+        elif self._form.type_ in (FormType.NOTIFICATION, FormType.WORKING):
             self._form_width = max(widths)
 
         height = 2  # title + horizontal line
         for form_field in self._form.fields:
             if isinstance(form_field, (FieldCursesInformation, FieldInformation)):
                 height += len(form_field.information)
             if isinstance(form_field, (FieldWorking)):
@@ -243,18 +243,15 @@
             window = curses.newwin(1, len(string), self._line_number, far_right + self._pad_left)
             window.keypad(True)
             form_field.win = window
             form_validity_state = [
                 f.valid for f in self._form.fields if not isinstance(f, FieldButton)
             ]
             form_field.conditional_validation(form_validity_state)
-            if form_field.disabled is True:
-                color = 8
-            else:
-                color = form_field.color
+            color = 8 if form_field.disabled is True else form_field.color
             line_part = CursesLinePart(far_right, string, color, 0)
             line_parts.append(line_part)
             far_right -= 1
         return CursesLine(tuple(line_parts))
 
     def _generate_error(self, form_field) -> CursesLine | None:
         """Generate the error for a field.
@@ -281,15 +278,15 @@
         )
         window.keypad(True)
         form_field.win = window
         lines = []
         for option in form_field.options:
             option_code = option.ansi_code(form_field)
             color = 8 if option.disabled else 0
-            text = f"{option_code} {str(option.text)}"
+            text = f"{option_code} {option.text!s}"
             line_part = CursesLinePart(self._input_start, text, color, 0)
             lines.append(CursesLine((line_part,)))
         return CursesLines(tuple(lines))
 
     def _generate_field_text(self, form_field) -> CursesLinePart:
         """Generate the text for a field.
 
@@ -341,18 +338,15 @@
     def _generate_prompt(self, form_field) -> list[CursesLinePart]:
         """Generate the prompt for a field.
 
         :param form_field: The field to generate the prompt for
         :returns: A list of CursesLinePart containing the prompt
         """
         prompt_start = self._prompt_end - len(form_field.full_prompt)
-        if form_field.valid is True:
-            color = 10
-        else:
-            color = 0
+        color = 10 if form_field.valid is True else 0
 
         cl_prompt = CursesLinePart(prompt_start, form_field.prompt, color, 0)
         cl_default = CursesLinePart(
             prompt_start + len(form_field.prompt),
             str(form_field.formatted_default),
             4,
             0,
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_button.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_button.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING
 
 from .curses_defs import CursesLinePart
 from .curses_window import CursesWindow
 
 
 if TYPE_CHECKING:
-    from .field_button import FieldButton  # pylint: disable=cyclic-import
+    from .field_button import FieldButton
 
 
 class FormHandlerButton(CursesWindow):
     """Handle form button."""
 
     def __init__(self, screen, ui_config):
         """Initialize the handler for a form button.
@@ -26,18 +26,15 @@
         super().__init__(ui_config=ui_config)
         self._form_field = None
         self._form_fields = None
         self._screen = screen
 
     def populate(self):
         """Populate the window with the button."""
-        if self._form_field.disabled is True:
-            color = 8
-        else:
-            color = self._form_field.color
+        color = 8 if self._form_field.disabled is True else self._form_field.color
 
         if self._ui_config.color is False:
             text = f"[{self._form_field.text.upper()}]"
         else:
             text = self._form_field.text
 
         clp_button = CursesLinePart(0, text, color, curses.A_STANDOUT)
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_information.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_information.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from curses import ascii as curses_ascii
 from typing import TYPE_CHECKING
 
 from .curses_window import CursesWindow
 
 
 if TYPE_CHECKING:
-    from .field_information import FieldInformation  # pylint: disable=cyclic-import
+    from .field_information import FieldInformation
 
 
 class FormHandlerInformation(CursesWindow):
     """Handle form button."""
 
     def __init__(self, screen, ui_config):
         """Initialize the handler for a informational notification.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_options.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 from typing import TYPE_CHECKING
 
 from .curses_defs import CursesLinePart
 from .curses_window import CursesWindow
 
 
 if TYPE_CHECKING:
-    from .field_checks import FieldChecks  # pylint: disable=cyclic-import
-    from .field_radio import FieldRadio  # pylint: disable=cyclic-import
+    from .field_checks import FieldChecks
+    from .field_radio import FieldRadio
 
 
 class FormHandlerOptions(CursesWindow):
     """Handle form checkbox field."""
 
     def __init__(self, screen, ui_config):
         """Initialize the handler for either form checkboxes or radio buttons.
@@ -35,18 +35,17 @@
         """
         for idx, option in enumerate(form_field.options):
             option_code = option.ansi_code(form_field)
             color = 8 if option.disabled else 0
             decoration = curses.A_STANDOUT if idx == active else 0
             clp_option_code = CursesLinePart(0, option_code, color, 0)
             if self._ui_config.color is False:
-                if idx == active:
-                    text = f"[{option.text.capitalize()}]"
-                else:
-                    text = option.text + "  "  # clear the []
+                text = (
+                    f"[{option.text.capitalize()}]" if idx == active else option.text + "  "
+                )  # clear the [], for else  # noqa: E501
             else:
                 text = option.text
             clp_text = CursesLinePart(len(option_code) + 1, text, color, decoration)
             self._add_line(self.win, idx, ([clp_option_code, clp_text]))
 
     def handle(self, idx, form_fields: list) -> tuple[FieldChecks | FieldRadio, int]:
         # pylint: disable=too-many-nested-blocks
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_text.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_text.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,16 +49,14 @@
         """Handle the input from the user.
 
         :param char: The character input from the user
         :returns: 0 if the window needs to be resized
                   1 if the window should be repainted
                   -1 if the window should be closed
         """
-        # pylint: disable=too-many-branches
-
         # in the case the term returns 127 instead of 263
         if char == curses_ascii.DEL:
             char = curses.KEY_BACKSPACE
 
         if char == curses.KEY_IC:
             self.insert_mode = not self.insert_mode
             ret = 1
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_handler_working.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_handler_working.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import TYPE_CHECKING
 
 from .curses_window import CursesWindow
 
 
 if TYPE_CHECKING:
-    from .field_working import FieldWorking  # pylint: disable=cyclic-import
+    from .field_working import FieldWorking
 
 
 class FormHandlerWorking(CursesWindow):
     """Handle form button."""
 
     def __init__(self, screen, ui_config):
         """Initialize the handler for a form working notification.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/form_utils.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/form_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import textwrap
 
 from functools import partial
 
 from ansible_navigator.utils.definitions import ExitMessage
 from ansible_navigator.utils.definitions import ExitMessages
 from ansible_navigator.utils.definitions import ExitPrefix
+from ansible_navigator.utils.functions import console_width
 
-from ..utils.functions import console_width
 from .colorize import ansi_to_curses
 from .curses_defs import CursesLines
 from .field_checks import FieldChecks
 from .field_curses_information import FieldCursesInformation
 from .field_information import FieldInformation
 from .field_option import FieldOption
 from .field_radio import FieldRadio
@@ -24,26 +24,25 @@
 from .form import Form
 from .form import FormType
 from .ui_constants import Color
 from .validators import FieldValidators
 
 
 def dict_to_form(form_data: dict) -> Form:
-    # pylint: disable=too-many-branches
     """Convert a python dict to a form.
 
     :param form_data: Form data
     :returns: Object containing fields from form
     """
     if form_data.get("type") == "notification":
-        form = Form(type=FormType.NOTIFICATION)
+        form = Form(type_=FormType.NOTIFICATION)
     elif form_data.get("type") == "working":
-        form = Form(type=FormType.WORKING)
+        form = Form(type_=FormType.WORKING)
     else:
-        form = Form(type=FormType.FORM)
+        form = Form(type_=FormType.FORM)
 
     form._dict = form_data  # pylint: disable=protected-access
     form.title = form_data["title"]
     form.title_color = form_data.get("title_color", 0)
 
     for field in form_data["fields"]:
         field_params = {"name": field["name"]}
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/menu_builder.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/menu_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import curses
 import enum
 import re
 
 from typing import Any
 from typing import Callable
 
-from ..content_defs import ContentBase
-from ..content_defs import ContentTypeSequence
+from ansible_navigator.content_defs import ContentBase
+from ansible_navigator.content_defs import ContentTypeSequence
+
 from .curses_defs import CursesLine
 from .curses_defs import CursesLinePart
 from .curses_defs import CursesLines
 from .ui_config import UIConfig
 from .utils import convert_percentage
 from .utils import distribute
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/sentinels.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/sentinels.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 import curses
 import logging
 import re
 
 from collections.abc import Mapping
 from collections.abc import Sequence
 from curses import ascii as curses_ascii
-from functools import lru_cache
+from functools import cache
 from math import ceil
 from math import floor
 from re import Match
 from re import Pattern
 from typing import Any
 from typing import Callable
 from typing import NamedTuple
 from typing import Protocol
 
-from ..content_defs import ContentFormat
-from ..content_defs import ContentType
-from ..content_defs import ContentTypeSequence
-from ..content_defs import ContentView
-from ..utils.functions import templar
-from ..utils.serialize import serialize
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.content_defs import ContentType
+from ansible_navigator.content_defs import ContentTypeSequence
+from ansible_navigator.content_defs import ContentView
+from ansible_navigator.utils.functions import templar
+from ansible_navigator.utils.serialize import serialize
+
 from .colorize import Colorize
 from .colorize import rgb_to_ansi
 from .curses_defs import CursesLine
 from .curses_defs import CursesLinePart
 from .curses_defs import CursesLines
 from .curses_defs import RgbTuple
 from .curses_defs import SimpleLinePart
@@ -283,19 +284,16 @@
 
     def _footer(self, key_dict: dict) -> CursesLine:
         """Build a footer from the key dict spread the columns out evenly.
 
         :param key_dict: the keys and their description
         :returns: The footer line
         """
-        column_widths = [len(f"{str(k)}: {str(v)}") for k, v in key_dict.items()]
-        if self._status:
-            status_width = self._progress_bar_width
-        else:
-            status_width = 0
+        column_widths = [len(f"{k!s}: {v!s}") for k, v in key_dict.items()]
+        status_width = self._progress_bar_width if self._status else 0
         gap = floor((self._screen_width - status_width - sum(column_widths)) / len(key_dict))
         adjusted_column_widths = [c + gap for c in column_widths]
         col_starts = [0]
         for idx, column_width in enumerate(adjusted_column_widths):
             col_starts.append(column_width + col_starts[idx])
         footer = []
         for idx, key in enumerate(key_dict):
@@ -409,17 +407,15 @@
         line_numbers: tuple[int, ...],
         heading: CursesLines | None,
         indent_heading: int,
         key_dict: dict,
         await_input: bool,
         count: int,
     ) -> str:
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
         """Show something on the screen.
 
         :param lines: The lines to show
         :param line_numbers: The number of lines to show
         :param heading: The headers to show
         :param indent_heading: The indentation of heading
         :param key_dict: any supplemental key to show
@@ -520,29 +516,30 @@
     ) -> tuple[str, Action] | tuple[None, None]:
         """Attempt to template & match the user input against the kegexes.
 
         :param entry: the user input
         :param current: the content on the screen
         :returns: The name of the action and the action to call or nothing if no match found
         """
-        if not entry.startswith("{{"):  # don't match pure template
-            if "{{" in entry and "}}" in entry:
-                if isinstance(current, Mapping):
-                    template_vars = current
-                    type_msgs = []
-                else:
-                    template_vars = {"this": current}
-                    type_msgs = ["Current content passed for templating is not a dictionary."]
-                    type_msgs.append("[HINT] Use 'this' to reference it (e.g. {{ this[0] }}")
-                errors, entry = templar(entry, template_vars)
-                if errors:
-                    msgs = ["Errors encountered while templating input"] + errors
-                    msgs.extend(type_msgs)
-                    self._show_form(warning_notification(msgs))
-                    return None, None
+        if (
+            not entry.startswith("{{") and "{{" in entry and "}}" in entry
+        ):  # don't match pure template
+            if isinstance(current, Mapping):
+                template_vars = current
+                type_msgs = []
+            else:
+                template_vars = {"this": current}
+                type_msgs = ["Current content passed for templating is not a dictionary."]
+                type_msgs.append("[HINT] Use 'this' to reference it (e.g. {{ this[0] }}")
+            errors, entry = templar(entry, template_vars)
+            if errors:
+                msgs = ["Errors encountered while templating input"] + errors
+                msgs.extend(type_msgs)
+                self._show_form(warning_notification(msgs))
+                return None, None
         for kegex in self._kegexes():
             match = kegex.kegex.match(entry)
             if match:
                 return kegex.name, Action(match=match, value=entry)
 
         msgs = [f"Could not find a match for ':{entry}'"]
         msgs.append("[Hint] Try ':help' for a list of available commands.")
@@ -674,30 +671,25 @@
 
     def _show_obj_from_list(
         self,
         objs: ContentTypeSequence,
         index: int,
         await_input: bool,
     ) -> Interaction:
-        # pylint: disable=too-many-branches
         # pylint: disable=too-many-locals
-        # pylint: disable=too-many-statements
         """Show an object on the display.
 
         :param objs: A list of one or more object
         :param index: The index associated with an object
         :param await_input: Should we wait for user input before returning
         :returns: interaction with the user
         """
         heading, lines = self._filter_and_serialize(objs[index])
         while True:
-            if heading is not None:
-                heading_len = len(heading)
-            else:
-                heading_len = 0
+            heading_len = len(heading) if heading is not None else 0
             footer_len = 1
 
             if self.scroll() == 0:
                 last_line_idx = min(
                     len(lines) - 1,
                     self._screen_height - heading_len - footer_len - 1,
                 )
@@ -705,18 +697,15 @@
                 last_line_idx = min(len(lines) - 1, self._scroll - 1)
 
             first_line_idx = max(
                 0,
                 last_line_idx - (self._screen_height - 1 - heading_len - footer_len),
             )
 
-            if len(objs) > 1:
-                key_dict = {"-": "previous", "+": "next", "[0-9]": "goto"}
-            else:
-                key_dict = {}
+            key_dict = {"-": "previous", "+": "next", "[0-9]": "goto"} if len(objs) > 1 else {}
 
             line_numbers = tuple(range(first_line_idx, last_line_idx + 1))
 
             entry = self._display(
                 lines=CursesLines(lines[first_line_idx : last_line_idx + 1]),
                 line_numbers=line_numbers,
                 heading=heading,
@@ -781,26 +770,21 @@
     def _obj_match_filter(self, obj: dict, columns: list) -> bool:
         """Check columns in a dictionary against a regex.
 
         :param obj: The dict to check
         :param columns: The dicts keys to check
         :returns: True if a match else False
         """
-        for key in columns:
-            if self._search_value(self.menu_filter(), obj.get(key)):
-                return True
-        return False
+        return any(self._search_value(self.menu_filter(), obj.get(key)) for key in columns)
 
     @staticmethod
-    @lru_cache(maxsize=None)
+    @cache
     def _search_value(regex: Pattern, value: str) -> Match | None:
         """Check a str against a regex.
 
-        lru_cache enabled because this is hit during resize
-
         :param regex: the compiled regex
         :param value: the string to check
         :returns: the match if made
         """
         return regex.search(str(value))
 
     def _get_heading_menu_items(
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_config.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_config.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/ui_constants.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/ui_constants.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/utils.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import functools
 import re
 
 from dataclasses import is_dataclass
 from math import floor
 from typing import Any
 
-from ..content_defs import ContentBase
+from ansible_navigator.content_defs import ContentBase
 
 
 def convert_percentage(
     content: dict[str, Any] | ContentBase,
     columns: list[str],
     progress_bar_width: int,
 ) -> None:
@@ -50,17 +50,16 @@
 @functools.cache
 def is_percent(string):
     """Determine if a string is a percentage.
 
     :param string: The string to check
     :returns: Boolean of comparison
     """
-    if string.endswith("%"):
-        if re.match(r"^\d{1,3}%$", string):
-            return True
+    if string.endswith("%") and re.match(r"^\d{1,3}%$", string):
+        return True
     return False
 
 
 def distribute(available, weights):
     """Distribute some available fairly across a list of numbers.
 
     :param available: the total
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/ui_framework/validators.py` & `ansible-navigator-3.3.0/src/ansible_navigator/ui_framework/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,18 +48,15 @@
 
         :param text: The text to validate
         :param hint: If True, return a hint message instead of a Validation
         :returns: A Validation or a hint message
         """
         if hint:
             return "Please provide a value (optional)"
-        if text:
-            value = "*" * randrange(15, 20)
-        else:
-            value = ""
+        value = "*" * randrange(15, 20) if text else ""
         return Validation(value=value, error_msg="")
 
     @staticmethod
     def none(
         text: FieldValidationStates | str = "",
         hint: bool = False,
     ) -> Validation | str:
@@ -83,26 +80,22 @@
         """
         if hint:
             return ""
         return Validation(value=text, error_msg="")
 
     @staticmethod
     def one_of(choices: list = [], text: str = "", hint: bool = False) -> Validation | str:
-        # pylint: disable=dangerous-default-value
         """Validate that some text is one of choices.
 
         :param choices: The list of choices
         :param text: The text to validate
         :param hint: If True, return a hint message instead of a Validation
         :returns: A Validation or a hint message
         """
-        if choices:
-            choices_str = f"{', '.join(choices[:-1])} or {choices[-1]}"
-        else:
-            choices_str = ""
+        choices_str = f"{', '.join(choices[:-1])} or {choices[-1]}" if choices else ""
         msg = f"Please enter {choices_str}"
         value = text
         if hint:
             return msg
         try:
             value = choices[[c.lower() for c in choices].index(text.lower())]
             msg = ""
@@ -124,15 +117,15 @@
         :param max_selected: The maximum number of choices that can be selected
         :param hint: If True, return a hint message instead of a Validation
         :returns: A Validation or a hint message
         :raises TypeError: If the types are not as expected
         """
         if min_selected == max_selected:
             word = "entry" if min_selected == 1 else "entries"
-            msg = f"Please select {str(min_selected)} {word}"
+            msg = f"Please select {min_selected!s} {word}"
         else:
             msg = f"Please select between {min_selected} and "
             word = str(max_selected) if max_selected != -1 else "all"
             msg += f"{word} entries"
 
         if hint:
             return msg
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/ansi.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/ansi.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/definitions.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/dict_merge.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/dict_merge.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,28 +30,29 @@
     :param left: Dict to be merged into
     :param right: Dict to be merged from
     :raises DictMergeError: If merging cannot be done
     :return: Merged dict
     """
     key = None
     try:
-        if left is None or isinstance(left, (str, int, float, bool)):
+        if left is None or isinstance(left, (str, int, float, bool)):  # noqa: SIM114
             # Border case for first run or if a is a primitive
             left = right
         elif isinstance(left, (tuple, list)):
             left = right
         elif isinstance(left, dict):
             if isinstance(right, dict):
                 for key in right:
                     if key in left:
                         left[key] = in_place_list_replace(left[key], right[key])
                     else:
                         left[key] = right[key]
             else:
-                raise DictMergeError(f"Cannot merge non-dict '{right}' into dict '{left}'")
+                msg = f"Cannot merge non-dict '{right}' into dict '{left}'"
+                raise DictMergeError(msg)
         else:
-            raise DictMergeError(f"Not implemented '{right}' into '{left}'")
+            msg = f"Not implemented '{right}' into '{left}'"
+            raise DictMergeError(msg)
     except TypeError as exc:
-        raise DictMergeError(
-            f"TypeError '{exc}' in key '{key}' when merging '{right}' into '{left}'",
-        ) from exc
+        msg = f"TypeError '{exc}' in key '{key}' when merging '{right}' into '{left}'"
+        raise DictMergeError(msg) from exc
     return left
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/dot_paths.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/dot_paths.py`

 * *Files 8% similar despite different names*

```diff
@@ -104,70 +104,74 @@
     :param behaviors: The merge behaviors
     :param content: The content of the settings file
     :param path: The path to the value
     :param value: The value to place
     :raises ValueError: If something can't be done
     :return: The updated content
     """
-    # pylint: disable=too-many-branches
     if (
         MergeBehaviors.DICT_DICT_REPLACE in behaviors
         and MergeBehaviors.DICT_DICT_UPDATE in behaviors
     ):
-        raise ValueError("Can't use both DICT_DICT_REPLACE and DICT_DICT_UPDATE behaviors")
+        msg = "Can't use both DICT_DICT_REPLACE and DICT_DICT_UPDATE behaviors"
+        raise ValueError(msg)
     if (
         MergeBehaviors.LIST_LIST_EXTEND in behaviors
         and MergeBehaviors.LIST_LIST_REPLACE in behaviors
     ):
-        raise ValueError("Can't use both LIST_LIST_EXTEND and LIST_LIST_REPLACE behaviors")
+        msg = "Can't use both LIST_LIST_EXTEND and LIST_LIST_REPLACE behaviors"
+        raise ValueError(msg)
 
     copied_content = copy.deepcopy(content)
     nested = copied_content
     if path in ("", None):
         if isinstance(value, dict):
             if MergeBehaviors.DICT_DICT_REPLACE in behaviors:
                 return value
             if MergeBehaviors.DICT_DICT_UPDATE in behaviors:
                 return {**nested, **value}
-        raise ValueError("Cannot place non dict at root of dict")
+        msg = "Cannot place non dict at root of dict"
+        raise ValueError(msg)
 
     for part in path.split("."):
         if part == path.rsplit(".", maxsplit=1)[-1]:
             if isinstance(nested.get(part), list):
                 if isinstance(value, list):
                     if MergeBehaviors.LIST_LIST_EXTEND in behaviors:
                         nested[part].extend(value)
                     elif MergeBehaviors.LIST_LIST_REPLACE in behaviors:
                         nested[part] = value
                     else:
-                        raise ValueError("No behavior specified for LIST_LIST")
+                        msg = "No behavior specified for LIST_LIST"
+                        raise ValueError(msg)
                 else:
                     if MergeBehaviors.LIST_APPEND in behaviors:
                         nested[part].append(value)
                     elif MergeBehaviors.LIST_REPLACE in behaviors:
                         nested[part] = value
                         continue
                     else:
-                        raise ValueError("No behavior specified for LIST_*")
+                        msg = "No behavior specified for LIST_*"
+                        raise ValueError(msg)
 
                 if MergeBehaviors.LIST_UNIQUE in behaviors:
                     nested[part] = list(dict.fromkeys(nested[part]))
                 if MergeBehaviors.LIST_SORT in behaviors:
                     nested[part].sort()
                 continue
 
-            if isinstance(nested.get(part), dict):
-                if isinstance(value, dict):
-                    if MergeBehaviors.DICT_DICT_UPDATE in behaviors:
-                        nested[part].update(value)
-                    elif MergeBehaviors.DICT_DICT_REPLACE in behaviors:
-                        nested[part] = value
-                    else:
-                        raise ValueError("No behavior specified for DICT_DICT")
-                    continue
+            if isinstance(nested.get(part), dict) and isinstance(value, dict):
+                if MergeBehaviors.DICT_DICT_UPDATE in behaviors:
+                    nested[part].update(value)
+                elif MergeBehaviors.DICT_DICT_REPLACE in behaviors:
+                    nested[part] = value
+                else:
+                    msg = "No behavior specified for DICT_DICT"
+                    raise ValueError(msg)
+                continue
 
             nested[part] = value
         elif part not in nested:
             nested[part] = {}
         nested = nested[part]
     return copied_content
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/functions.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def oxfordcomma(listed, condition):
     """Format a list into a sentence.
 
     :param listed: List of string entries to modify
     :param condition: String to splice into string, usually 'and'
     :returns: Modified string
     """
-    listed = [f"'{str(entry)}'" for entry in listed]
+    listed = [f"'{entry!s}'" for entry in listed]
     if len(listed) == 0:
         return ""
     if len(listed) == 1:
         return listed[0]
     if len(listed) == 2:
         return f"{listed[0]} {condition} {listed[1]}"
     return f"{', '.join(listed[:-1])} {condition} {listed[-1]}"
@@ -438,15 +438,15 @@
 
     env = Environment(autoescape=True, undefined=StrictUndefined)
     try:
         template: Any = env.from_string(string)
         result = template.render(template_vars)
     except (ValueError, TemplateError) as exc:
         errors.append(f"Error while templating string: '{string}'")
-        errors.append(f"The error was: {str(exc)}")
+        errors.append(f"The error was: {exc!s}")
         for error in errors:
             logger.error(error)
         return errors, string
 
     # We may have gotten the __repr__ of a python object
     # so let's try and turn it back
     try:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/json_schema.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/key_value_store.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/key_value_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         return self._path
 
     def close(self) -> None:
         """Close the connection to the database."""
         self.conn.commit()
         self.conn.close()
 
-    def open(self) -> sqlite3.Connection:
+    def open_(self) -> sqlite3.Connection:
         """Establish the connection to the database.
 
         :returns: A connection to the database
         """
         self.conn = sqlite3.connect(self.path)
         return self.conn
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/packaged_data.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/packaged_data.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/print.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/print.py`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/serialize.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from pathlib import Path
 from typing import IO
 from typing import Any
 from typing import NamedTuple
 
 import yaml
 
-from ..content_defs import ContentBase
-from ..content_defs import ContentFormat
-from ..content_defs import ContentType
-from ..content_defs import ContentView
-from ..content_defs import SerializationFormat
+from ansible_navigator.content_defs import ContentBase
+from ansible_navigator.content_defs import ContentFormat
+from ansible_navigator.content_defs import ContentType
+from ansible_navigator.content_defs import ContentView
+from ansible_navigator.content_defs import SerializationFormat
 
 
 logger = logging.getLogger(__name__)
 
 # pylint: disable=unused-import
 try:
     from yaml import CSafeDumper as SafeDumper
@@ -59,15 +59,16 @@
         content_view=content_view,
         serialization_format=serialization_format,
     )
     if serialization_format == SerializationFormat.YAML:
         return _yaml_dumps(dumpable=dumpable)
     if serialization_format == SerializationFormat.JSON:
         return _json_dumps(dumpable=dumpable)
-    raise ValueError("Unknown serialization format")
+    msg = "Unknown serialization format"
+    raise ValueError(msg)
 
 
 def serialize_write_file(
     content: ContentType,
     content_view: ContentView,
     file_mode: str,
     file: Path,
@@ -90,15 +91,16 @@
     with file.open(mode=file_mode, encoding="utf-8") as file_handle:
         if serialization_format == SerializationFormat.JSON:
             _json_dump(dumpable=dumpable, file_handle=file_handle)
             return
         if serialization_format == SerializationFormat.YAML:
             _yaml_dump(dumpable=dumpable, file_handle=file_handle)
             return
-    raise ValueError("Unknown serialization format")
+    msg = "Unknown serialization format"
+    raise ValueError(msg)
 
 
 def serialize_write_temp_file(
     content: ContentType,
     content_view: ContentView,
     content_format: ContentFormat,
 ) -> Path:
@@ -127,16 +129,16 @@
             _json_dump(dumpable=dumpable, file_handle=file_like)
             return Path(file_like.name)
         if content_format == ContentFormat.YAML:
             _yaml_dump(dumpable=dumpable, file_handle=file_like)
             return Path(file_like.name)
         _text_dump(dumpable=str(dumpable), file_handle=file_like)
         return Path(file_like.name)
-
-    raise ValueError("Unknown serialization format")
+    msg = "Unknown serialization format"
+    raise ValueError(msg)
 
 
 SERIALIZATION_FAILURE_MSG = (
     "The requested content could not be converted to {serialization_format}.\n"
     "The content was {content}\n"
     "Please log an issue for this, it should not have happened\n"
     "Error details: {exception_str}\n"
@@ -335,19 +337,15 @@
     .. note::
 
        Inspired by http://stackoverflow.com/a/15423007/115478.
 
     :param value: The value to check
     :returns: A boolean indicating if the string is multiline
     """
-    for character in "\u000a\u000d\u001c\u001d\u001e\u0085\u2028\u2029":
-        if character in value:
-            return True
-
-    return False
+    return any(character in value for character in "\n\r\x1c\x1d\x1e\x85\u2028\u2029")
 
 
 def opener(path: str, flags: int, mode: int) -> int:
     """Open a file with the given path and flags.
 
     :param path: The path of the file to open.
     :param flags: The flags to use when opening the file.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/definitions.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/definitions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 """Common definitions for a version migration."""
 from __future__ import annotations
 
+import contextlib
+
 from enum import Enum
 from pathlib import Path
 from typing import Callable
 from typing import Generic
 from typing import TypeVar
 
-from ..ansi import COLOR
-from ..ansi import changed
-from ..ansi import failed
-from ..ansi import subtle
-from ..ansi import working
+from ansible_navigator.utils.ansi import COLOR
+from ansible_navigator.utils.ansi import changed
+from ansible_navigator.utils.ansi import failed
+from ansible_navigator.utils.ansi import subtle
+from ansible_navigator.utils.ansi import working
 
 
 class MigrationType(Enum):
     """Enum for the type of migration."""
 
     SETTINGS_FILE = "settings"
     """Migration of the settings file."""
@@ -143,34 +145,32 @@
     def run_step(self, step: MigrationStep, *args, **kwargs) -> None:
         """Run the migration step.
 
         :param step: The migration step to run
         :param args: The positional arguments
         :param kwargs: The keyword arguments
         """
-        # pylint: disable=broad-except
         if not isinstance(step.function_name, str):
             return
         function = getattr(self, step.function_name)
         if self.check:
             try:
                 step.needed = function(*args, **kwargs)
-            except Exception:
+            except Exception:  # noqa: BLE001
                 step.needed = False
             return
 
         if not step.needed:
             step.print_not_needed()
             return
 
         step.print_start()
-        try:
+        with contextlib.suppress(Exception):
             step.needed = function(*args, **kwargs)
-        except Exception:
-            pass
+
         if step.needed:
             step.print_failed()
         else:
             step.print_updated()
         return
 
     def run_steps(self, *args, **kwargs) -> None:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/migrate.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/migrate.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """The ability to perform migrations."""
 
 from __future__ import annotations
 
 from pathlib import Path
 
-from ..ansi import COLOR
-from ..ansi import IS_TTY
-from ..ansi import blank_line
-from ..ansi import info
-from ..ansi import prompt_enter
-from ..ansi import prompt_yn
-from ..ansi import success
-from ..ansi import warning
+from ansible_navigator.utils.ansi import COLOR
+from ansible_navigator.utils.ansi import IS_TTY
+from ansible_navigator.utils.ansi import blank_line
+from ansible_navigator.utils.ansi import info
+from ansible_navigator.utils.ansi import prompt_enter
+from ansible_navigator.utils.ansi import prompt_yn
+from ansible_navigator.utils.ansi import success
+from ansible_navigator.utils.ansi import warning
+
 from .definitions import MigrationType
 from .definitions import migrations
 
 
 # isort: off
 # pylint: disable=unused-import
 # Migrations will run in the order they are imported
@@ -36,15 +37,14 @@
 
 def run_migrations(settings_file_str: str, migration_type: MigrationType) -> None:
     """Run migrations of a specific type.
 
     :param settings_file_str: Path to the settings file
     :param migration_type: Type of migration
     """
-    # pylint: disable=too-many-branches
     migrations_to_run = [
         migration()
         for migration in migrations
         if getattr(migration, "migration_type", None) == migration_type
     ]
 
     for migration in migrations_to_run:
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py` & `ansible-navigator-3.3.0/src/ansible_navigator/utils/version_migration/v1_v2_settings_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """The v1 to v2 settings file migration."""
 
 from __future__ import annotations
 
-from ..dot_paths import MergeBehaviors
-from ..dot_paths import check_path
-from ..dot_paths import get_with_path
-from ..dot_paths import move_to_path
-from ..dot_paths import place_at_path
+from ansible_navigator.utils.dot_paths import MergeBehaviors
+from ansible_navigator.utils.dot_paths import check_path
+from ansible_navigator.utils.dot_paths import get_with_path
+from ansible_navigator.utils.dot_paths import move_to_path
+from ansible_navigator.utils.dot_paths import place_at_path
+
 from .definitions import MigrationStep
 from .definitions import MigrationType
 from .settings_file import SettingsFile
 
 
 class V1V2SettingsFile(SettingsFile):
     """The v1 to v2 settings file migration.
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator.egg-info/PKG-INFO` & `ansible-navigator-3.3.0/src/ansible_navigator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-navigator
-Version: 3.2.0
+Version: 3.3.0
 Summary: A text-based user interface (TUI) for the Red Hat Ansible Automation Platform
 Author-email: "Bradley A. Thornton" <bthornto@redhat.com>
 Maintainer-email: Ansible by Red Hat <info@ansible.com>
 License: Apache
 Project-URL: homepage, https://github.com/ansible/ansible-navigator
 Project-URL: documentation, https://ansible-navigator.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/ansible/ansible-navigator
```

### Comparing `ansible-navigator-3.2.0/src/ansible_navigator.egg-info/SOURCES.txt` & `ansible-navigator-3.3.0/src/ansible_navigator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-navigator-3.2.0/tox.ini` & `ansible-navigator-3.3.0/tox.ini`

 * *Files identical despite different names*

