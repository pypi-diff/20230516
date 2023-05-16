# Comparing `tmp/adafruit-circuitpython-bh1750-1.1.6.tar.gz` & `tmp/adafruit-circuitpython-bh1750-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bh1750-1.1.6.tar", last modified: Mon Nov 28 18:15:33 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bh1750-1.1.7.tar", last modified: Tue May 16 17:46:33 2023, max compression
```

## Comparing `adafruit-circuitpython-bh1750-1.1.6.tar` & `adafruit-circuitpython-bh1750-1.1.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.649808 adafruit-circuitpython-bh1750-1.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.649808 adafruit-circuitpython-bh1750-1.1.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.649808 adafruit-circuitpython-bh1750-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6140 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.649808 adafruit-circuitpython-bh1750-1.1.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2837 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     7005 2022-11-28 18:15:25.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_bh1750.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3584 2022-11-28 18:15:33.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      957 2022-11-28 18:15:33.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:15:33.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:15:33.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:15:33.000000 adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      320 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5882 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      412 2022-11-28 18:15:25.000000 adafruit-circuitpython-bh1750-1.1.6/examples/bh1750_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1186 2022-11-28 18:15:25.000000 adafruit-circuitpython-bh1750-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:15:15.000000 adafruit-circuitpython-bh1750-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:15:33.653807 adafruit-circuitpython-bh1750-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.945158 adafruit-circuitpython-bh1750-1.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_bh1750.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/examples/bh1750_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/setup.cfg
```

### Comparing `adafruit-circuitpython-bh1750-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/.gitignore` & `adafruit-circuitpython-bh1750-1.1.7/.gitignore`

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

### Comparing `adafruit-circuitpython-bh1750-1.1.6/.pre-commit-config.yaml` & `adafruit-circuitpython-bh1750-1.1.7/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-bh1750-1.1.6/.pylintrc` & `adafruit-circuitpython-bh1750-1.1.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bh1750-1.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/LICENSE` & `adafruit-circuitpython-bh1750-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bh1750-1.1.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/LICENSES/MIT.txt` & `adafruit-circuitpython-bh1750-1.1.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bh1750-1.1.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/PKG-INFO` & `adafruit-circuitpython-bh1750-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bh1750
-Version: 1.1.6
+Version: 1.1.7
 Summary: CircuitPython library for use with the Adafruit BH1750 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BH1750
 Keywords: adafruit,blinka,circuitpython,micropython,bh1750
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bh1750-1.1.6/README.rst` & `adafruit-circuitpython-bh1750-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/adafruit_bh1750.py` & `adafruit-circuitpython-bh1750-1.1.7/adafruit_bh1750.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   https://circuitpython.org/downloads
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # imports
 
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BH1750.git"
 
 from time import sleep
 from struct import unpack_from
 from micropython import const
 from adafruit_bus_device import i2c_device
 
@@ -105,15 +105,14 @@
     """
 
     def __init__(self, num_bits: int, lowest_bit: int) -> None:
         self._bit_mask = ((1 << num_bits) - 1) << lowest_bit
         self._lowest_bit = lowest_bit
 
     def __get__(self, obj: Optional["BH1750"], objtype: Type["BH1750"]) -> int:
-
         return (obj._settings & self._bit_mask) >> self._lowest_bit
 
     def __set__(self, obj: "BH1750", value: int) -> None:
         # shift the value over to the right spot
         value <<= self._lowest_bit
         settings = obj._settings
 
@@ -186,15 +185,14 @@
 
     """
 
     mode = RWBitfields(2, 4)
     resolution = RWBitfields(2, 0)
 
     def __init__(self, i2c: I2C, address: int = _BH1750_DEFAULT_ADDRESS) -> None:
-
         self.i2c_device = i2c_device.I2CDevice(i2c, address)
         self._buffer = bytearray(2)
         self._settings_byte = 0
 
         self.initialize()
 
     def initialize(self) -> None:
@@ -210,15 +208,14 @@
     def _settings(self, value: int) -> None:
         self._settings_byte = value
         self._write(self._settings_byte)
         sleep(0.180)  # worse case time to take a new measurement
 
     @property
     def _raw_reading(self) -> int:
-
         self._buffer[0] = 0
         self._buffer[1] = 0
 
         with self.i2c_device as i2c:
             i2c.readinto(self._buffer)
 
         return unpack_from(">H", self._buffer)[0]
```

### Comparing `adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/PKG-INFO` & `adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bh1750
-Version: 1.1.6
+Version: 1.1.7
 Summary: CircuitPython library for use with the Adafruit BH1750 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BH1750
 Keywords: adafruit,blinka,circuitpython,micropython,bh1750
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bh1750-1.1.6/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt` & `adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/docs/_static/favicon.ico` & `adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/docs/conf.py` & `adafruit-circuitpython-bh1750-1.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/docs/index.rst` & `adafruit-circuitpython-bh1750-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.6/pyproject.toml` & `adafruit-circuitpython-bh1750-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bh1750"
 description = "CircuitPython library for use with the Adafruit BH1750 breakout"
-version = "1.1.6"
+version = "1.1.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BH1750"}
 keywords = [
     "adafruit",
```

