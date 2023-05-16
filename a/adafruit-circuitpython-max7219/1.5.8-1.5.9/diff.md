# Comparing `tmp/adafruit-circuitpython-max7219-1.5.8.tar.gz` & `tmp/adafruit-circuitpython-max7219-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-max7219-1.5.8.tar", last modified: Fri Aug 26 02:25:39 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-max7219-1.5.9.tar", last modified: Tue Nov 15 18:36:48 2022, max compression
```

## Comparing `adafruit-circuitpython-max7219-1.5.8.tar` & `adafruit-circuitpython-max7219-1.5.9.tar`

### file list

```diff
@@ -1,52 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.018930 adafruit-circuitpython-max7219-1.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.022930 adafruit-circuitpython-max7219-1.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.022930 adafruit-circuitpython-max7219-1.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.022930 adafruit-circuitpython-max7219-1.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2635 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.022930 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3396 2022-08-26 02:25:38.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1093 2022-08-26 02:25:39.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:25:38.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:25:38.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:25:38.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.022930 adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3921 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/bcddigits.py
--rw-r--r--   0 runner    (1001) docker     (121)     9473 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/matrices.py
--rw-r--r--   0 runner    (1001) docker     (121)     7377 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/max7219.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5749 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1060 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1506 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/examples/max7219_custommatrixtest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/examples/max7219_showbcddigits.py
--rw-r--r--   0 runner    (1001) docker     (121)     1349 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/examples/max7219_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-08-26 02:25:29.000000 adafruit-circuitpython-max7219-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:25:19.000000 adafruit-circuitpython-max7219-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:25:39.026930 adafruit-circuitpython-max7219-1.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.924616 adafruit-circuitpython-max7219-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.928617 adafruit-circuitpython-max7219-1.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.928617 adafruit-circuitpython-max7219-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1103 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.932617 adafruit-circuitpython-max7219-1.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     3396 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2635 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.932617 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3396 2022-11-15 18:36:48.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1131 2022-11-15 18:36:48.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-15 18:36:48.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-15 18:36:48.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-15 18:36:48.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.932617 adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3921 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/bcddigits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9473 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/matrices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7409 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/max7219.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)     5749 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      434 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)     1060 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1506 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/examples/max7219_custommatrixtest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2075 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/examples/max7219_showbcddigits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1349 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/examples/max7219_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2022-11-15 18:36:40.000000 adafruit-circuitpython-max7219-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-15 18:36:33.000000 adafruit-circuitpython-max7219-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-15 18:36:48.936617 adafruit-circuitpython-max7219-1.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-max7219-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/.gitignore` & `adafruit-circuitpython-max7219-1.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-max7219-1.5.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/.pylintrc` & `adafruit-circuitpython-max7219-1.5.9/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
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
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
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

### Comparing `adafruit-circuitpython-max7219-1.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-max7219-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/LICENSE` & `adafruit-circuitpython-max7219-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-max7219-1.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-max7219-1.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-max7219-1.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/PKG-INFO` & `adafruit-circuitpython-max7219-1.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max7219
-Version: 1.5.8
+Version: 1.5.9
 Summary: CircuitPython library for MAX7219 LED matrix driver.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MAX7219
 Keywords: adafruit,max7219,LED,matrix,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/README.rst` & `adafruit-circuitpython-max7219-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/PKG-INFO` & `adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max7219
-Version: 1.5.8
+Version: 1.5.9
 Summary: CircuitPython library for MAX7219 LED matrix driver.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MAX7219
 Keywords: adafruit,max7219,LED,matrix,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/adafruit_circuitpython_max7219.egg-info/SOURCES.txt` & `adafruit-circuitpython-max7219-1.5.9/adafruit_circuitpython_max7219.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

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
 adafruit_circuitpython_max7219.egg-info/PKG-INFO
 adafruit_circuitpython_max7219.egg-info/SOURCES.txt
 adafruit_circuitpython_max7219.egg-info/dependency_links.txt
 adafruit_circuitpython_max7219.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/bcddigits.py` & `adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/bcddigits.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     # Used only for typing
     from typing import List
     import digitalio
     import busio
 except ImportError:
     pass
 
-__version__ = "1.5.8"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MAX7219.git"
 
 _DECODEMODE = const(9)
 _SCANLIMIT = const(11)
 _SHUTDOWN = const(12)
 _DISPLAYTEST = const(15)
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/matrices.py` & `adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/matrices.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # Used only for typing
     from typing import Tuple
     import digitalio
     import busio
 except ImportError:
     pass
 
-__version__ = "1.5.8"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MAX7219.git"
 
 _DECODEMODE = const(9)
 _SCANLIMIT = const(11)
 _SHUTDOWN = const(12)
 _DISPLAYTEST = const(15)
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/adafruit_max7219/max7219.py` & `adafruit-circuitpython-max7219-1.5.9/adafruit_max7219/max7219.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     # Used only for typing
     import typing  # pylint: disable=unused-import
     import busio
 except ImportError:
     pass
 
-__version__ = "1.5.8"
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MAX7219.git"
 
 # register definitions
 _DIGIT0 = const(1)
 _INTENSITY = const(10)
 
 
@@ -74,15 +74,15 @@
     """
 
     def __init__(
         self,
         width: int,
         height: int,
         spi: busio.SPI,
-        cs: digitalio.DigitalInOut,
+        cs: digitalio.DigitalInOut,  # pylint: disable=invalid-name
         *,
         baudrate: int = 8000000,
         polarity: int = 0,
         phase: int = 0
     ):
 
         self._chip_select = cs
```

### Comparing `adafruit-circuitpython-max7219-1.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-max7219-1.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/docs/conf.py` & `adafruit-circuitpython-max7219-1.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/docs/index.rst` & `adafruit-circuitpython-max7219-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/examples/max7219_custommatrixtest.py` & `adafruit-circuitpython-max7219-1.5.9/examples/max7219_custommatrixtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/examples/max7219_showbcddigits.py` & `adafruit-circuitpython-max7219-1.5.9/examples/max7219_showbcddigits.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/examples/max7219_simpletest.py` & `adafruit-circuitpython-max7219-1.5.9/examples/max7219_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max7219-1.5.8/pyproject.toml` & `adafruit-circuitpython-max7219-1.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-max7219"
 description = "CircuitPython library for MAX7219 LED matrix driver."
-version = "1.5.8"
+version = "1.5.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MAX7219"}
 keywords = [
     "adafruit",
```

