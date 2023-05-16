# Comparing `tmp/depthcharge-ms-0.2.1.tar.gz` & `tmp/depthcharge-ms-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depthcharge-ms-0.2.1.tar", last modified: Sun May 14 05:03:38 2023, max compression
+gzip compressed data, was "depthcharge-ms-0.2.2.tar", last modified: Tue May 16 05:54:27 2023, max compression
```

## Comparing `depthcharge-ms-0.2.1.tar` & `depthcharge-ms-0.2.2.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.172362 depthcharge-ms-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/data/
--rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mgf
--rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzML
--rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzXML
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/components/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/feedforward.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/components/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.176362 depthcharge-ms-0.2.1/depthcharge/data/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/data/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/depthcharge/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-14 05:03:38.000000 depthcharge-ms-0.2.1/depthcharge_ms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/icon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    24683 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/logo-dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/static/logo-light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/test_components/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 05:03:38.180362 depthcharge-ms-0.2.1/tests/unit_tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_masses.py
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-14 05:03:21.000000 depthcharge-ms-0.2.1/tests/unit_tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.417820 depthcharge-ms-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.417820 depthcharge-ms-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4974 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    12882 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mgf
+-rw-r--r--   0 runner    (1001) docker     (123)   333865 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzML
+-rw-r--r--   0 runner    (1001) docker     (123)    67798 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzXML
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6700 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/feedforward.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15540 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/components/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9562 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/data/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/depthcharge/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 05:54:27.000000 depthcharge-ms-0.2.2/depthcharge_ms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15364 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/icon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    24683 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/logo-dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25343 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/static/logo-light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.421820 depthcharge-ms-0.2.2/tests/unit_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/tests/unit_tests/test_components/
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 05:54:27.425820 depthcharge-ms-0.2.2/tests/unit_tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-16 05:54:12.000000 depthcharge-ms-0.2.2/tests/unit_tests/test_version.py
```

### Comparing `depthcharge-ms-0.2.1/.github/workflows/lint.yml` & `depthcharge-ms-0.2.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/.github/workflows/publish.yml` & `depthcharge-ms-0.2.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/.github/workflows/tests.yml` & `depthcharge-ms-0.2.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/CHANGELOG.md` & `depthcharge-ms-0.2.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [v0.2.2] - 2023-05-15
+### Fixed
+- Fixed retrieving version information.
+
 ## [v0.2.1] - 2023-05-13
 ### Changed
 - Change target mask from float to boolean.
 - Log the number spectra that are skipped due to an invalid precursor charge.
 
 ## [v0.2.0] - 2023-03-06
 ### Breaking Changes
```

### Comparing `depthcharge-ms-0.2.1/CODE_OF_CONDUCT.md` & `depthcharge-ms-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/CONTRIBUTING.md` & `depthcharge-ms-0.2.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/LICENSE` & `depthcharge-ms-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/PKG-INFO` & `depthcharge-ms-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.2.1
+Version: 0.2.2
 Summary: A deep learning toolkit for proteomics
 Home-page: https://github.com/wfondrie/depthcharge
 Author: William E. Fondrie
 Author-email: fondriew@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/wfondrie/depthcharge/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.1 Summary: A deep
+Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.2 Summary: A deep
 learning toolkit for proteomics Home-page: https://github.com/wfondrie/
 depthcharge Author: William E. Fondrie Author-email: fondriew@gmail.com
 License: Apache 2.0 Project-URL: Documentation, https://
 depthcharge.readthedocs.io Project-URL: Bug Tracker, https://github.com/
 wfondrie/depthcharge/issues Project-URL: Discussion Board, https://github.com/
 wfondrie/depthcharge/discussions Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `depthcharge-ms-0.2.1/README.md` & `depthcharge-ms-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mgf` & `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mgf`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzML` & `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/data/TMT10-Trial-8.mzXML` & `depthcharge-ms-0.2.2/data/TMT10-Trial-8.mzXML`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/components/encoders.py` & `depthcharge-ms-0.2.2/depthcharge/components/encoders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/components/feedforward.py` & `depthcharge-ms-0.2.2/depthcharge/components/feedforward.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/components/transformers.py` & `depthcharge-ms-0.2.2/depthcharge/components/transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/data/datasets.py` & `depthcharge-ms-0.2.2/depthcharge/data/datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/data/hdf5.py` & `depthcharge-ms-0.2.2/depthcharge/data/hdf5.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/data/parsers.py` & `depthcharge-ms-0.2.2/depthcharge/data/parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/data/preprocessing.py` & `depthcharge-ms-0.2.2/depthcharge/data/preprocessing.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/masses.py` & `depthcharge-ms-0.2.2/depthcharge/masses.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/similarity.py` & `depthcharge-ms-0.2.2/depthcharge/similarity.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge/utils.py` & `depthcharge-ms-0.2.2/depthcharge/utils.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/depthcharge_ms.egg-info/PKG-INFO` & `depthcharge-ms-0.2.2/depthcharge_ms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: depthcharge-ms
-Version: 0.2.1
+Version: 0.2.2
 Summary: A deep learning toolkit for proteomics
 Home-page: https://github.com/wfondrie/depthcharge
 Author: William E. Fondrie
 Author-email: fondriew@gmail.com
 License: Apache 2.0
 Project-URL: Documentation, https://depthcharge.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/wfondrie/depthcharge/issues
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.1 Summary: A deep
+Metadata-Version: 2.1 Name: depthcharge-ms Version: 0.2.2 Summary: A deep
 learning toolkit for proteomics Home-page: https://github.com/wfondrie/
 depthcharge Author: William E. Fondrie Author-email: fondriew@gmail.com
 License: Apache 2.0 Project-URL: Documentation, https://
 depthcharge.readthedocs.io Project-URL: Bug Tracker, https://github.com/
 wfondrie/depthcharge/issues Project-URL: Discussion Board, https://github.com/
 wfondrie/depthcharge/discussions Classifier: Programming Language :: Python ::
 3 Classifier: License :: OSI Approved :: Apache Software License Classifier:
```

### Comparing `depthcharge-ms-0.2.1/depthcharge_ms.egg-info/SOURCES.txt` & `depthcharge-ms-0.2.2/depthcharge_ms.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,13 +41,14 @@
 docs/stylesheets/extra.css
 static/icon.svg
 static/logo-dark.png
 static/logo-light.png
 tests/conftest.py
 tests/unit_tests/test_masses.py
 tests/unit_tests/test_utils.py
+tests/unit_tests/test_version.py
 tests/unit_tests/test_components/test_encoders.py
 tests/unit_tests/test_components/test_transformers.py
 tests/unit_tests/test_data/test_datasets.py
 tests/unit_tests/test_data/test_index.py
 tests/unit_tests/test_data/test_loaders.py
 tests/unit_tests/test_data/test_parsers.py
```

### Comparing `depthcharge-ms-0.2.1/docs/README.md` & `depthcharge-ms-0.2.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/mkdocs.yml` & `depthcharge-ms-0.2.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/pyproject.toml` & `depthcharge-ms-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/setup.cfg` & `depthcharge-ms-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/static/icon.svg` & `depthcharge-ms-0.2.2/static/icon.svg`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/static/logo-dark.png` & `depthcharge-ms-0.2.2/static/logo-dark.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/static/logo-light.png` & `depthcharge-ms-0.2.2/static/logo-light.png`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/conftest.py` & `depthcharge-ms-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_encoders.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_encoders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_components/test_transformers.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_components/test_transformers.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_datasets.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_datasets.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_index.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_index.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_loaders.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_loaders.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_data/test_parsers.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_data/test_parsers.py`

 * *Files identical despite different names*

### Comparing `depthcharge-ms-0.2.1/tests/unit_tests/test_masses.py` & `depthcharge-ms-0.2.2/tests/unit_tests/test_masses.py`

 * *Files identical despite different names*

