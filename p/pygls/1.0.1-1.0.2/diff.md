# Comparing `tmp/pygls-1.0.1.tar.gz` & `tmp/pygls-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygls-1.0.1.tar", last modified: Thu Feb 16 12:12:38 2023, max compression
+gzip compressed data, was "pygls-1.0.2.tar", last modified: Tue May 16 13:19:30 2023, max compression
```

## Comparing `pygls-1.0.1.tar` & `pygls-1.0.2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.958593 pygls-1.0.1/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      168 2022-05-26 11:42:47.000000 pygls-1.0.1/.editorconfig
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      679 2022-05-26 11:42:47.000000 pygls-1.0.1/.gitattributes
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.926592 pygls-1.0.1/.github/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)       70 2022-08-01 12:02:09.000000 pygls-1.0.1/.github/FUNDING.yml
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.926592 pygls-1.0.1/.github/workflows/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2487 2023-01-28 20:44:49.000000 pygls-1.0.1/.github/workflows/ci.yml
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2025 2023-01-28 20:44:49.000000 pygls-1.0.1/.github/workflows/json-extension.yml
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     1308 2023-01-28 20:45:05.000000 pygls-1.0.1/.gitignore
--rw-rw-r--   0 tombh     (1000) tombh     (1000)    12302 2023-02-16 12:12:00.000000 pygls-1.0.1/CHANGELOG.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3293 2022-05-26 11:42:47.000000 pygls-1.0.1/CODE_OF_CONDUCT.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3414 2022-05-26 11:42:47.000000 pygls-1.0.1/CONTRIBUTING.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      905 2022-12-01 20:59:24.000000 pygls-1.0.1/CONTRIBUTORS.md
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     1517 2023-02-15 02:36:59.000000 pygls-1.0.1/HISTORY.md
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     4833 2023-01-27 19:25:21.000000 pygls-1.0.1/Implementations.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)    11367 2022-05-26 11:42:47.000000 pygls-1.0.1/LICENSE.txt
--rw-rwxr--   0 tombh     (1000) tombh     (1000)       36 2022-05-26 11:42:47.000000 pygls-1.0.1/MANIFEST.in
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     4661 2023-02-16 12:12:38.958593 pygls-1.0.1/PKG-INFO
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      959 2022-05-26 11:42:47.000000 pygls-1.0.1/PULL_REQUEST_TEMPLATE.md
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     3526 2023-01-28 20:44:49.000000 pygls-1.0.1/README.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     1261 2022-12-14 12:57:21.000000 pygls-1.0.1/RELEASING.md
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3034 2022-05-26 11:42:47.000000 pygls-1.0.1/ThirdPartyNotices.txt
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.927592 pygls-1.0.1/docs/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      584 2022-05-26 11:42:47.000000 pygls-1.0.1/docs/Makefile
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.928592 pygls-1.0.1/docs/assets/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     3076 2023-01-28 20:44:49.000000 pygls-1.0.1/docs/assets/hello-world-completion.png
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      756 2022-05-26 11:42:47.000000 pygls-1.0.1/docs/make.bat
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.928592 pygls-1.0.1/docs/source/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5086 2022-12-14 12:57:21.000000 pygls-1.0.1/docs/source/conf.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     1305 2022-12-14 12:57:21.000000 pygls-1.0.1/docs/source/index.rst
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.930592 pygls-1.0.1/docs/source/pages/
--rw-r--r--   0 tombh     (1000) tombh     (1000)    16311 2023-01-27 19:25:21.000000 pygls-1.0.1/docs/source/pages/advanced_usage.rst
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2748 2023-01-27 19:25:21.000000 pygls-1.0.1/docs/source/pages/getting_started.rst
--rw-rwxr--   0 tombh     (1000) tombh     (1000)    13249 2022-12-14 12:57:21.000000 pygls-1.0.1/docs/source/pages/migrating-to-v1.rst
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     1012 2022-05-26 11:42:47.000000 pygls-1.0.1/docs/source/pages/testing.rst
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     7018 2022-12-14 12:57:21.000000 pygls-1.0.1/docs/source/pages/tutorial.rst
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.918592 pygls-1.0.1/examples/
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.935592 pygls-1.0.1/examples/fountain-vscode-extension/
--rw-r--r--   0 tombh     (1000) tombh     (1000)       16 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/.gitignore
--rw-r--r--   0 tombh     (1000) tombh     (1000)     3834 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/README.md
--rw-r--r--   0 tombh     (1000) tombh     (1000)   408759 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/demo.png
--rw-r--r--   0 tombh     (1000) tombh     (1000)      487 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/fountain-language-configuration.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)   112066 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/package-lock.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1171 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/package.json
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.935592 pygls-1.0.1/examples/fountain-vscode-extension/src/
--rw-r--r--   0 tombh     (1000) tombh     (1000)      850 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/src/client.ts
--rw-r--r--   0 tombh     (1000) tombh     (1000)      814 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/src/server.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1679 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/src/server.ts
--rw-r--r--   0 tombh     (1000) tombh     (1000)      268 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/tsconfig.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)   108088 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/tunnel.png
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1332 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/fountain-vscode-extension/webpack.config.js
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.936592 pygls-1.0.1/examples/hello-world/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2755 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/hello-world/README.md
--rw-r--r--   0 tombh     (1000) tombh     (1000)      711 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/hello-world/main.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.938592 pygls-1.0.1/examples/json-vscode-extension/
--rw-r--r--   0 tombh     (1000) tombh     (1000)      245 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/.eslintrc.yml
--rw-r--r--   0 tombh     (1000) tombh     (1000)       70 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/.gitignore
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.938592 pygls-1.0.1/examples/json-vscode-extension/.vscode/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1619 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/.vscode/launch.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)      695 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/.vscode/tasks.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)      120 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/.vscodeignore
--rw-r--r--   0 tombh     (1000) tombh     (1000)    11367 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/LICENSE.txt
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1175 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/README.md
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.918592 pygls-1.0.1/examples/json-vscode-extension/client/
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.938592 pygls-1.0.1/examples/json-vscode-extension/client/src/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     3495 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/client/src/extension.ts
--rw-r--r--   0 tombh     (1000) tombh     (1000)    98529 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/package-lock.json
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2060 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/package.json
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.939592 pygls-1.0.1/examples/json-vscode-extension/server/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/__init__.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     2203 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/__main__.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)    11204 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/server.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.939592 pygls-1.0.1/examples/json-vscode-extension/server/tests/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/tests/__init__.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.940592 pygls-1.0.1/examples/json-vscode-extension/server/tests/unit/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/tests/unit/__init__.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     6061 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/server/tests/unit/test_features.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)      275 2023-01-28 20:44:49.000000 pygls-1.0.1/examples/json-vscode-extension/tsconfig.json
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.943592 pygls-1.0.1/pygls/
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1511 2023-02-16 12:12:00.000000 pygls-1.0.1/pygls/__init__.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)    14497 2022-12-14 12:57:21.000000 pygls-1.0.1/pygls/capabilities.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     1470 2022-07-06 23:06:23.000000 pygls-1.0.1/pygls/constants.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6247 2022-12-14 12:57:21.000000 pygls-1.0.1/pygls/exceptions.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     8263 2022-12-14 12:57:21.000000 pygls-1.0.1/pygls/feature_manager.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.945592 pygls-1.0.1/pygls/lsp/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5090 2022-12-14 12:57:21.000000 pygls-1.0.1/pygls/lsp/__init__.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2852 2022-12-14 12:57:21.000000 pygls-1.0.1/pygls/progress.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)    37243 2023-01-30 00:57:57.000000 pygls-1.0.1/pygls/protocol.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)       65 2022-05-26 11:42:47.000000 pygls-1.0.1/pygls/py.typed
--rw-r--r--   0 tombh     (1000) tombh     (1000)    19431 2023-01-30 00:57:57.000000 pygls-1.0.1/pygls/server.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5323 2022-07-06 23:06:23.000000 pygls-1.0.1/pygls/uris.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)    14925 2023-01-27 19:30:59.000000 pygls-1.0.1/pygls/workspace.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.944592 pygls-1.0.1/pygls.egg-info/
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     4661 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/PKG-INFO
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     4298 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/SOURCES.txt
--rw-rw-r--   0 tombh     (1000) tombh     (1000)        1 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/dependency_links.txt
--rw-rw-r--   0 tombh     (1000) tombh     (1000)        1 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/not-zip-safe
--rw-rw-r--   0 tombh     (1000) tombh     (1000)      205 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/requires.txt
--rw-rw-r--   0 tombh     (1000) tombh     (1000)        6 2023-02-16 12:12:38.000000 pygls-1.0.1/pygls.egg-info/top_level.txt
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      199 2022-07-07 16:59:19.000000 pygls-1.0.1/pyproject.toml
--rw-rw-r--   0 tombh     (1000) tombh     (1000)     1694 2023-02-16 12:12:38.959592 pygls-1.0.1/setup.cfg
--rwxrwxr-x   0 tombh     (1000) tombh     (1000)       93 2022-07-04 20:17:59.000000 pygls-1.0.1/setup.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.949592 pygls-1.0.1/tests/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     1628 2022-07-09 01:05:07.000000 pygls-1.0.1/tests/__init__.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)      932 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/_init_server_stall_fix_hack.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2508 2022-07-09 01:05:07.000000 pygls-1.0.1/tests/conftest.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5819 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/ls_setup.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.956592 pygls-1.0.1/tests/lsp/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)        0 2022-05-26 11:42:47.000000 pygls-1.0.1/tests/lsp/__init__.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.957593 pygls-1.0.1/tests/lsp/semantic_tokens/
--rw-rwxr--   0 tombh     (1000) tombh     (1000)        0 2022-07-09 01:05:07.000000 pygls-1.0.1/tests/lsp/semantic_tokens/__init__.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3499 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_delta_missing_legend.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2110 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_delta_missing_legend_none.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2029 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_full_missing_legend.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3720 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_range.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2033 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_range_missing_legends.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3374 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/semantic_tokens/test_semantic_tokens_full.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6620 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_call_hierarchy.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4756 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_code_action.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3599 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_code_lens.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4094 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_color_presentation.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3850 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_completion.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5939 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_declaration.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5954 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_definition.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     3193 2023-01-30 00:57:57.000000 pygls-1.0.1/tests/lsp/test_diagnostics.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2995 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_document_color.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4080 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_document_highlight.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3583 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_document_link.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6301 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_document_symbol.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4477 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_errors.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3303 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_folding_range.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3888 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_formatting.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5141 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_hover.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6022 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_implementation.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3969 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_linked_editing_range.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3332 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_moniker.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4511 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_on_type_formatting.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4071 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_prepare_rename.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3715 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_progress.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4252 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_range_formatting.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3590 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_references.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6659 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_rename.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3964 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_selection_range.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6110 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_signature_help.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     6028 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/lsp/test_type_definition.py
-drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-02-16 12:12:38.958593 pygls-1.0.1/tests/pyodide_testrunner/
--rw-r--r--   0 tombh     (1000) tombh     (1000)        6 2023-01-28 20:44:49.000000 pygls-1.0.1/tests/pyodide_testrunner/.gitignore
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1368 2023-01-28 20:44:49.000000 pygls-1.0.1/tests/pyodide_testrunner/index.html
--rw-r--r--   0 tombh     (1000) tombh     (1000)       15 2023-01-28 20:44:49.000000 pygls-1.0.1/tests/pyodide_testrunner/requirements.txt
--rw-r--r--   0 tombh     (1000) tombh     (1000)     3507 2023-01-28 20:44:49.000000 pygls-1.0.1/tests/pyodide_testrunner/run.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     1117 2023-01-28 20:44:49.000000 pygls-1.0.1/tests/pyodide_testrunner/test-runner.js
--rw-rwxr--   0 tombh     (1000) tombh     (1000)    12409 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_capabilities.py
--rw-r--r--   0 tombh     (1000) tombh     (1000)     9187 2023-01-27 19:30:59.000000 pygls-1.0.1/tests/test_document.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     5521 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_feature_manager.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     4647 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_language_server.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)    19076 2022-12-14 16:23:23.000000 pygls-1.0.1/tests/test_protocol.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3732 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_server_connection.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3868 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_types.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     2967 2022-07-09 01:05:07.000000 pygls-1.0.1/tests/test_uris.py
--rw-rwxr--   0 tombh     (1000) tombh     (1000)     3155 2022-12-14 12:57:21.000000 pygls-1.0.1/tests/test_workspace.py
--rw-rw-r--   0 tombh     (1000) tombh     (1000)      308 2023-01-28 20:44:49.000000 pygls-1.0.1/tox.ini
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.931557 pygls-1.0.2/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      168 2022-05-26 11:42:47.000000 pygls-1.0.2/.editorconfig
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      679 2022-05-26 11:42:47.000000 pygls-1.0.2/.gitattributes
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.913557 pygls-1.0.2/.github/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)       70 2022-08-01 12:02:09.000000 pygls-1.0.2/.github/FUNDING.yml
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.913557 pygls-1.0.2/.github/workflows/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2487 2023-01-28 20:44:49.000000 pygls-1.0.2/.github/workflows/ci.yml
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2025 2023-01-28 20:44:49.000000 pygls-1.0.2/.github/workflows/json-extension.yml
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     1308 2023-01-28 20:45:05.000000 pygls-1.0.2/.gitignore
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)    12554 2023-05-16 13:17:38.000000 pygls-1.0.2/CHANGELOG.md
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3293 2022-05-26 11:42:47.000000 pygls-1.0.2/CODE_OF_CONDUCT.md
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3414 2022-05-26 11:42:47.000000 pygls-1.0.2/CONTRIBUTING.md
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)      999 2023-05-15 23:09:44.000000 pygls-1.0.2/CONTRIBUTORS.md
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     1517 2023-02-15 02:36:59.000000 pygls-1.0.2/HISTORY.md
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     5038 2023-05-15 23:09:44.000000 pygls-1.0.2/Implementations.md
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)    11367 2022-05-26 11:42:47.000000 pygls-1.0.2/LICENSE.txt
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)       36 2022-05-26 11:42:47.000000 pygls-1.0.2/MANIFEST.in
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     4661 2023-05-16 13:19:30.931557 pygls-1.0.2/PKG-INFO
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      959 2022-05-26 11:42:47.000000 pygls-1.0.2/PULL_REQUEST_TEMPLATE.md
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     3526 2023-01-28 20:44:49.000000 pygls-1.0.2/README.md
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     1261 2022-12-14 12:57:21.000000 pygls-1.0.2/RELEASING.md
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3034 2022-05-26 11:42:47.000000 pygls-1.0.2/ThirdPartyNotices.txt
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.914557 pygls-1.0.2/docs/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      584 2022-05-26 11:42:47.000000 pygls-1.0.2/docs/Makefile
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.914557 pygls-1.0.2/docs/assets/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     3076 2023-01-28 20:44:49.000000 pygls-1.0.2/docs/assets/hello-world-completion.png
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      756 2022-05-26 11:42:47.000000 pygls-1.0.2/docs/make.bat
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.914557 pygls-1.0.2/docs/source/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5086 2022-12-14 12:57:21.000000 pygls-1.0.2/docs/source/conf.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     1305 2022-12-14 12:57:21.000000 pygls-1.0.2/docs/source/index.rst
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.915557 pygls-1.0.2/docs/source/pages/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    16311 2023-01-27 19:25:21.000000 pygls-1.0.2/docs/source/pages/advanced_usage.rst
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2748 2023-01-27 19:25:21.000000 pygls-1.0.2/docs/source/pages/getting_started.rst
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    13338 2023-03-03 18:40:43.000000 pygls-1.0.2/docs/source/pages/migrating-to-v1.rst
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1025 2023-05-15 23:09:44.000000 pygls-1.0.2/docs/source/pages/testing.rst
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     7039 2023-05-15 23:09:44.000000 pygls-1.0.2/docs/source/pages/tutorial.rst
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.907557 pygls-1.0.2/examples/
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.917557 pygls-1.0.2/examples/fountain-vscode-extension/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)       16 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/.gitignore
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     3834 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/README.md
+-rw-r--r--   0 tombh     (1000) tombh     (1000)   408759 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/demo.png
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      487 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/fountain-language-configuration.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)   112116 2023-05-15 23:09:44.000000 pygls-1.0.2/examples/fountain-vscode-extension/package-lock.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1171 2023-05-15 23:09:44.000000 pygls-1.0.2/examples/fountain-vscode-extension/package.json
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.918557 pygls-1.0.2/examples/fountain-vscode-extension/src/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      850 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/src/client.ts
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      814 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/src/server.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1679 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/src/server.ts
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      268 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/tsconfig.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)   108088 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/tunnel.png
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1332 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/fountain-vscode-extension/webpack.config.js
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.918557 pygls-1.0.2/examples/hello-world/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2755 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/hello-world/README.md
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      711 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/hello-world/main.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.919557 pygls-1.0.2/examples/json-vscode-extension/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      245 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/.eslintrc.yml
+-rw-r--r--   0 tombh     (1000) tombh     (1000)       70 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/.gitignore
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.919557 pygls-1.0.2/examples/json-vscode-extension/.vscode/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1619 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/.vscode/launch.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      695 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/.vscode/tasks.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      120 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/.vscodeignore
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    11367 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/LICENSE.txt
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1175 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/README.md
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.907557 pygls-1.0.2/examples/json-vscode-extension/client/
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.920557 pygls-1.0.2/examples/json-vscode-extension/client/src/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     3495 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/client/src/extension.ts
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    98529 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/package-lock.json
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2060 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/package.json
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.920557 pygls-1.0.2/examples/json-vscode-extension/server/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/server/__init__.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     2203 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/server/__main__.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    11204 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/server/server.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.920557 pygls-1.0.2/examples/json-vscode-extension/server/tests/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/server/tests/__init__.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.920557 pygls-1.0.2/examples/json-vscode-extension/server/tests/unit/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1232 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/server/tests/unit/__init__.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     6070 2023-05-15 23:09:44.000000 pygls-1.0.2/examples/json-vscode-extension/server/tests/unit/test_features.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)      275 2023-01-28 20:44:49.000000 pygls-1.0.2/examples/json-vscode-extension/tsconfig.json
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.922557 pygls-1.0.2/pygls/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1511 2023-05-16 13:17:38.000000 pygls-1.0.2/pygls/__init__.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)    14497 2022-12-14 12:57:21.000000 pygls-1.0.2/pygls/capabilities.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     1470 2022-07-06 23:06:23.000000 pygls-1.0.2/pygls/constants.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6247 2022-12-14 12:57:21.000000 pygls-1.0.2/pygls/exceptions.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     8263 2022-12-14 12:57:21.000000 pygls-1.0.2/pygls/feature_manager.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.923557 pygls-1.0.2/pygls/lsp/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     5086 2023-05-15 23:09:44.000000 pygls-1.0.2/pygls/lsp/__init__.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2852 2022-12-14 12:57:21.000000 pygls-1.0.2/pygls/progress.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    37243 2023-01-30 00:57:57.000000 pygls-1.0.2/pygls/protocol.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)       65 2022-05-26 11:42:47.000000 pygls-1.0.2/pygls/py.typed
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    19431 2023-01-30 00:57:57.000000 pygls-1.0.2/pygls/server.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5323 2022-07-06 23:06:23.000000 pygls-1.0.2/pygls/uris.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)    14925 2023-01-27 19:30:59.000000 pygls-1.0.2/pygls/workspace.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.923557 pygls-1.0.2/pygls.egg-info/
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     4661 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/PKG-INFO
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     4298 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/SOURCES.txt
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)        1 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/dependency_links.txt
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)        1 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/not-zip-safe
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)      188 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/requires.txt
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)        6 2023-05-16 13:19:30.000000 pygls-1.0.2/pygls.egg-info/top_level.txt
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      199 2022-07-07 16:59:19.000000 pygls-1.0.2/pyproject.toml
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)     1573 2023-05-16 13:19:30.932557 pygls-1.0.2/setup.cfg
+-rwxrwxr-x   0 tombh     (1000) tombh     (1000)       93 2022-07-04 20:17:59.000000 pygls-1.0.2/setup.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.925557 pygls-1.0.2/tests/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     1628 2022-07-09 01:05:07.000000 pygls-1.0.2/tests/__init__.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)      932 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/_init_server_stall_fix_hack.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2508 2022-07-09 01:05:07.000000 pygls-1.0.2/tests/conftest.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5819 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/ls_setup.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.929557 pygls-1.0.2/tests/lsp/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)        0 2022-05-26 11:42:47.000000 pygls-1.0.2/tests/lsp/__init__.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.930557 pygls-1.0.2/tests/lsp/semantic_tokens/
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)        0 2022-07-09 01:05:07.000000 pygls-1.0.2/tests/lsp/semantic_tokens/__init__.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3499 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_delta_missing_legend.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2110 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_delta_missing_legend_none.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2029 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_full_missing_legend.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3720 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_range.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2033 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_range_missing_legends.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3374 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/semantic_tokens/test_semantic_tokens_full.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6620 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_call_hierarchy.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4756 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_code_action.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3599 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_code_lens.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4094 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_color_presentation.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3850 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_completion.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5939 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_declaration.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5954 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_definition.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     3193 2023-01-30 00:57:57.000000 pygls-1.0.2/tests/lsp/test_diagnostics.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2995 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_document_color.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4080 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_document_highlight.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3583 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_document_link.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6301 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_document_symbol.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4477 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_errors.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3303 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_folding_range.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3888 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_formatting.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     5141 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_hover.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6022 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_implementation.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3969 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_linked_editing_range.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3332 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_moniker.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4511 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_on_type_formatting.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4071 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_prepare_rename.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3715 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_progress.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4252 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_range_formatting.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3590 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_references.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6659 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_rename.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3964 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_selection_range.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6110 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_signature_help.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     6028 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/lsp/test_type_definition.py
+drwxrwxr-x   0 tombh     (1000) tombh     (1000)        0 2023-05-16 13:19:30.931557 pygls-1.0.2/tests/pyodide_testrunner/
+-rw-r--r--   0 tombh     (1000) tombh     (1000)        6 2023-01-28 20:44:49.000000 pygls-1.0.2/tests/pyodide_testrunner/.gitignore
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1368 2023-01-28 20:44:49.000000 pygls-1.0.2/tests/pyodide_testrunner/index.html
+-rw-r--r--   0 tombh     (1000) tombh     (1000)       15 2023-01-28 20:44:49.000000 pygls-1.0.2/tests/pyodide_testrunner/requirements.txt
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     3507 2023-01-28 20:44:49.000000 pygls-1.0.2/tests/pyodide_testrunner/run.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     1117 2023-01-28 20:44:49.000000 pygls-1.0.2/tests/pyodide_testrunner/test-runner.js
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)    12409 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/test_capabilities.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     9187 2023-01-27 19:30:59.000000 pygls-1.0.2/tests/test_document.py
+-rw-r--r--   0 tombh     (1000) tombh     (1000)     5565 2023-05-15 23:09:44.000000 pygls-1.0.2/tests/test_feature_manager.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     4647 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/test_language_server.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)    19076 2022-12-14 16:23:23.000000 pygls-1.0.2/tests/test_protocol.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3732 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/test_server_connection.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3868 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/test_types.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     2967 2022-07-09 01:05:07.000000 pygls-1.0.2/tests/test_uris.py
+-rw-rwxr--   0 tombh     (1000) tombh     (1000)     3155 2022-12-14 12:57:21.000000 pygls-1.0.2/tests/test_workspace.py
+-rw-rw-r--   0 tombh     (1000) tombh     (1000)      308 2023-01-28 20:44:49.000000 pygls-1.0.2/tox.ini
```

### Comparing `pygls-1.0.1/.gitattributes` & `pygls-1.0.2/.gitattributes`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/.github/workflows/ci.yml` & `pygls-1.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/.github/workflows/json-extension.yml` & `pygls-1.0.2/.github/workflows/json-extension.yml`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/.gitignore` & `pygls-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/CHANGELOG.md` & `pygls-1.0.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,32 @@
 and this project adheres to [Semantic Versioning][semver].
 
 ## [Unreleased]
 ### Added
 ### Changed
 ### Fixed
 
+## [1.0.2] - May 15th, 2023
+### Changed
+- Update typeguard to 3.x ([#327])
+
+### Fixed
+- Data files are no longer placed inside the wrong `site-packages` folder when installing `pygls` ([#232])
+[#232]: https://github.com/openlawlibrary/pygls/issues/232
+
+
 ## [1.0.1] - February 16th, 2023
 ### Fixed
 
  - Fix progress example in json extension. ([#230])
  - Fix `AttributeErrors` in `get_configuration_async`, `get_configuration_callback`, `get_configuration_threaded` commands in json extension. ([#307])
  - Fix type annotations for `get_configuration_async` and `get_configuration` methods on `LanguageServer` and `LanguageServerProtocol` objects ([#307])
- - Provide `version` param for publishing diagnostics ([#303]) 
+ - Provide `version` param for publishing diagnostics ([#303])
  - Relaxed the Python version upper bound to `<4` ([#318])
- 
+
 [#230]: https://github.com/openlawlibrary/pygls/issues/230
 [#303]: https://github.com/openlawlibrary/pygls/issues/303
 [#307]: https://github.com/openlawlibrary/pygls/issues/307
 [#318]: https://github.com/openlawlibrary/pygls/issues/318
 
 ## [1.0.0] - 2/12/2022
 ### Changed
```

### Comparing `pygls-1.0.1/CODE_OF_CONDUCT.md` & `pygls-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/CONTRIBUTING.md` & `pygls-1.0.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/CONTRIBUTORS.md` & `pygls-1.0.2/CONTRIBUTORS.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 - [Brett Cannon](https://github.com/brettcannon/)
 - [Daniel Elero](https://github.com/danixeee)
 - [Daniel Miller](https://github.com/millerdev)
 - [DeathAxe](https://github.com/deathaxe)
 - [Denis Loginov](https://github.com/dinvlad)
 - [Dillan Mills](https://github.com/DillanCMills)
 - [Felicián Németh](https://github.com/nemethf)
+- [Felix Yan](https://github.com/felixonmars)
+- [Jelle van der Waa](https://github.com/jelly)
 - [Jérome Perrin](https://github.com/perrinjerome)
 - [Karthik Nadig](https://github.com/karthiknadig)
 - [Laurence Warne](https://github.com/LaurenceWarne)
 - [Matej Kašťák](https://github.com/MatejKastak)
 - [Max O'Cull](https://github.com/Maxattax97)
 - [Samuel Roeca](https://github.com/pappasam)
 - [Tom BH](https://github.com/tombh)
```

### Comparing `pygls-1.0.1/HISTORY.md` & `pygls-1.0.2/HISTORY.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/Implementations.md` & `pygls-1.0.2/Implementations.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 | _Jedi Language Server_   | [Samuel Roeca](https://softwarejourneyman.com/pages/about.html#about) | [jedi-language-server](https://github.com/pappasam/jedi-language-server)   | Python Language Server wrapping [Jedi](https://github.com/davidhalter/jedi)                                                   |
 | _Ruff Language Server_   | [Charlie Marsh](https://github.com/charliermarsh) | [ruff-lsp](https://github.com/charliermarsh/ruff-lsp) | Language Server for Python's [ruff](https://github.com/charliermarsh/ruff) |
 | _Stata Language Server_   | [Hai Bo](https://github.com/HankBO) | [stata-language-server](https://github.com/HankBO/stata-language-server)   | Language Server for [Stata](https://www.stata.com/)  |
 | _VSCode `autopep8` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-autopep8](https://github.com/microsoft/vscode-autopep8) | VSCode extension for Python's [autopep8](https://github.com/hhatto/autopep8) |
 | _VSCode `black` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-black-formatter](https://github.com/microsoft/vscode-black-formatter) | VSCode extension for Python's [black](https://github.com/psf/black) |
 | _VSCode `isort` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-isort](https://github.com/microsoft/vscode-isort) | VSCode extension for Python's [isort](https://pycqa.github.io/isort) |
 | _VSCode `flake8` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-flake8](https://github.com/microsoft/vscode-flake8) | VSCode extension for Python's [flake8](https://github.com/PyCQA/flake8) |
+| _VSCode `mypy` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-mypy](https://github.com/microsoft/vscode-mypy) | VSCode extension for Python's [mypy](https://github.com/python/mypy) |
 | _VSCode `pylint` extension_   | [Microsoft](https://github.com/microsoft) | [vscode-pylint](https://github.com/microsoft/vscode-pylint) | VSCode extension for Python's [pylint](https://github.com/PyCQA/pylint) |
 | _VSCode `ufmt` extension_   | [Omnilib](https://github.com/omnilib) | [vscode-ufmt](https://github.com/omnilib/vscode-ufmt) | VSCode extension for Python's [ufmt](https://ufmt.omnilib.dev/en/stable/) |
 | _YARA Language Server_   | [Avast](https://github.com/avast) | [yls](https://github.com/avast/yls) | Language Server for [YARA](https://github.com/VirusTotal/yara) |
 | _zc.buildout Language Server_   | [Jérome Perrin](https://github.com/perrinjerome) | [zc.buildout.languageserver](https://github.com/perrinjerome/vscode-zc-buildout)   | Language Server for [zc.buildout](http://docs.buildout.org/en/latest/) profiles.  |
 
 ## _(alphabetic by name, maintainer)_
```

### Comparing `pygls-1.0.1/LICENSE.txt` & `pygls-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/PKG-INFO` & `pygls-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygls
-Version: 1.0.1
+Version: 1.0.2
 Summary: a pythonic generic language server (pronounced like "pie glass").
 Home-page: https://github.com/openlawlibrary/pygls/tree/master/
 Author: Open Law Library
 Author-email: info@openlawlib.org
 License: Apache 2.0
 Keywords: python,pythonic,generic,language,server,protocol
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygls-1.0.1/PULL_REQUEST_TEMPLATE.md` & `pygls-1.0.2/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/README.md` & `pygls-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/RELEASING.md` & `pygls-1.0.2/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/ThirdPartyNotices.txt` & `pygls-1.0.2/ThirdPartyNotices.txt`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/Makefile` & `pygls-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/assets/hello-world-completion.png` & `pygls-1.0.2/docs/assets/hello-world-completion.png`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/make.bat` & `pygls-1.0.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/source/conf.py` & `pygls-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/source/index.rst` & `pygls-1.0.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/source/pages/advanced_usage.rst` & `pygls-1.0.2/docs/source/pages/advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/source/pages/getting_started.rst` & `pygls-1.0.2/docs/source/pages/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/docs/source/pages/migrating-to-v1.rst` & `pygls-1.0.2/docs/source/pages/migrating-to-v1.rst`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 Known Migrations
 ----------------
 You may find insight and inspiration from these projects that have already successfully migrated to v1:
 
 * `jedi-language-server`_
 * `vscode-ruff`_
 * `esbonio`_
+* `yara-language-server`_
 
 Updating Imports
 ----------------
 
 The ``pygls.lsp.methods`` and ``pygls.lsp.types`` modules no longer exist.
 Instead, all types and method names should now be imported from the ``lsprotocol.types`` module.
 
@@ -231,9 +232,10 @@
 .. _cattrs: https://cattrs.readthedocs.io/en/stable/
 .. _converter: https://cattrs.readthedocs.io/en/stable/converters.html
 .. _hooks.py: https://github.com/microsoft/lsprotocol/blob/main/lsprotocol/_hooks.py
 .. _lsprotocol: https://github.com/microsoft/lsprotocol
 .. _pydantic: https://pydantic-docs.helpmanual.io/
 .. _structure hooks: https://cattrs.readthedocs.io/en/stable/structuring.html#registering-custom-structuring-hooks
 .. _jedi-language-server: https://github.com/pappasam/jedi-language-server/pull/230
+.. _yara-language-server: https://github.com/avast/yls/pull/34
 .. _vscode-ruff: https://github.com/charliermarsh/vscode-ruff/pull/37
 .. _esbonio: https://github.com/swyddfa/esbonio/pull/484
```

### Comparing `pygls-1.0.1/docs/source/pages/testing.rst` & `pygls-1.0.2/docs/source/pages/testing.rst`

 * *Files 12% similar despite different names*

```diff
@@ -16,13 +16,13 @@
 Integration Tests
 -----------------
 
 Integration tests coverage includes the whole workflow, from sending the client
 request, to getting the result from the server. Since the *Language Server
 Protocol* defines bidirectional communication between the client and the
 server, we used *pygls* to simulate the client and send desired requests to the
-server. To get better understanding of how setup it, take a look at our test
+server. To get a better understanding of how to set it up, take a look at our test
 `fixtures`_.
 
 
-.. _unit tests: https://github.com/openlawlibrary/pygls/blob/master/examples/json-extension/server/tests/unit
+.. _unit tests: https://github.com/openlawlibrary/pygls/blob/master/examples/json-vscode-extension/server/tests/unit
 .. _fixtures: https://github.com/openlawlibrary/pygls/blob/master/tests/conftest.py#L29
```

### Comparing `pygls-1.0.1/docs/source/pages/tutorial.rst` & `pygls-1.0.2/docs/source/pages/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -190,11 +190,11 @@
 
 Modify the Example
 ~~~~~~~~~~~~~~~~~~
 
 We encourage you to continue to :ref:`advanced section <advanced-usage>` and
 modify this example.
 
-.. _json-extension: https://github.com/openlawlibrary/pygls/blob/master/examples/json-extension
-.. _README: https://github.com/openlawlibrary/pygls/blob/master/examples/json-extension/README.md
-.. _server.py: https://github.com/openlawlibrary/pygls/blob/master/examples/json-extension/server/server.py
+.. _json-extension: https://github.com/openlawlibrary/pygls/blob/master/examples/json-vscode-extension
+.. _README: https://github.com/openlawlibrary/pygls/blob/master/examples/json-vscode-extension/README.md
+.. _server.py: https://github.com/openlawlibrary/pygls/blob/master/examples/json-vscode-extension/server/server.py
 .. _cooperative multitasking: https://en.wikipedia.org/wiki/Cooperative_multitasking
```

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/README.md` & `pygls-1.0.2/examples/fountain-vscode-extension/README.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/demo.png` & `pygls-1.0.2/examples/fountain-vscode-extension/demo.png`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/package-lock.json` & `pygls-1.0.2/examples/fountain-vscode-extension/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962177584657025%*

 * *Differences: {"'dependencies'": "{'@types/eslint': {'version': '8.21.2', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/eslint/-/eslint-8.21.2.tgz', 'integrity': "*

 * *                   "'sha512-EMpxUyystd3uZVByZap1DACsMXvb82ypQnGn89e1Y0a+LYu3JJscUd/gqhRsVFDkaD2MIiWo0MT8EfXr3DGRKw=='}, "*

 * *                   "'@types/eslint-scope': {'version': '3.7.4', 'resolved': "*

 * *                   "'https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz', "*

 * *                   "'integrity': "*

 * *        […]*

```diff
@@ -53,37 +53,37 @@
                 "@jridgewell/sourcemap-codec": "^1.4.10"
             },
             "resolved": "https://registry.npmjs.org/@jridgewell/trace-mapping/-/trace-mapping-0.3.14.tgz",
             "version": "0.3.14"
         },
         "@types/eslint": {
             "dev": true,
-            "integrity": "sha512-KubbADPkfoU75KgKeKLsFHXnU4ipH7wYg0TRT33NK3N3yiu7jlFAAoygIWBV+KbuHx/G+AvuGX6DllnK35gfJA==",
+            "integrity": "sha512-EMpxUyystd3uZVByZap1DACsMXvb82ypQnGn89e1Y0a+LYu3JJscUd/gqhRsVFDkaD2MIiWo0MT8EfXr3DGRKw==",
             "requires": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-7.28.2.tgz",
-            "version": "7.28.2"
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.21.2.tgz",
+            "version": "8.21.2"
         },
         "@types/eslint-scope": {
             "dev": true,
-            "integrity": "sha512-SCFeogqiptms4Fg29WpOTk5nHIzfpKCemSN63ksBQYKTcXoJEmJagV+DhVmbapZzY4/5YaOV1nZwrsU79fFm1g==",
+            "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
             "requires": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
-            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.1.tgz",
-            "version": "3.7.1"
+            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
+            "version": "3.7.4"
         },
         "@types/estree": {
             "dev": true,
-            "integrity": "sha512-C6N5s2ZFtuZRj54k2/zyRhNDjJwwcViAM3Nbm8zjBpbqAdZ00mr0CFxvSKeO8Y/e03WVFLpQMdHYVfUd6SB+Hw==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.50.tgz",
-            "version": "0.0.50"
+            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
+            "version": "0.0.51"
         },
         "@types/json-schema": {
             "dev": true,
             "integrity": "sha512-qcUXuemtEu+E5wZSJHNxUXeCZhAfXKQ41D+duX+VYPde7xyEVZci+/oXKJL13tnRs9lR2pr4fod59GT6/X1/yQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.9.tgz",
             "version": "7.0.9"
         },
@@ -278,17 +278,17 @@
             "dev": true,
             "integrity": "sha512-NuHqBY1PB/D8xU6s/thBgOAiAP7HOYDQ32+BFZILJ8ivkUkAHQnWfn6WhL79Owj1qmUnoN/YPhktdIoucipkAQ==",
             "resolved": "https://registry.npmjs.org/@xtuc/long/-/long-4.2.2.tgz",
             "version": "4.2.2"
         },
         "acorn": {
             "dev": true,
-            "integrity": "sha512-yXbYeFy+jUuYd3/CDcg2NkIYE991XYX/bje7LmjJigUciaeO1JR4XxXgCIV1/Zc/dRuFEyw1L0pbA+qynJkW5Q==",
-            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.5.0.tgz",
-            "version": "8.5.0"
+            "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
+            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
+            "version": "8.8.2"
         },
         "acorn-import-assertions": {
             "dev": true,
             "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
             "requires": {},
             "resolved": "https://registry.npmjs.org/acorn-import-assertions/-/acorn-import-assertions-1.8.0.tgz",
             "version": "1.8.0"
@@ -443,21 +443,21 @@
             "dev": true,
             "integrity": "sha512-ChtwF7qB03INq1SyMpue08wc6cve+ktj2UC/Y7se9vB+JryfzziJeYwsgb8jLaCA5GMkHCdn5M62PfSMWhifZg==",
             "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.3.893.tgz",
             "version": "1.3.893"
         },
         "enhanced-resolve": {
             "dev": true,
-            "integrity": "sha512-EGAbGvH7j7Xt2nc0E7D99La1OiEs8LnyimkRgwExpUMScN6O+3x9tIWs7PLQZVNx4YD+00skHXPXi1yQHpAmZA==",
+            "integrity": "sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==",
             "requires": {
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.8.3.tgz",
-            "version": "5.8.3"
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz",
+            "version": "5.12.0"
         },
         "envinfo": {
             "dev": true,
             "integrity": "sha512-/o+BXHmB7ocbHEAs6F2EnG0ogybVVUdkRunTT2glZU9XAaGmhqskrvKwqXuDfNjEO0LZKWdejEEpnq8aM0tOaw==",
             "resolved": "https://registry.npmjs.org/envinfo/-/envinfo-7.8.1.tgz",
             "version": "7.8.1"
         },
@@ -582,17 +582,17 @@
             "dev": true,
             "integrity": "sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==",
             "resolved": "https://registry.npmjs.org/glob-to-regexp/-/glob-to-regexp-0.4.1.tgz",
             "version": "0.4.1"
         },
         "graceful-fs": {
             "dev": true,
-            "integrity": "sha512-qkIilPUYcNhJpd33n0GBXTB1MMPp14TxEsEs0pTrsSVucApsYzW5V+Q8Qxhik6KU3evy+qkAAowTByymK0avdg==",
-            "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.8.tgz",
-            "version": "4.2.8"
+            "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
+            "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
+            "version": "4.2.11"
         },
         "has": {
             "dev": true,
             "integrity": "sha512-f2dvO0VU6Oej7RkWJGrehjbzMAjFp5/VKPp5tTpWIV4JHHZK1/BxbFRtf/siA2SWTe09caDmVtYYzWEIbBS4zw==",
             "requires": {
                 "function-bind": "^1.1.1"
             },
@@ -687,19 +687,19 @@
                 "@types/node": "*",
                 "merge-stream": "^2.0.0",
                 "supports-color": "^8.0.0"
             },
             "resolved": "https://registry.npmjs.org/jest-worker/-/jest-worker-27.3.1.tgz",
             "version": "27.3.1"
         },
-        "json-parse-better-errors": {
+        "json-parse-even-better-errors": {
             "dev": true,
-            "integrity": "sha512-mrqyZKfX5EhL7hvqcV6WG1yYjnjeuYDzDhhcAAUrq8Po85NBQBJP+ZDUT75qZQ98IkUoBqdkExkukOU7Ts2wrw==",
-            "resolved": "https://registry.npmjs.org/json-parse-better-errors/-/json-parse-better-errors-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==",
+            "resolved": "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz",
+            "version": "2.3.1"
         },
         "json-schema-traverse": {
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
@@ -1114,53 +1114,53 @@
         "vscode-languageserver-types": {
             "integrity": "sha512-k8luDIWJWyenLc5ToFQQMaSrqCHiLwyKPHKPQZ5zz21vM+vIVUSvsRpcbiECH4WR88K2XZqc4ScRcZ7nk/jbeA==",
             "resolved": "https://registry.npmjs.org/vscode-languageserver-types/-/vscode-languageserver-types-3.16.0.tgz",
             "version": "3.16.0"
         },
         "watchpack": {
             "dev": true,
-            "integrity": "sha512-up4YAn/XHgZHIxFBVCdlMiWDj6WaLKpwVeGQk2I5thdYxF/KmF0aaz6TfJZ/hfl1h/XlcDr7k1KH7ThDagpFaA==",
+            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
             "requires": {
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
-            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.2.0.tgz",
-            "version": "2.2.0"
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
+            "version": "2.4.0"
         },
         "webpack": {
             "dev": true,
-            "integrity": "sha512-HYrw6bkj/MDmphAXvqLEvn2fVoDZsYu6O638WjK6lSNgIpjb5jl/KtOrqJyU9EC/ZV9mLUmZW5h4mASB+CVA4A==",
+            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
             "requires": {
-                "@types/eslint-scope": "^3.7.0",
-                "@types/estree": "^0.0.50",
+                "@types/eslint-scope": "^3.7.3",
+                "@types/estree": "^0.0.51",
                 "@webassemblyjs/ast": "1.11.1",
                 "@webassemblyjs/wasm-edit": "1.11.1",
                 "@webassemblyjs/wasm-parser": "1.11.1",
-                "acorn": "^8.4.1",
+                "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.8.3",
+                "enhanced-resolve": "^5.10.0",
                 "es-module-lexer": "^0.9.0",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
-                "graceful-fs": "^4.2.4",
-                "json-parse-better-errors": "^1.0.2",
+                "graceful-fs": "^4.2.9",
+                "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
                 "schema-utils": "^3.1.0",
                 "tapable": "^2.1.1",
                 "terser-webpack-plugin": "^5.1.3",
-                "watchpack": "^2.2.0",
-                "webpack-sources": "^3.2.0"
+                "watchpack": "^2.4.0",
+                "webpack-sources": "^3.2.3"
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.63.0.tgz",
-            "version": "5.63.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
+            "version": "5.76.0"
         },
         "webpack-cli": {
             "dependencies": {
                 "commander": {
                     "dev": true,
                     "integrity": "sha512-QrWXB+ZQSVPmIWIhtEO9H+gwHaMGYiF5ChvoJ+K9ZGHG/sVsa6yiesAD1GC/x46sET00Xlwo1u49RVVVzvcSkw==",
                     "resolved": "https://registry.npmjs.org/commander/-/commander-7.2.0.tgz",
@@ -1194,17 +1194,17 @@
                 "wildcard": "^2.0.0"
             },
             "resolved": "https://registry.npmjs.org/webpack-merge/-/webpack-merge-5.8.0.tgz",
             "version": "5.8.0"
         },
         "webpack-sources": {
             "dev": true,
-            "integrity": "sha512-t6BMVLQ0AkjBOoRTZgqrWm7xbXMBzD+XDq2EZ96+vMfn3qKgsvdXZhbPZ4ElUOpdv4u+iiGe+w3+J75iy/bYGA==",
-            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.1.tgz",
-            "version": "3.2.1"
+            "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
+            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
+            "version": "3.2.3"
         },
         "which": {
             "dev": true,
             "integrity": "sha512-BLI3Tl1TW3Pvl70l3yq3Y64i+awpwXqsGBYWkkqMtnbXgrMD+yj7rhW0kuEDxzJaYXGjEW5ogapKNMEKNMjibA==",
             "requires": {
                 "isexe": "^2.0.0"
             },
@@ -1231,15 +1231,15 @@
                 "vscode-languageclient": "^7.0.0"
             },
             "devDependencies": {
                 "@types/vscode": "^1.62.0",
                 "path-browserify": "^1.0.1",
                 "ts-loader": "^9.2.6",
                 "typescript": "^4.4.4",
-                "webpack": "^5.63.0",
+                "webpack": "^5.76.0",
                 "webpack-cli": "^4.9.1"
             },
             "engines": {
                 "vscode": "^1.62.0"
             },
             "license": "Apache-2.0",
             "name": "fountain-extension",
@@ -1314,33 +1314,33 @@
         },
         "node_modules/@types/eslint": {
             "dependencies": {
                 "@types/estree": "*",
                 "@types/json-schema": "*"
             },
             "dev": true,
-            "integrity": "sha512-KubbADPkfoU75KgKeKLsFHXnU4ipH7wYg0TRT33NK3N3yiu7jlFAAoygIWBV+KbuHx/G+AvuGX6DllnK35gfJA==",
-            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-7.28.2.tgz",
-            "version": "7.28.2"
+            "integrity": "sha512-EMpxUyystd3uZVByZap1DACsMXvb82ypQnGn89e1Y0a+LYu3JJscUd/gqhRsVFDkaD2MIiWo0MT8EfXr3DGRKw==",
+            "resolved": "https://registry.npmjs.org/@types/eslint/-/eslint-8.21.2.tgz",
+            "version": "8.21.2"
         },
         "node_modules/@types/eslint-scope": {
             "dependencies": {
                 "@types/eslint": "*",
                 "@types/estree": "*"
             },
             "dev": true,
-            "integrity": "sha512-SCFeogqiptms4Fg29WpOTk5nHIzfpKCemSN63ksBQYKTcXoJEmJagV+DhVmbapZzY4/5YaOV1nZwrsU79fFm1g==",
-            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.1.tgz",
-            "version": "3.7.1"
+            "integrity": "sha512-9K4zoImiZc3HlIp6AVUDE4CWYx22a+lhSZMYNpbjW04+YF0KWj4pJXnEMjdnFTiQibFFmElcsasJXDbdI/EPhA==",
+            "resolved": "https://registry.npmjs.org/@types/eslint-scope/-/eslint-scope-3.7.4.tgz",
+            "version": "3.7.4"
         },
         "node_modules/@types/estree": {
             "dev": true,
-            "integrity": "sha512-C6N5s2ZFtuZRj54k2/zyRhNDjJwwcViAM3Nbm8zjBpbqAdZ00mr0CFxvSKeO8Y/e03WVFLpQMdHYVfUd6SB+Hw==",
-            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.50.tgz",
-            "version": "0.0.50"
+            "integrity": "sha512-CuPgU6f3eT/XgKKPqKd/gLZV1Xmvf1a2R5POBOGQa6uv82xpls89HU5zKeVoyR8XzHd1RGNOlQlvUe3CFkjWNQ==",
+            "resolved": "https://registry.npmjs.org/@types/estree/-/estree-0.0.51.tgz",
+            "version": "0.0.51"
         },
         "node_modules/@types/json-schema": {
             "dev": true,
             "integrity": "sha512-qcUXuemtEu+E5wZSJHNxUXeCZhAfXKQ41D+duX+VYPde7xyEVZci+/oXKJL13tnRs9lR2pr4fod59GT6/X1/yQ==",
             "resolved": "https://registry.npmjs.org/@types/json-schema/-/json-schema-7.0.9.tgz",
             "version": "7.0.9"
         },
@@ -1554,17 +1554,17 @@
             "bin": {
                 "acorn": "bin/acorn"
             },
             "dev": true,
             "engines": {
                 "node": ">=0.4.0"
             },
-            "integrity": "sha512-yXbYeFy+jUuYd3/CDcg2NkIYE991XYX/bje7LmjJigUciaeO1JR4XxXgCIV1/Zc/dRuFEyw1L0pbA+qynJkW5Q==",
-            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.5.0.tgz",
-            "version": "8.5.0"
+            "integrity": "sha512-xjIYgE8HBrkpd/sJqOGNspf8uHG+NOHGOw6a/Urj8taM2EXfdNAH2oFcPeIFfsv3+kz/mJrS5VuMqbNLjCa2vw==",
+            "resolved": "https://registry.npmjs.org/acorn/-/acorn-8.8.2.tgz",
+            "version": "8.8.2"
         },
         "node_modules/acorn-import-assertions": {
             "dev": true,
             "integrity": "sha512-m7VZ3jwz4eK6A4Vtt8Ew1/mNbP24u0FhdyfA7fSvnJR6LMdfOYnmuIrrJAgrYfYJ10F/otaHTtrtrtmHdMNzEw==",
             "peerDependencies": {
                 "acorn": "^8"
             },
@@ -1775,17 +1775,17 @@
                 "graceful-fs": "^4.2.4",
                 "tapable": "^2.2.0"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-EGAbGvH7j7Xt2nc0E7D99La1OiEs8LnyimkRgwExpUMScN6O+3x9tIWs7PLQZVNx4YD+00skHXPXi1yQHpAmZA==",
-            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.8.3.tgz",
-            "version": "5.8.3"
+            "integrity": "sha512-QHTXI/sZQmko1cbDoNAa3mJ5qhWUUNAq3vR0/YiD379fWQrcfuoX1+HW2S0MTt7XmoPLapdaDKUtelUSPic7hQ==",
+            "resolved": "https://registry.npmjs.org/enhanced-resolve/-/enhanced-resolve-5.12.0.tgz",
+            "version": "5.12.0"
         },
         "node_modules/envinfo": {
             "bin": {
                 "envinfo": "dist/cli.js"
             },
             "dev": true,
             "engines": {
@@ -1950,17 +1950,17 @@
             "dev": true,
             "integrity": "sha512-lkX1HJXwyMcprw/5YUZc2s7DrpAiHB21/V+E1rHUrVNokkvB6bqMzT0VfV6/86ZNabt1k14YOIaT7nDvOX3Iiw==",
             "resolved": "https://registry.npmjs.org/glob-to-regexp/-/glob-to-regexp-0.4.1.tgz",
             "version": "0.4.1"
         },
         "node_modules/graceful-fs": {
             "dev": true,
-            "integrity": "sha512-qkIilPUYcNhJpd33n0GBXTB1MMPp14TxEsEs0pTrsSVucApsYzW5V+Q8Qxhik6KU3evy+qkAAowTByymK0avdg==",
-            "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.8.tgz",
-            "version": "4.2.8"
+            "integrity": "sha512-RbJ5/jmFcNNCcDV5o9eTnBLJ/HszWV0P73bc+Ff4nS/rJj+YaS6IGyiOL0VoBYX+l1Wrl3k63h/KrH+nhJ0XvQ==",
+            "resolved": "https://registry.npmjs.org/graceful-fs/-/graceful-fs-4.2.11.tgz",
+            "version": "4.2.11"
         },
         "node_modules/has": {
             "dependencies": {
                 "function-bind": "^1.1.1"
             },
             "dev": true,
             "engines": {
@@ -2098,19 +2098,19 @@
             "funding": {
                 "url": "https://github.com/chalk/supports-color?sponsor=1"
             },
             "integrity": "sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
             "version": "8.1.1"
         },
-        "node_modules/json-parse-better-errors": {
+        "node_modules/json-parse-even-better-errors": {
             "dev": true,
-            "integrity": "sha512-mrqyZKfX5EhL7hvqcV6WG1yYjnjeuYDzDhhcAAUrq8Po85NBQBJP+ZDUT75qZQ98IkUoBqdkExkukOU7Ts2wrw==",
-            "resolved": "https://registry.npmjs.org/json-parse-better-errors/-/json-parse-better-errors-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==",
+            "resolved": "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz",
+            "version": "2.3.1"
         },
         "node_modules/json-schema-traverse": {
             "dev": true,
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
             "resolved": "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz",
             "version": "0.4.1"
         },
@@ -2708,64 +2708,64 @@
                 "glob-to-regexp": "^0.4.1",
                 "graceful-fs": "^4.1.2"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-up4YAn/XHgZHIxFBVCdlMiWDj6WaLKpwVeGQk2I5thdYxF/KmF0aaz6TfJZ/hfl1h/XlcDr7k1KH7ThDagpFaA==",
-            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.2.0.tgz",
-            "version": "2.2.0"
+            "integrity": "sha512-Lcvm7MGST/4fup+ifyKi2hjyIAwcdI4HRgtvTpIUxBRhB+RFtUh8XtDOxUfctVCnhVi+QQj49i91OyvzkJl6cg==",
+            "resolved": "https://registry.npmjs.org/watchpack/-/watchpack-2.4.0.tgz",
+            "version": "2.4.0"
         },
         "node_modules/webpack": {
             "bin": {
                 "webpack": "bin/webpack.js"
             },
             "dependencies": {
-                "@types/eslint-scope": "^3.7.0",
-                "@types/estree": "^0.0.50",
+                "@types/eslint-scope": "^3.7.3",
+                "@types/estree": "^0.0.51",
                 "@webassemblyjs/ast": "1.11.1",
                 "@webassemblyjs/wasm-edit": "1.11.1",
                 "@webassemblyjs/wasm-parser": "1.11.1",
-                "acorn": "^8.4.1",
+                "acorn": "^8.7.1",
                 "acorn-import-assertions": "^1.7.6",
                 "browserslist": "^4.14.5",
                 "chrome-trace-event": "^1.0.2",
-                "enhanced-resolve": "^5.8.3",
+                "enhanced-resolve": "^5.10.0",
                 "es-module-lexer": "^0.9.0",
                 "eslint-scope": "5.1.1",
                 "events": "^3.2.0",
                 "glob-to-regexp": "^0.4.1",
-                "graceful-fs": "^4.2.4",
-                "json-parse-better-errors": "^1.0.2",
+                "graceful-fs": "^4.2.9",
+                "json-parse-even-better-errors": "^2.3.1",
                 "loader-runner": "^4.2.0",
                 "mime-types": "^2.1.27",
                 "neo-async": "^2.6.2",
                 "schema-utils": "^3.1.0",
                 "tapable": "^2.1.1",
                 "terser-webpack-plugin": "^5.1.3",
-                "watchpack": "^2.2.0",
-                "webpack-sources": "^3.2.0"
+                "watchpack": "^2.4.0",
+                "webpack-sources": "^3.2.3"
             },
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/webpack"
             },
-            "integrity": "sha512-HYrw6bkj/MDmphAXvqLEvn2fVoDZsYu6O638WjK6lSNgIpjb5jl/KtOrqJyU9EC/ZV9mLUmZW5h4mASB+CVA4A==",
+            "integrity": "sha512-l5sOdYBDunyf72HW8dF23rFtWq/7Zgvt/9ftMof71E/yUb1YLOBmTgA2K4vQthB3kotMrSj609txVE0dnr2fjA==",
             "peerDependenciesMeta": {
                 "webpack-cli": {
                     "optional": true
                 }
             },
-            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.63.0.tgz",
-            "version": "5.63.0"
+            "resolved": "https://registry.npmjs.org/webpack/-/webpack-5.76.0.tgz",
+            "version": "5.76.0"
         },
         "node_modules/webpack-cli": {
             "bin": {
                 "webpack-cli": "bin/cli.js"
             },
             "dependencies": {
                 "@discoveryjs/json-ext": "^0.5.0",
@@ -2829,17 +2829,17 @@
             "version": "5.8.0"
         },
         "node_modules/webpack-sources": {
             "dev": true,
             "engines": {
                 "node": ">=10.13.0"
             },
-            "integrity": "sha512-t6BMVLQ0AkjBOoRTZgqrWm7xbXMBzD+XDq2EZ96+vMfn3qKgsvdXZhbPZ4ElUOpdv4u+iiGe+w3+J75iy/bYGA==",
-            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.1.tgz",
-            "version": "3.2.1"
+            "integrity": "sha512-/DyMEOrDgLKKIG0fmvtz+4dUX/3Ghozwgm6iPp8KRhvn+eQf9+Q7GWxVNMk3+uCPWfdXYC4ExGBckIXdFEfH1w==",
+            "resolved": "https://registry.npmjs.org/webpack-sources/-/webpack-sources-3.2.3.tgz",
+            "version": "3.2.3"
         },
         "node_modules/which": {
             "bin": {
                 "node-which": "bin/node-which"
             },
             "dependencies": {
                 "isexe": "^2.0.0"
```

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/package.json` & `pygls-1.0.2/examples/fountain-vscode-extension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9972222222222222%*

 * *Differences: {"'devDependencies'": "{'webpack': '^5.76.0'}"}*

```diff
@@ -26,15 +26,15 @@
     },
     "description": "Example web extension that adds language support for the Fountain screenwriting format.",
     "devDependencies": {
         "@types/vscode": "^1.62.0",
         "path-browserify": "^1.0.1",
         "ts-loader": "^9.2.6",
         "typescript": "^4.4.4",
-        "webpack": "^5.63.0",
+        "webpack": "^5.76.0",
         "webpack-cli": "^4.9.1"
     },
     "engines": {
         "vscode": "^1.62.0"
     },
     "license": "Apache-2.0",
     "name": "fountain-extension",
```

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/src/client.ts` & `pygls-1.0.2/examples/fountain-vscode-extension/src/client.ts`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/src/server.py` & `pygls-1.0.2/examples/fountain-vscode-extension/src/server.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/src/server.ts` & `pygls-1.0.2/examples/fountain-vscode-extension/src/server.ts`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/tunnel.png` & `pygls-1.0.2/examples/fountain-vscode-extension/tunnel.png`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/fountain-vscode-extension/webpack.config.js` & `pygls-1.0.2/examples/fountain-vscode-extension/webpack.config.js`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/hello-world/README.md` & `pygls-1.0.2/examples/hello-world/README.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/hello-world/main.py` & `pygls-1.0.2/examples/hello-world/main.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/.vscode/launch.json` & `pygls-1.0.2/examples/json-vscode-extension/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/.vscode/tasks.json` & `pygls-1.0.2/examples/json-vscode-extension/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/LICENSE.txt` & `pygls-1.0.2/examples/json-vscode-extension/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/README.md` & `pygls-1.0.2/examples/json-vscode-extension/README.md`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/client/src/extension.ts` & `pygls-1.0.2/examples/json-vscode-extension/client/src/extension.ts`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/package-lock.json` & `pygls-1.0.2/examples/json-vscode-extension/package-lock.json`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/package.json` & `pygls-1.0.2/examples/json-vscode-extension/package.json`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/__init__.py` & `pygls-1.0.2/examples/json-vscode-extension/server/__init__.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/__main__.py` & `pygls-1.0.2/examples/json-vscode-extension/server/__main__.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/server.py` & `pygls-1.0.2/examples/json-vscode-extension/server/server.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/tests/__init__.py` & `pygls-1.0.2/examples/json-vscode-extension/server/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/tests/unit/__init__.py` & `pygls-1.0.2/examples/json-vscode-extension/server/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/examples/json-vscode-extension/server/tests/unit/test_features.py` & `pygls-1.0.2/examples/json-vscode-extension/server/tests/unit/test_features.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import asyncio
 import io
 import json
 import threading
 import time
 
 import pytest
-from mock import Mock
+from unittest.mock import Mock
 from lsprotocol.types import (DidCloseTextDocumentParams,
                               DidOpenTextDocumentParams, TextDocumentIdentifier,
                               WorkspaceConfigurationResponse,
                               TextDocumentItem)
 from pygls.server import StdOutTransportAdapter
 from pygls.workspace import Document, Workspace
```

### Comparing `pygls-1.0.1/pygls/__init__.py` & `pygls-1.0.2/pygls/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,13 +15,13 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. #
 # See the License for the specific language governing permissions and      #
 # limitations under the License.                                           #
 ############################################################################
 import os
 import sys
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 
 IS_WIN = os.name == 'nt'
 IS_PYODIDE = 'pyodide' in sys.modules
 
 pygls = 'pygls'
```

### Comparing `pygls-1.0.1/pygls/capabilities.py` & `pygls-1.0.2/pygls/capabilities.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/constants.py` & `pygls-1.0.2/pygls/constants.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/exceptions.py` & `pygls-1.0.2/pygls/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/feature_manager.py` & `pygls-1.0.2/pygls/feature_manager.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/lsp/__init__.py` & `pygls-1.0.2/pygls/lsp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,11 +118,11 @@
         return lsp_methods_map[method_name][1]
     except KeyError:
         raise MethodTypeNotRegisteredError(method_name)
 
 
 def is_instance(o, t):
     try:
-        check_type('', o, t)
+        check_type(o, t)
         return True
     except TypeError:
         return False
```

### Comparing `pygls-1.0.1/pygls/progress.py` & `pygls-1.0.2/pygls/progress.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/protocol.py` & `pygls-1.0.2/pygls/protocol.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/server.py` & `pygls-1.0.2/pygls/server.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/uris.py` & `pygls-1.0.2/pygls/uris.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls/workspace.py` & `pygls-1.0.2/pygls/workspace.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/pygls.egg-info/PKG-INFO` & `pygls-1.0.2/pygls.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygls
-Version: 1.0.1
+Version: 1.0.2
 Summary: a pythonic generic language server (pronounced like "pie glass").
 Home-page: https://github.com/openlawlibrary/pygls/tree/master/
 Author: Open Law Library
 Author-email: info@openlawlib.org
 License: Apache 2.0
 Keywords: python,pythonic,generic,language,server,protocol
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pygls-1.0.1/pygls.egg-info/SOURCES.txt` & `pygls-1.0.2/pygls.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/setup.cfg` & `pygls-1.0.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 	setuptools_scm>=3.4.3
 	toml
 python_requires = >=3.7,<4
 packages = find:
 zip_safe = False
 install_requires = 
 	lsprotocol
-	typeguard>=2.10.0,<3
+	typeguard>=3,<4
 include_package_data = True
 tests_require = 
-	mock==4.0.3
 	pytest==7.1.2
 	pytest-asyncio==0.18.3
 
 [options.packages.find]
 exclude = 
 	tests
 	tests.*
@@ -53,23 +52,17 @@
 	bandit==1.7.4
 	flake8==4.0.1
 	mypy==0.961
 docs = 
 	sphinx==5.0.1
 	sphinx_rtd_theme==1.0.0
 test = 
-	mock==4.0.3
 	pytest==7.1.2
 	pytest-asyncio==0.18.3
 
-[options.data_files]
-lib/site-packages/pygls = 
-	ThirdPartyNotices.txt
-	./pygls/py.typed
-
 [flake8]
 max-line-length = 99
 
 [mypy]
 ignore_missing_imports = True
 
 [egg_info]
```

### Comparing `pygls-1.0.1/tests/__init__.py` & `pygls-1.0.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/_init_server_stall_fix_hack.py` & `pygls-1.0.2/tests/_init_server_stall_fix_hack.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/conftest.py` & `pygls-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/ls_setup.py` & `pygls-1.0.2/tests/ls_setup.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_delta_missing_legend.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_delta_missing_legend.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_delta_missing_legend_none.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_delta_missing_legend_none.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_full_missing_legend.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_full_missing_legend.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_range.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_range.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_range_missing_legends.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_range_missing_legends.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/semantic_tokens/test_semantic_tokens_full.py` & `pygls-1.0.2/tests/lsp/semantic_tokens/test_semantic_tokens_full.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_call_hierarchy.py` & `pygls-1.0.2/tests/lsp/test_call_hierarchy.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_code_action.py` & `pygls-1.0.2/tests/lsp/test_code_action.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_code_lens.py` & `pygls-1.0.2/tests/lsp/test_code_lens.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_color_presentation.py` & `pygls-1.0.2/tests/lsp/test_color_presentation.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_completion.py` & `pygls-1.0.2/tests/lsp/test_completion.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_declaration.py` & `pygls-1.0.2/tests/lsp/test_declaration.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_definition.py` & `pygls-1.0.2/tests/lsp/test_definition.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_diagnostics.py` & `pygls-1.0.2/tests/lsp/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_document_color.py` & `pygls-1.0.2/tests/lsp/test_document_color.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_document_highlight.py` & `pygls-1.0.2/tests/lsp/test_document_highlight.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_document_link.py` & `pygls-1.0.2/tests/lsp/test_document_link.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_document_symbol.py` & `pygls-1.0.2/tests/lsp/test_document_symbol.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_errors.py` & `pygls-1.0.2/tests/lsp/test_errors.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_folding_range.py` & `pygls-1.0.2/tests/lsp/test_folding_range.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_formatting.py` & `pygls-1.0.2/tests/lsp/test_formatting.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_hover.py` & `pygls-1.0.2/tests/lsp/test_hover.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_implementation.py` & `pygls-1.0.2/tests/lsp/test_implementation.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_linked_editing_range.py` & `pygls-1.0.2/tests/lsp/test_linked_editing_range.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_moniker.py` & `pygls-1.0.2/tests/lsp/test_moniker.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_on_type_formatting.py` & `pygls-1.0.2/tests/lsp/test_on_type_formatting.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_prepare_rename.py` & `pygls-1.0.2/tests/lsp/test_prepare_rename.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_progress.py` & `pygls-1.0.2/tests/lsp/test_progress.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_range_formatting.py` & `pygls-1.0.2/tests/lsp/test_range_formatting.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_references.py` & `pygls-1.0.2/tests/lsp/test_references.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_rename.py` & `pygls-1.0.2/tests/lsp/test_rename.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_selection_range.py` & `pygls-1.0.2/tests/lsp/test_selection_range.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_signature_help.py` & `pygls-1.0.2/tests/lsp/test_signature_help.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/lsp/test_type_definition.py` & `pygls-1.0.2/tests/lsp/test_type_definition.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/pyodide_testrunner/index.html` & `pygls-1.0.2/tests/pyodide_testrunner/index.html`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/pyodide_testrunner/run.py` & `pygls-1.0.2/tests/pyodide_testrunner/run.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/pyodide_testrunner/test-runner.js` & `pygls-1.0.2/tests/pyodide_testrunner/test-runner.js`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_capabilities.py` & `pygls-1.0.2/tests/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_document.py` & `pygls-1.0.2/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_feature_manager.py` & `pygls-1.0.2/tests/test_feature_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 from pygls.exceptions import (
     CommandAlreadyRegisteredError,
     FeatureAlreadyRegisteredError,
     ValidationError,
 )
 from pygls.feature_manager import has_ls_param_or_annotation, wrap_with_server
 from lsprotocol import types
+from typeguard import TypeCheckError
+from typeguard._utils import qualified_name
 
 
 def test_has_ls_param_or_annotation():
     class Temp:
         pass
 
     def f1(ls, a, b, c):
@@ -88,18 +90,18 @@
 
 
 def test_register_feature_with_wrong_options(feature_manager):
     class Options:
         pass
 
     with pytest.raises(
-        TypeError,
+        TypeCheckError,
         match=(
-            f'Options of method "{types.TEXT_DOCUMENT_COMPLETION}" should be instance of type '
-            "<class 'lsprotocol.types.CompletionOptions'>"
+            f'{qualified_name(Options)} is not an instance of '
+            "lsprotocol.types.CompletionOptions"
         ),  # noqa
     ):
 
         @feature_manager.feature(types.TEXT_DOCUMENT_COMPLETION, Options())
         def completions():
             pass
```

### Comparing `pygls-1.0.1/tests/test_language_server.py` & `pygls-1.0.2/tests/test_language_server.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_protocol.py` & `pygls-1.0.2/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_server_connection.py` & `pygls-1.0.2/tests/test_server_connection.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_types.py` & `pygls-1.0.2/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_uris.py` & `pygls-1.0.2/tests/test_uris.py`

 * *Files identical despite different names*

### Comparing `pygls-1.0.1/tests/test_workspace.py` & `pygls-1.0.2/tests/test_workspace.py`

 * *Files identical despite different names*

