# Comparing `tmp/adafruit-circuitpython-aw9523-1.1.5.tar.gz` & `tmp/adafruit-circuitpython-aw9523-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-aw9523-1.1.5.tar", last modified: Sat Jan  7 15:43:43 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-aw9523-1.1.6.tar", last modified: Tue May 16 17:45:55 2023, max compression
```

## Comparing `adafruit-circuitpython-aw9523-1.1.5.tar` & `adafruit-circuitpython-aw9523-1.1.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.208791 adafruit-circuitpython-aw9523-1.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.208791 adafruit-circuitpython-aw9523-1.1.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.208791 adafruit-circuitpython-aw9523-1.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     9367 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_aw9523.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-01-07 15:43:43.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-01-07 15:43:43.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-07 15:43:43.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-01-07 15:43:43.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-01-07 15:43:43.000000 adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_constant_current_leds.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_read_all_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_set_all_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-01-07 15:43:35.000000 adafruit-circuitpython-aw9523-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-07 15:43:26.000000 adafruit-circuitpython-aw9523-1.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-07 15:43:43.212791 adafruit-circuitpython-aw9523-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_aw9523.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_constant_current_leds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_read_all_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_set_all_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/setup.cfg
```

### Comparing `adafruit-circuitpython-aw9523-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/.gitignore` & `adafruit-circuitpython-aw9523-1.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/.pre-commit-config.yaml` & `adafruit-circuitpython-aw9523-1.1.6/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-aw9523-1.1.5/.pylintrc` & `adafruit-circuitpython-aw9523-1.1.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-aw9523-1.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/LICENSE` & `adafruit-circuitpython-aw9523-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-aw9523-1.1.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/LICENSES/MIT.txt` & `adafruit-circuitpython-aw9523-1.1.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-aw9523-1.1.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/PKG-INFO` & `adafruit-circuitpython-aw9523-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-aw9523
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for AW9523 GPIO expander and LED driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AW9523
 Keywords: adafruit,blinka,circuitpython,micropython,aw9523,gpio,expander,led,constant-,current,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-aw9523-1.1.5/README.rst` & `adafruit-circuitpython-aw9523-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/adafruit_aw9523.py` & `adafruit-circuitpython-aw9523-1.1.6/adafruit_aw9523.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 try:
     from typing import Optional
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AW9523.git"
 
 _AW9523_DEFAULT_ADDR = const(0x58)
 _AW9523_REG_CHIPID = const(0x10)  # Register for hardcode chip ID
 _AW9523_REG_SOFTRESET = const(0x7F)  # Register for soft resetting
 _AW9523_REG_INPUT0 = const(0x00)  # Register for reading input values
 _AW9523_REG_OUTPUT0 = const(0x02)  # Register for writing output values
@@ -169,14 +169,15 @@
 ====================================================
 
 Digital input/output of the MCP230xx.
 
 * Author(s): Tony DiCola
 """
 
+
 # Internal helpers to simplify setting and getting a bit inside an integer.
 def _get_bit(val: bool, bit: int) -> bool:
     return val & (1 << bit) > 0
 
 
 def _enable_bit(val: bool, bit: int) -> int:
     return val | (1 << bit)
```

### Comparing `adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/PKG-INFO` & `adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-aw9523
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python library for AW9523 GPIO expander and LED driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AW9523
 Keywords: adafruit,blinka,circuitpython,micropython,aw9523,gpio,expander,led,constant-,current,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-aw9523-1.1.5/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt` & `adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/docs/_static/favicon.ico` & `adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/docs/conf.py` & `adafruit-circuitpython-aw9523-1.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/docs/index.rst` & `adafruit-circuitpython-aw9523-1.1.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_constant_current_leds.py` & `adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_constant_current_leds.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/examples/aw9523_simpletest.py` & `adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.5/pyproject.toml` & `adafruit-circuitpython-aw9523-1.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-aw9523"
 description = "Python library for AW9523 GPIO expander and LED driver"
-version = "1.1.5"
+version = "1.1.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AW9523"}
 keywords = [
     "adafruit",
```

