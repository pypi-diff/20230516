# Comparing `tmp/adafruit-circuitpython-apds9960-3.1.6.tar.gz` & `tmp/adafruit-circuitpython-apds9960-3.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-apds9960-3.1.6.tar", last modified: Mon Nov 28 18:16:11 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-apds9960-3.1.7.tar", last modified: Tue May 16 17:44:47 2023, max compression
```

## Comparing `adafruit-circuitpython-apds9960-3.1.6.tar` & `adafruit-circuitpython-apds9960-3.1.7.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.106207 adafruit-circuitpython-apds9960-3.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.106207 adafruit-circuitpython-apds9960-3.1.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.106207 adafruit-circuitpython-apds9960-3.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.106207 adafruit-circuitpython-apds9960-3.1.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     9910 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     9125 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    35503 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/apds9960.py
--rw-r--r--   0 runner    (1001) docker     (122)     1568 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/colorutility.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     9910 2022-11-28 18:16:11.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1164 2022-11-28 18:16:11.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:16:11.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:16:11.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-28 18:16:11.000000 adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      197 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5611 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      810 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1214 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      872 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_color_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      726 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_gesture_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      928 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_proximity_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1259 2022-11-28 18:16:03.000000 adafruit-circuitpython-apds9960-3.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:15:56.000000 adafruit-circuitpython-apds9960-3.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:16:11.110206 adafruit-circuitpython-apds9960-3.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.392189 adafruit-circuitpython-apds9960-3.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35503 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/apds9960.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/colorutility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_color_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_gesture_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_proximity_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/setup.cfg
```

### Comparing `adafruit-circuitpython-apds9960-3.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/.gitignore` & `adafruit-circuitpython-apds9960-3.1.7/.gitignore`

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

### Comparing `adafruit-circuitpython-apds9960-3.1.6/.pre-commit-config.yaml` & `adafruit-circuitpython-apds9960-3.1.7/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-apds9960-3.1.6/.pylintrc` & `adafruit-circuitpython-apds9960-3.1.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-apds9960-3.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/LICENSE` & `adafruit-circuitpython-apds9960-3.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-apds9960-3.1.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/LICENSES/MIT.txt` & `adafruit-circuitpython-apds9960-3.1.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-apds9960-3.1.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/PKG-INFO` & `adafruit-circuitpython-apds9960-3.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-apds9960
-Version: 3.1.6
+Version: 3.1.7
 Summary: CircuitPython driver for APSD9960 Gesture breakout board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_APDS9960
 Keywords: adafruit,apsd9960,gesture,color,proximity,light,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-apds9960-3.1.6/README.rst` & `adafruit-circuitpython-apds9960-3.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/apds9960.py` & `adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/apds9960.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 try:
     # Only used for typing
     from typing import Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "3.1.6"
+__version__ = "3.1.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960.git"
 
 # Only one address is possible for the APDS9960, no alternates are available
 _APDS9960_I2C_ADDRESS = const(0x39)
 _DEVICE_ID = const(0xAB)
 
 # APDS9960_RAM        = const(0x00)
@@ -122,14 +122,15 @@
 
 _BIT_POS_CONTROL_PGAIN = const(2)
 _BIT_MASK_CONTROL_PGAIN = const(0x0C)
 
 _BIT_POS_GCONF2_GGAIN = const(5)
 _BIT_MASK_GCONF2_GGAIN = const(0x60)
 
+
 # pylint: disable-msg=too-many-instance-attributes
 class APDS9960:
     """
     Provide basic driver services for the APDS9960 breakout board
 
     :param ~busio.I2C i2c: The I2C bus the APDS9960 is connected to
     :param int rotation: Rotation of the device. Defaults to :const:`0`
@@ -170,15 +171,14 @@
         self,
         i2c: I2C,
         *,
         rotation: int = 0,
         reset: bool = True,
         set_defaults: bool = True
     ):
-
         self.rotation = rotation
 
         self.buf129 = None  # Gesture FIFO buffer, only instantiated if needed
         self.buf4 = None  # Gesture data processing buffer, only instantiated if needed
         self.buf2 = bytearray(2)  # I2C communication buffer
 
         self.i2c_device = I2CDevice(i2c, _APDS9960_I2C_ADDRESS)
```

### Comparing `adafruit-circuitpython-apds9960-3.1.6/adafruit_apds9960/colorutility.py` & `adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/colorutility.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ====================================================
 
 Helper functions for color calculations
 
 * Author(s): Michael McWethy
 """
 
-__version__ = "3.1.6"
+__version__ = "3.1.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960.git"
 
 
 def calculate_color_temperature(r: int, g: int, b: int) -> float:
     """Converts the raw R/G/B values to color temperature in degrees Kelvin"""
 
     #  1. Map RGB values to their XYZ counterparts.
```

### Comparing `adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/PKG-INFO` & `adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-apds9960
-Version: 3.1.6
+Version: 3.1.7
 Summary: CircuitPython driver for APSD9960 Gesture breakout board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_APDS9960
 Keywords: adafruit,apsd9960,gesture,color,proximity,light,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-apds9960-3.1.6/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt` & `adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/docs/_static/favicon.ico` & `adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/docs/conf.py` & `adafruit-circuitpython-apds9960-3.1.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/docs/examples.rst` & `adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/docs/index.rst` & `adafruit-circuitpython-apds9960-3.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_color_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_color_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_gesture_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_gesture_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/examples/apds9960_proximity_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_proximity_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.6/pyproject.toml` & `adafruit-circuitpython-apds9960-3.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-apds9960"
 description = "CircuitPython driver for APSD9960 Gesture breakout board"
-version = "3.1.6"
+version = "3.1.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960"}
 keywords = [
     "adafruit",
```

