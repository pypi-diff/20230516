# Comparing `tmp/adafruit-circuitpython-dash-display-1.1.14.tar.gz` & `tmp/adafruit-circuitpython-dash-display-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dash-display-1.1.14.tar", last modified: Tue May 16 17:48:58 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-dash-display-1.1.9.tar", last modified: Fri Jul 22 16:48:46 2022, max compression
```

## Comparing `adafruit-circuitpython-dash-display-1.1.14.tar` & `adafruit-circuitpython-dash-display-1.1.9.tar`

### file list

```diff
@@ -1,57 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.072293 adafruit-circuitpython-dash-display-1.1.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.064293 adafruit-circuitpython-dash-display-1.1.14/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.064293 adafruit-circuitpython-dash-display-1.1.14/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-16 17:48:58.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-16 17:48:58.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:58.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 17:48:58.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 17:48:58.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9804 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/adafruit_dash_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_advancedtest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:58.068293 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/battery_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/door_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_setter_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/relay_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/relay_hi_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/temp_humid_daughter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 17:48:50.000000 adafruit-circuitpython-dash-display-1.1.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 17:48:41.000000 adafruit-circuitpython-dash-display-1.1.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:58.072293 adafruit-circuitpython-dash-display-1.1.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.882013 adafruit-circuitpython-dash-display-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.890014 adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2725 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4419 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.894014 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5162 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-22 16:48:46.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     9775 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/adafruit_dash_display.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.898014 adafruit-circuitpython-dash-display-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.902014 adafruit-circuitpython-dash-display-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5846 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      408 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.902014 adafruit-circuitpython-dash-display-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     5484 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_advancedtest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/battery_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2099 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/door_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2478 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1852 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2429 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_hi_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4048 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/temp_humid_daughter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2324 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-22 16:48:46.906015 adafruit-circuitpython-dash-display-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-07-22 16:48:32.000000 adafruit-circuitpython-dash-display-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dash-display-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/.gitignore` & `adafruit-circuitpython-dash-display-1.1.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
-.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/.pre-commit-config.yaml` & `adafruit-circuitpython-dash-display-1.1.9/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 23.3.0
+    rev: 22.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v1.1.2
+    rev: v0.14.0
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.17.4
+    rev: v2.11.1
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/.pylintrc` & `adafruit-circuitpython-dash-display-1.1.9/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=pylint.extensions.no_self_use
+load-plugins=
 
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
-# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
-disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
+# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
+disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,14 +221,20 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
+# List of optional constructs for which whitespace checking is disabled. `dict-
+# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
+# `trailing-comma` allows a space between comma and closing bracket: (a, ).
+# `empty-line` allows space-only lines.
+no-space-check=trailing-comma,dict-separator
+
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -247,53 +253,81 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
+# Naming hint for argument names
+argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
+# Naming hint for attribute names
+attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
+# Naming hint for class attribute names
+class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
+
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
+# Naming hint for class names
+# class-name-hint=[A-Z_][a-zA-Z0-9]+$
+class-name-hint=[A-Z_][a-zA-Z0-9_]+$
+
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
+# Naming hint for constant names
+const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
+
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
+# Naming hint for function names
+function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
+# Naming hint for inline iteration names
+inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
+
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
+# Naming hint for method names
+method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
+# Naming hint for module names
+module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
+
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -301,14 +335,17 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
+# Naming hint for variable names
+variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
+
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dash-display-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/LICENSE` & `adafruit-circuitpython-dash-display-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dash-display-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/LICENSES/MIT.txt` & `adafruit-circuitpython-dash-display-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dash-display-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/PKG-INFO` & `adafruit-circuitpython-dash-display-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dash-display
-Version: 1.1.14
+Version: 1.1.9
 Summary: CircuitPython library for creating Adafruit IO dashboards.
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
+Author: Adafruit Industries
+Author-email: circuitpython@adafruit.com
 License: MIT
-Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
-Keywords: adafruit,displays,iot,adafruitio,hardware,micropythoncircuitpython
+Keywords: adafruit displays iot adafruitio hardware micropythoncircuitpython
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-dash_display/badge/?version=latest
@@ -160,7 +161,9 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
+
+
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/README.rst` & `adafruit-circuitpython-dash-display-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/PKG-INFO` & `adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dash-display
-Version: 1.1.14
+Version: 1.1.9
 Summary: CircuitPython library for creating Adafruit IO dashboards.
-Author-email: Adafruit Industries <circuitpython@adafruit.com>
+Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
+Author: Adafruit Industries
+Author-email: circuitpython@adafruit.com
 License: MIT
-Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display
-Keywords: adafruit,displays,iot,adafruitio,hardware,micropythoncircuitpython
+Keywords: adafruit displays iot adafruitio hardware micropythoncircuitpython
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
-Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-dash_display/badge/?version=latest
@@ -160,7 +161,9 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display/blob/HEAD/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
+
+
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt` & `adafruit-circuitpython-dash-display-1.1.9/adafruit_circuitpython_dash_display.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,22 +3,21 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_dash_display.py
-optional_requirements.txt
 pyproject.toml
 requirements.txt
+setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release_gh.yml
-.github/workflows/release_pypi.yml
+.github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_dash_display.egg-info/PKG-INFO
 adafruit_circuitpython_dash_display.egg-info/SOURCES.txt
 adafruit_circuitpython_dash_display.egg-info/dependency_links.txt
 adafruit_circuitpython_dash_display.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/adafruit_dash_display.py` & `adafruit-circuitpython-dash-display-1.1.9/adafruit_dash_display.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 import time
 from collections import OrderedDict
 from adafruit_display_shapes.rect import Rect
 from adafruit_display_text.label import Label
 import displayio
 import terminalio
 
-__version__ = "1.1.14"
+__version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Dash_Display.git"
 
 
 class Feed:
     """Feed object to make getting and setting different feed properties easier"""
 
     def __init__(
@@ -110,15 +110,14 @@
         """Setter for last received value"""
         self._last_val = value
 
 
 class Hub:  # pylint: disable=too-many-instance-attributes
     """Object that lets you make an IOT dashboard"""
 
-    # pylint: disable=invalid-name
     def __init__(self, display, io, nav):
         self.display = display
 
         self.io = io  # pylint: disable=invalid-name
 
         self.up_btn, self.select, self.down, self.back, self.submit = nav
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/docs/_static/favicon.ico` & `adafruit-circuitpython-dash-display-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/docs/conf.py` & `adafruit-circuitpython-dash-display-1.1.9/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
-import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -49,22 +48,15 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit  CircuitPython Dash_Display Library"
-creation_year = "2021"
-current_year = str(datetime.datetime.now().year)
-year_duration = (
-    current_year
-    if current_year == creation_year
-    else creation_year + " - " + current_year
-)
-copyright = year_duration + " Eva Herrada for Adafruit Industries"
+copyright = "2021 Eva Herrada for Adafruit Industries"
 author = "Eva Herrada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/docs/index.rst` & `adafruit-circuitpython-dash-display-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_advancedtest.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/battery_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/battery_daughter.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("battery")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/door_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/door_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_daughter.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("neopixel")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_setter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/neopixel_setter_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/neopixel_setter_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/relay_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_daughter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("lamp")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/relay_hi_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/relay_hi_daughter.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 esp = adafruit_esp32spi.ESP_SPIcontrol(spi, esp32_cs, esp32_ready, esp32_reset)
 """Use below for Most Boards"""
 status_light = neopixel.NeoPixel(
     board.NEOPIXEL, 1, brightness=0.2
 )  # Uncomment for Most Boards
 wifi = adafruit_esp32spi_wifimanager.ESPSPI_WiFiManager(esp, secrets, status_light)
 
-
 # Define callback functions which will be called when certain events happen.
 # pylint: disable=unused-argument
 def connected(client):
     client.subscribe("heatindex")
 
 
 def subscribe(client, userdata, topic, granted_qos):
```

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_client_examples/temp_humid_daughter.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_client_examples/temp_humid_daughter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dash-display-1.1.14/examples/dash_display_simpletest.py` & `adafruit-circuitpython-dash-display-1.1.9/examples/dash_display_simpletest.py`

 * *Files identical despite different names*

