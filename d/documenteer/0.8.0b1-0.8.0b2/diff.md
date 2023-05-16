# Comparing `tmp/documenteer-0.8.0b1.tar.gz` & `tmp/documenteer-0.8.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "documenteer-0.8.0b1.tar", last modified: Wed Feb  8 21:14:19 2023, max compression
+gzip compressed data, was "documenteer-0.8.0b2.tar", last modified: Wed Mar  1 15:51:31 2023, max compression
```

## Comparing `documenteer-0.8.0b1.tar` & `documenteer-0.8.0b2.tar`

### file list

```diff
@@ -1,255 +1,255 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.799534 documenteer-0.8.0b1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/SUPPORT.md
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.799534 documenteer-0.8.0b1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/workflows/ci-cron.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.npmrc
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.nvmrc
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.prettierrc.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.799534 documenteer-0.8.0b1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    28262 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/demo/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.799534 documenteer-0.8.0b1/demo/rst-technote/
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/demo/rst-technote/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/demo/rst-technote/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/demo/rst-technote/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/demo/rst-technote/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/demo/rst-technote/technote.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.799534 documenteer-0.8.0b1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/_rst_epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28262 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.803534 documenteer-0.8.0b1/docs/dev/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.803534 documenteer-0.8.0b1/docs/dev/api/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.conf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.ext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.requestsutils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.sphinxconfig.rst
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.sphinxext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.sphinxrunner.rst
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/documenteer.stackdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/html-templates.rst
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/release.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/theme-assets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/dev/theme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/documenteer.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.803534 documenteer-0.8.0b1/docs/guides/
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/badges.rst
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/configuration-preset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/diagrams.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/extend-conf-py.rst
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/organization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/pyproject-configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/rst-epilog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/tabsets.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/guides/toml-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.803534 documenteer-0.8.0b1/docs/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/build-overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/cpp-api-linking.rst
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/package-docs-cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/pipelines/stack-docs-cli.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.803534 documenteer-0.8.0b1/docs/sphinx-extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/autocppapi.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/autodocreset.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/docushare-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/jira-reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/lsst-pybtex-style.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/lssttasks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/package-toctree.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/sphinx-extensions/remote-code-block.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/docs/technotes/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/technotes/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/technotes/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/docs/technotes/refresh-lsst-bib.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/licenses/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/licenses/astropy-helpers.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/licenses/sphinx-issue.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/licenses/sphinx.txt
--rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-02-08 21:14:02.000000 documenteer-0.8.0b1/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/package.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/postcss.config.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/src/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/src/assets/rubin-technote/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/assets/rubin-technote/styles/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/_hacks.scss
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/_properties.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/assets/rubin-technote/styles/components/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/components/_index.scss
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/components/_version-info.scss
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/assets/rubin-technote/styles/rubin-technote.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer/assets/rsd-assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/rubin-favicon-transparent-32px.png
--rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/rubin-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/rubin-pydata-theme.css
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer/assets/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/scripts/rubin-technote.js
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/scripts/rubin-technote.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer/assets/styles/
--rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/styles/rubin-technote.css
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-02-08 21:14:04.000000 documenteer-0.8.0b1/src/documenteer/assets/styles/rubin-technote.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/bin/buildstackdocs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/bin/refreshlsstbib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10446 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/guide.py
--rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/pipelinespkg.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/technote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/conf/technotebeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/ext/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/ext/autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/ext/autodocreset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/requestsutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/sphinxconfig/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxconfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxconfig/stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxconfig/technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxconfig/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/sphinxext/
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lsstdocushare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.811534 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/configfieldlists.py
--rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/crossrefs.py
--rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/pyapisummary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/topiclists.py
--rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/remotecodeblock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxext/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/sphinxrunner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/stackdocs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/stackdocs/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
--rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/data/doxygen.defaults.conf
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/data/mainpage.dox
--rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/packagecli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/stackdocs/stackcli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/src/documenteer/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/templates/pydata/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/pydata/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/templates/technote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/technote/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/templates/technote/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/technote/components/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.815534 documenteer-0.8.0b1/src/documenteer/templates/technote/sections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/technote/sections/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/technote/sections/header-article.html
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/templates/technote/sections/sidebar-primary.html
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/src/documenteer/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.807534 documenteer-0.8.0b1/src/documenteer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-08 21:14:19.000000 documenteer-0.8.0b1/src/documenteer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/afw.doxygen.conf
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/doxygen.tag.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/tests/data/package_alpha/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/tests/data/package_alpha/doc/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/doc/_static/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/doc/_static/package_alpha/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/doc/doxygen.conf.in
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/doc/manifest.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/doc/package.alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/doc/package.alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/doc/package_alpha/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/doc/package_alpha/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/include/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_alpha/src/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_alpha/src/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/tests/data/package_beta/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/data/package_beta/doc/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/data/package_beta/doc/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.795534 documenteer-0.8.0b1/tests/roots/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:14:19.819534 documenteer-0.8.0b1/tests/roots/test-autocppapi/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/roots/test-autocppapi/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/roots/test-autocppapi/doxygen.tag.zip
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/roots/test-autocppapi/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_conf_toml.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_conf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_ext_autocppapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_packagemetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_refreshlsstbib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxconfig_stackconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxconfig_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_lsstdocushare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_lssttasks_taskutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_mockcoderefs.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_packagetoctree.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_sphinxext_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_stackdocs_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_stackdocs_doxygen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_stackdocs_doxygentag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_stackdocs_pkgdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_stackdocs_rootdiscovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tests/test_technoteconf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/tox.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-02-08 21:13:55.000000 documenteer-0.8.0b1/webpack.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/SUPPORT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/workflows/ci-cron.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.npmrc
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.nvmrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.prettierrc.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/demo/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.166154 documenteer-0.8.0b2/demo/rst-technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/demo/rst-technote/technote.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/_rst_epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28383 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/dev/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.170154 documenteer-0.8.0b2/docs/dev/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.conf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.ext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.requestsutils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxconfig.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxrunner.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/documenteer.stackdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/html-templates.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/release.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/theme-assets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/dev/theme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/documenteer.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.174154 documenteer-0.8.0b2/docs/guides/
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/badges.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/configuration-preset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/diagrams.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/extend-conf-py.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7899 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/organization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/pyproject-configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/rst-epilog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/tabsets.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/guides/toml-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.174154 documenteer-0.8.0b2/docs/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/build-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/cpp-api-linking.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/package-docs-cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/pipelines/stack-docs-cli.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/docs/sphinx-extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/autocppapi.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/autodocreset.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/docushare-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/jira-reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/lsst-pybtex-style.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/lssttasks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/package-toctree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/sphinx-extensions/remote-code-block.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/docs/technotes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/docs/technotes/refresh-lsst-bib.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/astropy-helpers.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/sphinx-issue.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13362 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/licenses/sphinx.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   212497 2023-03-01 15:51:14.000000 documenteer-0.8.0b2/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/postcss.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/assets/rubin-technote/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/src/assets/rubin-technote/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/_hacks.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/_properties.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.178154 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_global-breadcrumbs.scss
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_index.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/components/_version-info.scss
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/assets/rubin-technote/styles/rubin-technote.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon-transparent-32px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2369 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-pydata-theme.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer/assets/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)     7548 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-03-01 15:51:17.000000 documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/buildstackdocs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/bin/refreshlsstbib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15143 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10632 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/guide.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13979 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/pipelinespkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/technote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/conf/technotebeta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/ext/autodocreset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/requestsutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.186154 documenteer-0.8.0b2/src/documenteer/sphinxconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20527 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxconfig/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/sphinxext/
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4128 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lsstdocushare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39808 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/configfieldlists.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12373 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/crossrefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10419 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/pyapisummary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topiclists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5155 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7497 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5298 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/remotecodeblock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6132 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxext/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/sphinxrunner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.190154 documenteer-0.8.0b2/src/documenteer/stackdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/stackdocs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1063166 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   105749 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/doxygen.defaults.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/data/mainpage.dox
+-rw-r--r--   0 runner    (1001) docker     (123)    23844 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/packagecli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9948 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9741 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/stackdocs/stackcli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.158154 documenteer-0.8.0b2/src/documenteer/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/pydata/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/pydata/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/components/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.194154 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/header-article.html
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/templates/technote/sections/sidebar-primary.html
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/src/documenteer/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.182154 documenteer-0.8.0b2/src/documenteer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6975 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-01 15:51:31.000000 documenteer-0.8.0b2/src/documenteer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.198154 documenteer-0.8.0b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.198154 documenteer-0.8.0b2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/afw.doxygen.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/doxygen.tag.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_alpha/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/_static/package_alpha/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/doxygen.conf.in
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/manifest.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/package.alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/package.alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/doc/package_alpha/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/doc/package_alpha/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/include/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_alpha/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_alpha/src/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/data/package_beta/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/data/package_beta/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/data/package_beta/doc/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.162154 documenteer-0.8.0b2/tests/roots/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-01 15:51:31.202154 documenteer-0.8.0b2/tests/roots/test-autocppapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)   199942 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/doxygen.tag.zip
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/roots/test-autocppapi/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_conf_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_conf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_ext_autocppapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_packagemetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_refreshlsstbib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxconfig_stackconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxconfig_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_lsstdocushare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_lssttasks_taskutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_mockcoderefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_packagetoctree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_sphinxext_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_doxygen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_doxygentag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_pkgdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_stackdocs_rootdiscovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tests/test_technoteconf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-03-01 15:51:04.000000 documenteer-0.8.0b2/webpack.config.js
```

### Comparing `documenteer-0.8.0b1/.github/workflows/ci-cron.yaml` & `documenteer-0.8.0b2/.github/workflows/ci-cron.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/.github/workflows/ci.yaml` & `documenteer-0.8.0b2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/.gitignore` & `documenteer-0.8.0b2/.gitignore`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/.pre-commit-config.yaml` & `documenteer-0.8.0b2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/.vscode/tasks.json` & `documenteer-0.8.0b2/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/CHANGELOG.md` & `documenteer-0.8.0b2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Unreleased
 
 - Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
   These technotes are now themed with Rubin's modern branding.
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
+- Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-0.8.0b1/LICENSE` & `documenteer-0.8.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/PKG-INFO` & `documenteer-0.8.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.0b1
+Version: 0.8.0b2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-0.8.0b1/README.md` & `documenteer-0.8.0b2/README.md`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/demo/rst-technote/index.rst` & `documenteer-0.8.0b2/demo/rst-technote/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/Makefile` & `documenteer-0.8.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/_rst_epilog.rst` & `documenteer-0.8.0b2/docs/_rst_epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/changelog.md` & `documenteer-0.8.0b2/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 ## Unreleased
 
 - Add a new `documenteer.conf.technotebeta` configuration for [technote](https://technote.lsst.io)-based technotes.
   These technotes are now themed with Rubin's modern branding.
 - Drop support for Python 3.7.
 - Drop support for Sphinx versions earlier than 5.
+- Temporarily pin pydata-sphinx-theme < 0.13 on account of a change in logo path checking (affects user guide projects).
 
 ## 0.7.0 (2022-10-20)
 
 - Documenteer provides a new Sphinx configuration profile for general Rubin user guide projects, `documenteer.conf.guide`.
   This configuration profile features the new [pydata-sphinx-theme](https://pydata-sphinx-theme.readthedocs.io/en/stable/), with customizations based on design tokens from the [Rubin Style Dictionary](https://style-dictionary.lsst.io).
   Most metadata and Sphinx configurations can also be set through a `documenteer.toml` file, located alongside the standard Sphinx `conf.py` file.
   Install `documenteer[guide]` with `pip` to get the dependencies needed for this Sphinx configuration.
```

### Comparing `documenteer-0.8.0b1/docs/dev/api/documenteer.sphinxext.rst` & `documenteer-0.8.0b2/docs/dev/api/documenteer.sphinxext.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/dev/api/documenteer.stackdocs.rst` & `documenteer-0.8.0b2/docs/dev/api/documenteer.stackdocs.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/dev/development.rst` & `documenteer-0.8.0b2/docs/dev/development.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/dev/html-templates.rst` & `documenteer-0.8.0b2/docs/dev/html-templates.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/dev/release.rst` & `documenteer-0.8.0b2/docs/dev/release.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/dev/theme-assets.rst` & `documenteer-0.8.0b2/docs/dev/theme-assets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/documenteer.toml` & `documenteer-0.8.0b2/docs/documenteer.toml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/badges.rst` & `documenteer-0.8.0b2/docs/guides/badges.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/configuration.rst` & `documenteer-0.8.0b2/docs/guides/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/diagrams.rst` & `documenteer-0.8.0b2/docs/guides/diagrams.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/extend-conf-py.rst` & `documenteer-0.8.0b2/docs/guides/extend-conf-py.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/index.rst` & `documenteer-0.8.0b2/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/organization.rst` & `documenteer-0.8.0b2/docs/guides/organization.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/overview.rst` & `documenteer-0.8.0b2/docs/guides/overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/pyproject-configuration.rst` & `documenteer-0.8.0b2/docs/guides/pyproject-configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/rst-epilog.rst` & `documenteer-0.8.0b2/docs/guides/rst-epilog.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/tabsets.rst` & `documenteer-0.8.0b2/docs/guides/tabsets.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/guides/toml-reference.rst` & `documenteer-0.8.0b2/docs/guides/toml-reference.rst`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 .. _guide-project-base-url:
 
 base\_url
 ---------
 
 |optional| |py-auto|
 
-The root URL of the documentation project, used to set the `canonical URL link rel <https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel#attr-canonical>`__, which is valuable for search engines.
+The root URL of the documentation project, used to set the `canonical URL link rel <https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel>`__, which is valuable for search engines.
 
 .. code-block:: toml
 
    [project]
    base_url = "https://documenteer.lsst.io"
 
 copyright
```

### Comparing `documenteer-0.8.0b1/docs/index.rst` & `documenteer-0.8.0b2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/build-overview.rst` & `documenteer-0.8.0b2/docs/pipelines/build-overview.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/configuration.rst` & `documenteer-0.8.0b2/docs/pipelines/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/cpp-api-linking.rst` & `documenteer-0.8.0b2/docs/pipelines/cpp-api-linking.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/index.rst` & `documenteer-0.8.0b2/docs/pipelines/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/install.rst` & `documenteer-0.8.0b2/docs/pipelines/install.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/package-docs-cli.rst` & `documenteer-0.8.0b2/docs/pipelines/package-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/pipelines/stack-docs-cli.rst` & `documenteer-0.8.0b2/docs/pipelines/stack-docs-cli.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/autocppapi.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/autocppapi.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/autodocreset.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/autodocreset.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/docushare-reference.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/docushare-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/jira-reference.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/jira-reference.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/lsst-pybtex-style.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/lsst-pybtex-style.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/lssttasks.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/lssttasks.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/package-toctree.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/package-toctree.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/sphinx-extensions/remote-code-block.rst` & `documenteer-0.8.0b2/docs/sphinx-extensions/remote-code-block.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/technotes/configuration.rst` & `documenteer-0.8.0b2/docs/technotes/configuration.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/technotes/index.rst` & `documenteer-0.8.0b2/docs/technotes/index.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/docs/technotes/refresh-lsst-bib.rst` & `documenteer-0.8.0b2/docs/technotes/refresh-lsst-bib.rst`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/licenses/astropy-helpers.txt` & `documenteer-0.8.0b2/licenses/astropy-helpers.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/licenses/sphinx-issue.txt` & `documenteer-0.8.0b2/licenses/sphinx-issue.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/licenses/sphinx.txt` & `documenteer-0.8.0b2/licenses/sphinx.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/package-lock.json` & `documenteer-0.8.0b2/package-lock.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/package.json` & `documenteer-0.8.0b2/package.json`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/pyproject.toml` & `documenteer-0.8.0b2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     "types-PyYAML",
     "types-docutils",
     "types-mock",
 ]
 guide = [
     # Theme and extensions for Rubin user guide projects
     "sphinx_design",
-    "pydata-sphinx-theme>=0.10.0",
+    "pydata-sphinx-theme>=0.10.0,<0.13.0",
     "sphinx-autodoc-typehints",
     "sphinx-automodapi",
     "sphinx-copybutton",
     "sphinx-prompt",
     "myst-parser",
     "markdown-it-py[linkify]",
     "sphinxcontrib-mermaid",
```

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/favicon.ico` & `documenteer-0.8.0b2/src/documenteer/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg` & `documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-black-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg` & `documenteer-0.8.0b2/src/documenteer/assets/rsd-assets/rubin-imagotype-color-on-white-crop.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rubin-favicon-transparent-32px.png` & `documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon-transparent-32px.png`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rubin-favicon.svg` & `documenteer-0.8.0b2/src/documenteer/assets/rubin-favicon.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rubin-pydata-theme.css` & `documenteer-0.8.0b2/src/documenteer/assets/rubin-pydata-theme.css`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg` & `documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-dark.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/rubin-titlebar-imagotype-light.svg` & `documenteer-0.8.0b2/src/documenteer/assets/rubin-titlebar-imagotype-light.svg`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/scripts/rubin-technote.js` & `documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/scripts/rubin-technote.js.map` & `documenteer-0.8.0b2/src/documenteer/assets/scripts/rubin-technote.js.map`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/styles/rubin-technote.css` & `documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/assets/styles/rubin-technote.css.map` & `documenteer-0.8.0b2/src/documenteer/assets/styles/rubin-technote.css.map`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/bin/buildstackdocs.py` & `documenteer-0.8.0b2/src/documenteer/bin/buildstackdocs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/bin/refreshlsstbib.py` & `documenteer-0.8.0b2/src/documenteer/bin/refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/_toml.py` & `documenteer-0.8.0b2/src/documenteer/conf/_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/_utils.py` & `documenteer-0.8.0b2/src/documenteer/conf/_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/guide.py` & `documenteer-0.8.0b2/src/documenteer/conf/guide.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,14 +93,15 @@
     "napoleon_preprocess_types",
     "napoleon_type_aliases",
     "napoleon_attr_annotations",
     # MYST
     "myst_enable_extensions",
     # MERMAID
     "mermaid_output_format",
+    "mermaid_version",
     # OPENGRAPH
     "ogp_site_url",
     "ogp_site_name",
     "ogp_use_first_image",
 ]
 
 _conf = DocumenteerConfig.find_and_load()
@@ -344,14 +345,18 @@
 # https://mermaid-js.github.io/mermaid/#/
 # ============================================================================
 
 # The raw format renders the diagram client-side, and doesn't require a
 # Mermaid CLI installation
 mermaid_output_format = "raw"
 
+# Temporary workaround for not getting mermaid 10 successfully from unpkg
+# https://github.com/mgaitan/sphinxcontrib-mermaid/issues/110
+mermaid_version = "9.4.0"
+
 # ============================================================================
 # #OPENGRAPH OpenGraph diagram support
 # https://github.com/wpilibsuite/sphinxext-opengraph
 # https://ogp.me/
 # ============================================================================
 
 ogp_site_url = _conf.base_url
```

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/pipelines.py` & `documenteer-0.8.0b2/src/documenteer/conf/pipelines.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/pipelinespkg.py` & `documenteer-0.8.0b2/src/documenteer/conf/pipelinespkg.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/technote.py` & `documenteer-0.8.0b2/src/documenteer/conf/technote.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/conf/technotebeta.py` & `documenteer-0.8.0b2/src/documenteer/conf/technotebeta.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/ext/autocppapi.py` & `documenteer-0.8.0b2/src/documenteer/ext/autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/ext/autodocreset.py` & `documenteer-0.8.0b2/src/documenteer/ext/autodocreset.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/packagemetadata.py` & `documenteer-0.8.0b2/src/documenteer/packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/requestsutils.py` & `documenteer-0.8.0b2/src/documenteer/requestsutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxconfig/stackconf.py` & `documenteer-0.8.0b2/src/documenteer/sphinxconfig/stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxconfig/technoteconf.py` & `documenteer-0.8.0b2/src/documenteer/sphinxconfig/technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxconfig/utils.py` & `documenteer-0.8.0b2/src/documenteer/sphinxconfig/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/__init__.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/bibtex.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/bibtex.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/jira.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lsstdocushare.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/__init__.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/__init__.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/configfieldlists.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/configfieldlists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/crossrefs.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/crossrefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/pyapisummary.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/pyapisummary.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/taskutils.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/topiclists.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topiclists.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/lssttasks/topics.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/lssttasks/topics.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/mockcoderefs.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/packagetoctree.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/remotecodeblock.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/remotecodeblock.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxext/utils.py` & `documenteer-0.8.0b2/src/documenteer/sphinxext/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/sphinxrunner.py` & `documenteer-0.8.0b2/src/documenteer/sphinxrunner.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/build.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/build.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml` & `documenteer-0.8.0b2/src/documenteer/stackdocs/data/cppreference-doxygen-web.tag.xml`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/data/doxygen.defaults.conf` & `documenteer-0.8.0b2/src/documenteer/stackdocs/data/doxygen.defaults.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/doxygen.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/doxygentag.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/packagecli.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/packagecli.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/pkgdiscovery.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/rootdiscovery.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/stackdocs/stackcli.py` & `documenteer-0.8.0b2/src/documenteer/stackdocs/stackcli.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/templates/technote/sections/header-article.html` & `documenteer-0.8.0b2/src/documenteer/templates/technote/sections/header-article.html`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/utils.py` & `documenteer-0.8.0b2/src/documenteer/utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer/version.py` & `documenteer-0.8.0b2/src/documenteer/version.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer.egg-info/PKG-INFO` & `documenteer-0.8.0b2/src/documenteer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: documenteer
-Version: 0.8.0b1
+Version: 0.8.0b2
 Summary: Rubin Observatory / LSST Sphinx documentation tools, extensions, and configurations.
 License: The MIT License (MIT)
         
         Copyright (c) 2015-2022 Association of Universities for Research in Astronomy, Inc. (AURA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `documenteer-0.8.0b1/src/documenteer.egg-info/SOURCES.txt` & `documenteer-0.8.0b2/src/documenteer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/src/documenteer.egg-info/requires.txt` & `documenteer-0.8.0b2/src/documenteer.egg-info/requires.txt`

 * *Files 25% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 types-requests
 types-PyYAML
 types-docutils
 types-mock
 
 [guide]
 sphinx_design
-pydata-sphinx-theme>=0.10.0
+pydata-sphinx-theme<0.13.0,>=0.10.0
 sphinx-autodoc-typehints
 sphinx-automodapi
 sphinx-copybutton
 sphinx-prompt
 myst-parser
 markdown-it-py[linkify]
 sphinxcontrib-mermaid
```

### Comparing `documenteer-0.8.0b1/tests/conftest.py` & `documenteer-0.8.0b2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/data/afw.doxygen.conf` & `documenteer-0.8.0b2/tests/data/afw.doxygen.conf`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/data/doxygen.tag.zip` & `documenteer-0.8.0b2/tests/data/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/roots/test-autocppapi/conf.py` & `documenteer-0.8.0b2/tests/roots/test-autocppapi/conf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/roots/test-autocppapi/doxygen.tag.zip` & `documenteer-0.8.0b2/tests/roots/test-autocppapi/doxygen.tag.zip`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_conf_toml.py` & `documenteer-0.8.0b2/tests/test_conf_toml.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_conf_utils.py` & `documenteer-0.8.0b2/tests/test_conf_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_ext_autocppapi.py` & `documenteer-0.8.0b2/tests/test_ext_autocppapi.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_packagemetadata.py` & `documenteer-0.8.0b2/tests/test_packagemetadata.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_refreshlsstbib.py` & `documenteer-0.8.0b2/tests/test_refreshlsstbib.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxconfig_stackconf.py` & `documenteer-0.8.0b2/tests/test_sphinxconfig_stackconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxconfig_utils.py` & `documenteer-0.8.0b2/tests/test_sphinxconfig_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_jira.py` & `documenteer-0.8.0b2/tests/test_sphinxext_jira.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_lsstdocushare.py` & `documenteer-0.8.0b2/tests/test_sphinxext_lsstdocushare.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_lssttasks_taskutils.py` & `documenteer-0.8.0b2/tests/test_sphinxext_lssttasks_taskutils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_mockcoderefs.py` & `documenteer-0.8.0b2/tests/test_sphinxext_mockcoderefs.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_packagetoctree.py` & `documenteer-0.8.0b2/tests/test_sphinxext_packagetoctree.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_sphinxext_utils.py` & `documenteer-0.8.0b2/tests/test_sphinxext_utils.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_stackdocs_build.py` & `documenteer-0.8.0b2/tests/test_stackdocs_build.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_stackdocs_doxygen.py` & `documenteer-0.8.0b2/tests/test_stackdocs_doxygen.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_stackdocs_doxygentag.py` & `documenteer-0.8.0b2/tests/test_stackdocs_doxygentag.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_stackdocs_pkgdiscovery.py` & `documenteer-0.8.0b2/tests/test_stackdocs_pkgdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_stackdocs_rootdiscovery.py` & `documenteer-0.8.0b2/tests/test_stackdocs_rootdiscovery.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tests/test_technoteconf.py` & `documenteer-0.8.0b2/tests/test_technoteconf.py`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/tox.ini` & `documenteer-0.8.0b2/tox.ini`

 * *Files identical despite different names*

### Comparing `documenteer-0.8.0b1/webpack.config.js` & `documenteer-0.8.0b2/webpack.config.js`

 * *Files identical despite different names*

