# Comparing `tmp/adafruit-circuitpython-datetime-1.2.3.tar.gz` & `tmp/adafruit-circuitpython-datetime-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-datetime-1.2.3.tar", last modified: Tue Nov 15 17:25:38 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-datetime-1.2.4.tar", last modified: Tue May 16 17:49:05 2023, max compression
```

## Comparing `adafruit-circuitpython-datetime-1.2.3.tar` & `adafruit-circuitpython-datetime-1.2.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.199875 adafruit-circuitpython-datetime-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13925 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3822 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4581 2022-11-15 17:25:38.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-11-15 17:25:38.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 17:25:38.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 17:25:38.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-15 17:25:38.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    60298 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/adafruit_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5772 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      975 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1443 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/examples/datetime_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/examples/datetime_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/examples/datetime_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-15 17:25:21.000000 adafruit-circuitpython-datetime-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:25:38.203875 adafruit-circuitpython-datetime-1.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    18478 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (121)    49197 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (121)    14920 2022-11-15 17:25:30.000000 adafruit-circuitpython-datetime-1.2.3/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.987288 adafruit-circuitpython-datetime-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_time.py
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/.gitignore` & `adafruit-circuitpython-datetime-1.2.4/.gitignore`

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

### Comparing `adafruit-circuitpython-datetime-1.2.3/.pre-commit-config.yaml` & `adafruit-circuitpython-datetime-1.2.4/.pre-commit-config.yaml`

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
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/.pylintrc` & `adafruit-circuitpython-datetime-1.2.4/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-datetime-1.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/LICENSE` & `adafruit-circuitpython-datetime-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-datetime-1.2.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/LICENSES/MIT.txt` & `adafruit-circuitpython-datetime-1.2.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/LICENSES/Python-2.0.txt` & `adafruit-circuitpython-datetime-1.2.4/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-datetime-1.2.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/PKG-INFO` & `adafruit-circuitpython-datetime-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-datetime
-Version: 1.2.3
+Version: 1.2.4
 Summary: Subset of CPython datetime module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_datetime
 Keywords: adafruit,blinka,circuitpython,micropython,datetime,date,time,timedelta,tzinfo,timezone
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/README.rst` & `adafruit-circuitpython-datetime-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/PKG-INFO` & `adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-datetime
-Version: 1.2.3
+Version: 1.2.4
 Summary: Subset of CPython datetime module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_datetime
 Keywords: adafruit,blinka,circuitpython,micropython,datetime,date,time,timedelta,tzinfo,timezone
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/adafruit_circuitpython_datetime.egg-info/SOURCES.txt` & `adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/adafruit_datetime.py` & `adafruit-circuitpython-datetime-1.2.4/adafruit_datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from micropython import const
 
 try:
     from typing import Any, Union, Optional, Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DateTime.git"
 
 # Constants
 MINYEAR = const(1)
 MAXYEAR = const(9999)
 _MAXORDINAL = const(3652059)
 _DI400Y = const(146097)
@@ -66,14 +66,15 @@
     "Nov",
     "Dec",
 )
 _DAYNAMES = (None, "Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun")
 
 _INVALID_ISO_ERROR = "Invalid isoformat string: '{}'"
 
+
 # Utility functions - universal
 def _cmp(obj_x: Any, obj_y: Any) -> int:
     return 0 if obj_x == obj_y else 1 if obj_x > obj_y else -1
 
 
 def _cmperror(
     obj_x: Union["datetime", "timedelta"], obj_y: Union["datetime", "timedelta"]
@@ -327,15 +328,14 @@
         seconds: int = 0,
         microseconds: int = 0,
         milliseconds: int = 0,
         minutes: int = 0,
         hours: int = 0,
         weeks: int = 0,
     ) -> "timedelta":
-
         # Check that all inputs are ints or floats.
         if not all(
             isinstance(i, (int, float))
             for i in [days, seconds, microseconds, milliseconds, minutes, hours, weeks]
         ):
             raise TypeError("Kwargs to this function must be int or float.")
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/docs/_static/favicon.ico` & `adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/docs/conf.py` & `adafruit-circuitpython-datetime-1.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/docs/index.rst` & `adafruit-circuitpython-datetime-1.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/examples/datetime_simpletest.py` & `adafruit-circuitpython-datetime-1.2.4/examples/datetime_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/examples/datetime_time.py` & `adafruit-circuitpython-datetime-1.2.4/examples/datetime_time.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/examples/datetime_timedelta.py` & `adafruit-circuitpython-datetime-1.2.4/examples/datetime_timedelta.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/pyproject.toml` & `adafruit-circuitpython-datetime-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-datetime"
 description = "Subset of CPython datetime module"
-version = "1.2.3"
+version = "1.2.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_datetime"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-datetime-1.2.3/tests/test_date.py` & `adafruit-circuitpython-datetime-1.2.4/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/tests/test_datetime.py` & `adafruit-circuitpython-datetime-1.2.4/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.3/tests/test_time.py` & `adafruit-circuitpython-datetime-1.2.4/tests/test_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         self.assertRaises(TypeError, lambda: () < me)
         self.assertRaises(TypeError, lambda: () <= me)
         self.assertRaises(TypeError, lambda: () > me)
         self.assertRaises(TypeError, lambda: () >= me)
 
 
 class TestTime(HarmlessMixedComparison, unittest.TestCase):
-
     theclass = cpy_time
     theclass_cpython = cpython_time
 
     def test_basic_attributes(self):
         t = self.theclass(12, 0)
         t2 = self.theclass_cpython(12, 0)
         # Check adafruit_datetime module
```

