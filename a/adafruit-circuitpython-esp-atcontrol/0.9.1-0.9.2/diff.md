# Comparing `tmp/adafruit-circuitpython-esp-atcontrol-0.9.1.tar.gz` & `tmp/adafruit-circuitpython-esp-atcontrol-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp-atcontrol-0.9.1.tar", last modified: Mon Nov 14 21:25:09 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-esp-atcontrol-0.9.2.tar", last modified: Tue May 16 17:53:39 2023, max compression
```

## Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1.tar` & `adafruit-circuitpython-esp-atcontrol-0.9.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.051098 adafruit-circuitpython-esp-atcontrol-0.9.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.043098 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.043098 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-11-14 21:25:09.051098 adafruit-circuitpython-esp-atcontrol-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3910 2022-11-14 21:25:09.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-11-14 21:25:09.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 21:25:09.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-14 21:25:09.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-14 21:25:09.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27580 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol.py
--rw-r--r--   0 runner    (1001) docker     (121)     4161 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol_socket.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7460 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.047098 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5685 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      977 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 21:25:09.051098 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2392 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (121)     2964 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (121)     6238 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_countviewer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_localtime.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     2501 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2466 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_webclient.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1268 2022-11-14 21:25:00.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      171 2022-11-14 21:24:47.000000 adafruit-circuitpython-esp-atcontrol-0.9.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 21:25:09.051098 adafruit-circuitpython-esp-atcontrol-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.662764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.666764 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.670764 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-16 17:53:39.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.670764 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27580 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_socket.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7460 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6238 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_countviewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-16 17:53:30.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 17:53:20.000000 adafruit-circuitpython-esp-atcontrol-0.9.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:53:39.674764 adafruit-circuitpython-esp-atcontrol-0.9.2/setup.cfg
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-esp-atcontrol-0.9.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/.gitignore` & `adafruit-circuitpython-esp-atcontrol-0.9.2/.gitignore`

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

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/.pre-commit-config.yaml` & `adafruit-circuitpython-esp-atcontrol-0.9.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/.pylintrc` & `adafruit-circuitpython-esp-atcontrol-0.9.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-esp-atcontrol-0.9.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSE` & `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/MIT.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/PKG-INFO` & `adafruit-circuitpython-esp-atcontrol-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp-atcontrol
-Version: 0.9.1
+Version: 0.9.2
 Summary: CircuitPython driver for communicating using ESP AT command set.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol
 Keywords: adafruit,software,esp,at,atcontrol,internet,communication,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/README.rst` & `adafruit-circuitpython-esp-atcontrol-0.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO` & `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp-atcontrol
-Version: 0.9.1
+Version: 0.9.2
 Summary: CircuitPython driver for communicating using ESP AT command set.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol
 Keywords: adafruit,software,esp,at,atcontrol,internet,communication,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt` & `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_circuitpython_esp_atcontrol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 try:
     from typing import Optional, Dict, Union, List
     import busio
 except ImportError:
     pass
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_espATcontrol.git"
 
 
 class OKError(Exception):
     """The exception thrown when we didn't get acknowledgement to an AT command"""
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol_socket.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_socket.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     global _the_interface  # pylint: disable=global-statement, invalid-name
     _the_interface = iface
 
 
 SOCK_STREAM = const(1)
 AF_INET = const(2)
 
+
 # pylint: disable=too-many-arguments, unused-argument
 def getaddrinfo(
     host: str,
     port: int,
     family: int = 0,
     socktype: int = 0,
     proto: int = 0,
@@ -60,15 +61,16 @@
         if type != SOCK_STREAM:
             raise RuntimeError("Only SOCK_STREAM type supported")
         self._buffer = b""
         self.settimeout(0)
 
     def connect(self, address: Tuple[str, int], conntype: Optional[str] = None) -> None:
         """Connect the socket to the 'address' (which should be dotted quad IP). 'conntype'
-        is an extra that may indicate SSL or not, depending on the underlying interface"""
+        is an extra that may indicate SSL or not, depending on the underlying interface
+        """
         host, port = address
 
         if not _the_interface.socket_connect(
             conntype, host, port, keepalive=10, retries=3
         ):
             raise RuntimeError("Failed to connect to host", host)
         self._buffer = b""
```

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/adafruit_espatcontrol/adafruit_espatcontrol_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/docs/_static/favicon.ico` & `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/docs/conf.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/docs/index.rst` & `adafruit-circuitpython-esp-atcontrol-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_aio_post.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_cheerlights.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_countviewer.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_countviewer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_localtime.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_simpletest.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/examples/esp_atcontrol_webclient.py` & `adafruit-circuitpython-esp-atcontrol-0.9.2/examples/esp_atcontrol_webclient.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp-atcontrol-0.9.1/pyproject.toml` & `adafruit-circuitpython-esp-atcontrol-0.9.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp-atcontrol"
 description = "CircuitPython driver for communicating using ESP AT command set."
-version = "0.9.1"
+version = "0.9.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP_ATcontrol"}
 keywords = [
     "adafruit",
```

