# Comparing `tmp/adafruit-circuitpython-adxl34x-1.12.8.tar.gz` & `tmp/adafruit-circuitpython-adxl34x-1.12.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-adxl34x-1.12.8.tar", last modified: Mon Nov 28 18:16:29 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-adxl34x-1.12.9.tar", last modified: Tue May 16 17:44:20 2023, max compression
```

## Comparing `adafruit-circuitpython-adxl34x-1.12.8.tar` & `adafruit-circuitpython-adxl34x-1.12.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.013213 adafruit-circuitpython-adxl34x-1.12.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.005212 adafruit-circuitpython-adxl34x-1.12.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.009212 adafruit-circuitpython-adxl34x-1.12.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.009212 adafruit-circuitpython-adxl34x-1.12.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.009212 adafruit-circuitpython-adxl34x-1.12.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3613 2022-11-28 18:16:29.013213 adafruit-circuitpython-adxl34x-1.12.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2821 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/README.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (122)    18139 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_adxl34x.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.009212 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3613 2022-11-28 18:16:28.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1166 2022-11-28 18:16:29.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:16:28.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:16:28.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:16:28.000000 adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.009212 adafruit-circuitpython-adxl34x-1.12.8/docs/
--rw-r--r--   0 runner    (1001) docker     (122)     6148 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (122)       91 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/.DS_Store.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.013213 adafruit-circuitpython-adxl34x-1.12.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5912 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      856 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:16:29.013213 adafruit-circuitpython-adxl34x-1.12.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      760 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_freefall_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      755 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_motion_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      854 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_offset_calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_tap_detection_test.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1260 2022-11-28 18:16:21.000000 adafruit-circuitpython-adxl34x-1.12.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:16:14.000000 adafruit-circuitpython-adxl34x-1.12.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:16:29.013213 adafruit-circuitpython-adxl34x-1.12.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.824602 adafruit-circuitpython-adxl34x-1.12.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.816602 adafruit-circuitpython-adxl34x-1.12.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-16 17:44:20.824602 adafruit-circuitpython-adxl34x-1.12.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/README.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18138 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_adxl34x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-05-16 17:44:20.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-16 17:44:20.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:44:20.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 17:44:20.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-16 17:44:20.000000 adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/.DS_Store.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:20.820602 adafruit-circuitpython-adxl34x-1.12.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_freefall_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_motion_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_offset_calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_tap_detection_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-16 17:44:13.000000 adafruit-circuitpython-adxl34x-1.12.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-16 17:44:03.000000 adafruit-circuitpython-adxl34x-1.12.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:44:20.824602 adafruit-circuitpython-adxl34x-1.12.9/setup.cfg
```

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-adxl34x-1.12.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/.gitignore` & `adafruit-circuitpython-adxl34x-1.12.9/.gitignore`

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

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/.pre-commit-config.yaml` & `adafruit-circuitpython-adxl34x-1.12.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/.pylintrc` & `adafruit-circuitpython-adxl34x-1.12.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-adxl34x-1.12.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/LICENSE` & `adafruit-circuitpython-adxl34x-1.12.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-adxl34x-1.12.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/LICENSES/MIT.txt` & `adafruit-circuitpython-adxl34x-1.12.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-adxl34x-1.12.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/PKG-INFO` & `adafruit-circuitpython-adxl34x-1.12.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adxl34x
-Version: 1.12.8
+Version: 1.12.9
 Summary: A CircuitPython driver for the ADXL34x family of accelerometers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ADXL34x
 Keywords: adafruit,hardware,accelerometer,acceleration,spi,i2c,triple,axismicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/README.rst` & `adafruit-circuitpython-adxl34x-1.12.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/adafruit_adxl34x.py` & `adafruit-circuitpython-adxl34x-1.12.9/adafruit_adxl34x.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     from typing import Tuple, Dict
 
     # This is only needed for typing
     import busio
 except ImportError:
     pass
 
-__version__ = "1.12.8"
+__version__ = "1.12.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ADXL34x.git"
 _ADXL345_DEFAULT_ADDRESS: int = const(0x53)  # Assumes ALT address pin low
 
 # Conversion factors
 _ADXL345_MG2G_MULTIPLIER: float = 0.004  # 4mg per lsb
 _STANDARD_GRAVITY: float = 9.80665  # earth standard gravity
 
@@ -174,15 +174,14 @@
         .. code-block:: python
 
             acceleration = accelerometer.acceleration
 
     """
 
     def __init__(self, i2c: busio.I2C, address: int = _ADXL345_DEFAULT_ADDRESS):
-
         self._i2c = i2c_device.I2CDevice(i2c, address)
         self._buffer = bytearray(6)
         # set the 'measure' bit in to enable measurement
         self._write_register_byte(_REG_POWER_CTL, 0x08)
         self._write_register_byte(_REG_INT_ENABLE, 0x0)
 
         self._enabled_interrupts = {}
```

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/PKG-INFO` & `adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-adxl34x
-Version: 1.12.8
+Version: 1.12.9
 Summary: A CircuitPython driver for the ADXL34x family of accelerometers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ADXL34x
 Keywords: adafruit,hardware,accelerometer,acceleration,spi,i2c,triple,axismicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/adafruit_circuitpython_adxl34x.egg-info/SOURCES.txt` & `adafruit-circuitpython-adxl34x-1.12.9/adafruit_circuitpython_adxl34x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/docs/.DS_Store` & `adafruit-circuitpython-adxl34x-1.12.9/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/docs/_static/favicon.ico` & `adafruit-circuitpython-adxl34x-1.12.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/docs/conf.py` & `adafruit-circuitpython-adxl34x-1.12.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/docs/examples.rst` & `adafruit-circuitpython-adxl34x-1.12.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/docs/index.rst` & `adafruit-circuitpython-adxl34x-1.12.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_freefall_detection_test.py` & `adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_freefall_detection_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_motion_detection_test.py` & `adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_motion_detection_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_offset_calibration.py` & `adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_offset_calibration.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/examples/adxl34x_tap_detection_test.py` & `adafruit-circuitpython-adxl34x-1.12.9/examples/adxl34x_tap_detection_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-adxl34x-1.12.8/pyproject.toml` & `adafruit-circuitpython-adxl34x-1.12.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-adxl34x"
 description = "A CircuitPython driver for the ADXL34x family of accelerometers."
-version = "1.12.8"
+version = "1.12.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ADXL34x"}
 keywords = [
     "adafruit",
```

