# Comparing `tmp/adafruit-circuitpython-24lc32-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-24lc32-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-24lc32-1.0.8.tar", last modified: Mon Nov 28 18:16:58 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-24lc32-1.0.9.tar", last modified: Tue May 16 17:42:27 2023, max compression
```

## Comparing `adafruit-circuitpython-24lc32-1.0.8.tar` & `adafruit-circuitpython-24lc32-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.088851 adafruit-circuitpython-24lc32-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.088851 adafruit-circuitpython-24lc32-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.088851 adafruit-circuitpython-24lc32-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.088851 adafruit-circuitpython-24lc32-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4378 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3612 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)    10649 2022-11-28 18:16:49.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_24lc32.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.088851 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4378 2022-11-28 18:16:58.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      957 2022-11-28 18:16:58.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:16:58.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:16:58.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:16:58.000000 adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     6072 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1054 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      185 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      469 2022-11-28 18:16:49.000000 adafruit-circuitpython-24lc32-1.0.8/examples/24lc32_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1226 2022-11-28 18:16:49.000000 adafruit-circuitpython-24lc32-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:16:38.000000 adafruit-circuitpython-24lc32-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:16:58.092851 adafruit-circuitpython-24lc32-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.017909 adafruit-circuitpython-24lc32-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.017909 adafruit-circuitpython-24lc32-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.017909 adafruit-circuitpython-24lc32-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.017909 adafruit-circuitpython-24lc32-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-05-16 17:42:19.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_24lc32.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-05-16 17:42:26.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 17:42:27.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:42:26.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:42:26.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:42:26.000000 adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-16 17:42:19.000000 adafruit-circuitpython-24lc32-1.0.9/examples/24lc32_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-16 17:42:19.000000 adafruit-circuitpython-24lc32-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:42:11.000000 adafruit-circuitpython-24lc32-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:42:27.021909 adafruit-circuitpython-24lc32-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-24lc32-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-24lc32-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/.gitignore` & `adafruit-circuitpython-24lc32-1.0.9/.gitignore`

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

### Comparing `adafruit-circuitpython-24lc32-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-24lc32-1.0.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-24lc32-1.0.8/.pylintrc` & `adafruit-circuitpython-24lc32-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-24lc32-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/LICENSE` & `adafruit-circuitpython-24lc32-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-24lc32-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-24lc32-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-24lc32-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/PKG-INFO` & `adafruit-circuitpython-24lc32-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-24lc32
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for Adafruit 24LC32 I2C EEPROM Breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_24LC32.git
 Keywords: adafruit,blinka,circuitpython,micropython,24lc32,EEPROM,memory,nvm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-24lc32-1.0.8/README.rst` & `adafruit-circuitpython-24lc32-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/adafruit_24lc32.py` & `adafruit-circuitpython-24lc32-1.0.9/adafruit_24lc32.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 try:
     from typing import Optional, Union, Sequence
     from digitalio import DigitalInOut
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_24LC32.git"
 
 _MAX_SIZE_I2C = const(0x1000)
 
 
 class EEPROM:
     """
@@ -250,15 +250,14 @@
 
     def _write(
         self,
         start_address: int,
         data: Union[int, Sequence[int]],
         wraparound: bool = False,
     ) -> None:
-
         # Decided against using the chip's "Page Write", since that would require
         # doubling the memory usage by creating a buffer that includes the passed
         # in data so that it can be sent all in one `i2c.write`. The single-write
         # method is slower, and forces us to handle wraparound, but I feel this
         # is a better tradeoff for limiting the memory required for large writes.
         buffer = bytearray(3)
         if not isinstance(data, int):
```

### Comparing `adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/PKG-INFO` & `adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-24lc32
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython driver for Adafruit 24LC32 I2C EEPROM Breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_24LC32.git
 Keywords: adafruit,blinka,circuitpython,micropython,24lc32,EEPROM,memory,nvm
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-24lc32-1.0.8/adafruit_circuitpython_24lc32.egg-info/SOURCES.txt` & `adafruit-circuitpython-24lc32-1.0.9/adafruit_circuitpython_24lc32.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-24lc32-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/docs/conf.py` & `adafruit-circuitpython-24lc32-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/docs/index.rst` & `adafruit-circuitpython-24lc32-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-24lc32-1.0.8/pyproject.toml` & `adafruit-circuitpython-24lc32-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-24lc32"
 description = "CircuitPython driver for Adafruit 24LC32 I2C EEPROM Breakout"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_24LC32.git"}
 keywords = [
     "adafruit",
```

