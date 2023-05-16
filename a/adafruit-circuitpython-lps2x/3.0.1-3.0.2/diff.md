# Comparing `tmp/adafruit-circuitpython-lps2x-3.0.1.tar.gz` & `tmp/adafruit-circuitpython-lps2x-3.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lps2x-3.0.1.tar", last modified: Mon Nov 28 18:11:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-lps2x-3.0.2.tar", last modified: Tue May 16 17:58:47 2023, max compression
```

## Comparing `adafruit-circuitpython-lps2x-3.0.1.tar` & `adafruit-circuitpython-lps2x-3.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.731056 adafruit-circuitpython-lps2x-3.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.731056 adafruit-circuitpython-lps2x-3.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2966 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3733 2022-11-28 18:11:08.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2022-11-28 18:11:08.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:11:08.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:11:08.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-28 18:11:08.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11347 2022-11-28 18:10:58.000000 adafruit-circuitpython-lps2x-3.0.1/adafruit_lps2x.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      315 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5891 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1234 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      547 2022-11-28 18:10:58.000000 adafruit-circuitpython-lps2x-3.0.1/examples/lps2x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1240 2022-11-28 18:10:58.000000 adafruit-circuitpython-lps2x-3.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:10:41.000000 adafruit-circuitpython-lps2x-3.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:11:08.735056 adafruit-circuitpython-lps2x-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_lps2x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/examples/lps2x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-lps2x-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/.gitignore` & `adafruit-circuitpython-lps2x-3.0.2/.gitignore`

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

### Comparing `adafruit-circuitpython-lps2x-3.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-lps2x-3.0.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-lps2x-3.0.1/.pylintrc` & `adafruit-circuitpython-lps2x-3.0.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lps2x-3.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/LICENSE` & `adafruit-circuitpython-lps2x-3.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lps2x-3.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-lps2x-3.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lps2x-3.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/PKG-INFO` & `adafruit-circuitpython-lps2x-3.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lps2x
-Version: 3.0.1
+Version: 3.0.2
 Summary: Library for the ST LPS2x family of pressure sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LPS2x
 Keywords: adafruit,blinka,circuitpython,micropython,lps2x,LPS25,LPS,pressure,MEMS,barometric
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lps2x-3.0.1/README.rst` & `adafruit-circuitpython-lps2x-3.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/PKG-INFO` & `adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lps2x
-Version: 3.0.1
+Version: 3.0.2
 Summary: Library for the ST LPS2x family of pressure sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LPS2x
 Keywords: adafruit,blinka,circuitpython,micropython,lps2x,LPS25,LPS,pressure,MEMS,barometric
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lps2x-3.0.1/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt` & `adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/adafruit_lps2x.py` & `adafruit-circuitpython-lps2x-3.0.2/adafruit_lps2x.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     https://circuitpythohn.org/downloads
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
-__version__ = "3.0.1"
+__version__ = "3.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LPS2X.git"
 from time import sleep
 from micropython import const
 import adafruit_bus_device.i2c_device as i2cdevice
 from adafruit_register.i2c_struct import ROUnaryStruct
 from adafruit_register.i2c_bits import RWBits, ROBits
 from adafruit_register.i2c_bit import RWBit
@@ -217,15 +217,14 @@
 
     enabled = RWBit(_LPS25_CTRL_REG1, 7)
     """Controls the power down state of the sensor. Setting to `False` will shut the sensor down"""
     _reset = RWBit(_LPS25_CTRL_REG2, 2)
     _data_rate = RWBits(3, _LPS25_CTRL_REG1, 4)
 
     def __init__(self, i2c_bus: I2C, address: int = _LPS2X_DEFAULT_ADDRESS) -> None:
-
         Rate.add_values(
             (
                 ("LPS25_RATE_ONE_SHOT", 0, 0, None),
                 ("LPS25_RATE_1_HZ", 1, 1, None),
                 ("LPS25_RATE_7_HZ", 2, 7, None),
                 ("LPS25_RATE_12_5_HZ", 3, 12.5, None),
                 ("LPS25_RATE_25_HZ", 4, 25, None),
```

### Comparing `adafruit-circuitpython-lps2x-3.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/docs/conf.py` & `adafruit-circuitpython-lps2x-3.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/docs/index.rst` & `adafruit-circuitpython-lps2x-3.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/examples/lps2x_simpletest.py` & `adafruit-circuitpython-lps2x-3.0.2/examples/lps2x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.1/pyproject.toml` & `adafruit-circuitpython-lps2x-3.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lps2x"
 description = "Library for the ST LPS2x family of pressure sensors"
-version = "3.0.1"
+version = "3.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LPS2x"}
 keywords = [
     "adafruit",
```

