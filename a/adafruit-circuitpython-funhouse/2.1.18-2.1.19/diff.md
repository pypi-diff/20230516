# Comparing `tmp/adafruit-circuitpython-funhouse-2.1.18.tar.gz` & `tmp/adafruit-circuitpython-funhouse-2.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-funhouse-2.1.18.tar", last modified: Fri Aug 26 02:46:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-funhouse-2.1.19.tar", last modified: Tue May 16 17:54:10 2023, max compression
```

## Comparing `adafruit-circuitpython-funhouse-2.1.18.tar` & `adafruit-circuitpython-funhouse-2.1.19.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.959293 adafruit-circuitpython-funhouse-2.1.18/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.951293 adafruit-circuitpython-funhouse-2.1.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6306 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6306 2022-08-26 02:46:36.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1112 2022-08-26 02:46:36.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:46:36.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-08-26 02:46:36.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-08-26 02:46:36.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/
--rwxr-xr-x   0 runner    (1001) docker     (121)     4451 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1835 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7268 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/network.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     6960 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      440 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6025 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     2221 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:46:36.955293 adafruit-circuitpython-funhouse-2.1.18/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)     2507 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_adafruit_io_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (121)     3383 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1506 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_temperature_logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1199 2022-08-26 02:46:28.000000 adafruit-circuitpython-funhouse-2.1.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-26 02:46:20.000000 adafruit-circuitpython-funhouse-2.1.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:46:36.959293 adafruit-circuitpython-funhouse-2.1.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4450 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7268 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6960 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_adafruit_io_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1506 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_temperature_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/setup.cfg
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/.gitignore` & `adafruit-circuitpython-funhouse-2.1.19/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/.pre-commit-config.yaml` & `adafruit-circuitpython-funhouse-2.1.19/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/.pylintrc` & `adafruit-circuitpython-funhouse-2.1.19/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-funhouse-2.1.19/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/LICENSE` & `adafruit-circuitpython-funhouse-2.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-funhouse-2.1.19/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/LICENSES/MIT.txt` & `adafruit-circuitpython-funhouse-2.1.19/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/LICENSES/Unlicense.txt` & `adafruit-circuitpython-funhouse-2.1.19/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/PKG-INFO` & `adafruit-circuitpython-funhouse-2.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-funhouse
-Version: 2.1.18
+Version: 2.1.19
 Summary: Helper library for the FunHouse board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FunHouse
 Keywords: adafruit,funhouse,microcontroller,sensors,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/README.rst` & `adafruit-circuitpython-funhouse-2.1.19/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/PKG-INFO` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-funhouse
-Version: 2.1.18
+Version: 2.1.19
 Summary: Helper library for the FunHouse board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FunHouse
 Keywords: adafruit,funhouse,microcontroller,sensors,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 README.rst.license
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_funhouse.egg-info/PKG-INFO
 adafruit_circuitpython_funhouse.egg-info/SOURCES.txt
 adafruit_circuitpython_funhouse.egg-info/dependency_links.txt
 adafruit_circuitpython_funhouse.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/__init__.py` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from typing import Optional, Dict, Union, Callable, Sequence, List
     from adafruit_dotstar import DotStar
 except ImportError:
     pass
 
-__version__ = "2.1.18"
+__version__ = "2.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class FunHouse(PortalBase):
     """Class representing the Adafruit FunHouse.
 
     :param url: The URL of your data source. Defaults to ``None``.
@@ -78,15 +78,14 @@
         default_bg: int = 0,
         status_dotstar: Optional[DotStar] = None,
         json_transform: Optional[Union[Callable, List[Callable]]] = None,
         rotation: int = 270,
         scale: int = 1,
         debug: bool = False,
     ) -> None:
-
         network = Network(
             status_dotstar=status_dotstar,
             extract_values=False,
             debug=debug,
         )
 
         graphics = Graphics(
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/graphics.py` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * Adafruit's PortalBase library: https://github.com/adafruit/Adafruit_CircuitPython_PortalBase
 
 """
 
 import board
 from adafruit_portalbase.graphics import GraphicsBase
 
-__version__ = "2.1.18"
+__version__ = "2.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the FunHouse Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/network.py` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Optional, Union, Callable
     from adafruit_dotstar import DotStar
 except ImportError:
     pass
 
-__version__ = "2.1.18"
+__version__ = "2.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 IO_MQTT_BROKER = "io.adafruit.com"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit FunHouse.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/adafruit_funhouse/peripherals.py` & `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/peripherals.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import adafruit_dotstar
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "2.1.18"
+__version__ = "2.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the FunHouse Library
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/docs/_static/favicon.ico` & `adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/docs/conf.py` & `adafruit-circuitpython-funhouse-2.1.19/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/docs/examples.rst` & `adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/docs/index.rst` & `adafruit-circuitpython-funhouse-2.1.19/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_adafruit_io_mqtt.py` & `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_adafruit_io_mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # SPDX-License-Identifier: MIT
 import time
 from adafruit_funhouse import FunHouse
 
 funhouse = FunHouse(default_bg=None)
 funhouse.peripherals.set_dotstars(0x800000, 0x808000, 0x008000, 0x000080, 0x800080)
 
+
 # pylint: disable=unused-argument
 def connected(client):
     print("Connected to Adafruit IO! Subscribing...")
     client.subscribe("buzzer")
     client.subscribe("neopixels")
```

### Comparing `adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_simpletest.py` & `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/examples/funhouse_temperature_logger.py` & `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_temperature_logger.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.18/pyproject.toml` & `adafruit-circuitpython-funhouse-2.1.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-funhouse"
 description = "Helper library for the FunHouse board"
-version = "2.1.18"
+version = "2.1.19"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse"}
 keywords = [
     "adafruit",
```

