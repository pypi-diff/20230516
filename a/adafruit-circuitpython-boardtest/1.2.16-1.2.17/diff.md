# Comparing `tmp/adafruit-circuitpython-boardtest-1.2.16.tar.gz` & `tmp/adafruit-circuitpython-boardtest-1.2.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-boardtest-1.2.16.tar", last modified: Fri Aug 26 02:33:46 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-boardtest-1.2.17.tar", last modified: Tue May 16 17:48:06 2023, max compression
```

## Comparing `adafruit-circuitpython-boardtest-1.2.16.tar` & `adafruit-circuitpython-boardtest-1.2.17.tar`

### file list

```diff
@@ -1,61 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.733893 adafruit-circuitpython-boardtest-1.2.16/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.733893 adafruit-circuitpython-boardtest-1.2.16/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.737893 adafruit-circuitpython-boardtest-1.2.16/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16351 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.737893 adafruit-circuitpython-boardtest-1.2.16/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4181 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.737893 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3504 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_gpio.py
--rw-r--r--   0 runner    (1001) docker     (121)     5359 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_i2c.py
--rw-r--r--   0 runner    (1001) docker     (121)     3291 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_led.py
--rw-r--r--   0 runner    (1001) docker     (121)     4745 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_sd.py
--rw-r--r--   0 runner    (1001) docker     (121)     2475 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_sd_cd.py
--rw-r--r--   0 runner    (1001) docker     (121)     6679 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_spi.py
--rw-r--r--   0 runner    (1001) docker     (121)     3026 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_uart.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_voltage_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.737893 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4952 2022-08-26 02:33:46.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-08-26 02:33:46.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:33:46.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-08-26 02:33:46.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-26 02:33:46.000000 adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      518 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5989 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7586 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.fzz
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.fzz.license
--rw-r--r--   0 runner    (1001) docker     (121)   168217 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.png
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.png.license
--rw-r--r--   0 runner    (1001) docker     (121)   149724 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig_bb.png
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/docs/test_jig_bb.png.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     8668 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/examples/boardtest_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-08-26 02:33:36.000000 adafruit-circuitpython-boardtest-1.2.16/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-26 02:33:22.000000 adafruit-circuitpython-boardtest-1.2.16/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:33:46.741893 adafruit-circuitpython-boardtest-1.2.16/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.810864 adafruit-circuitpython-boardtest-1.2.17/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd_cd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_uart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2740 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_voltage_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.814864 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 17:48:06.000000 adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz.license
+-rw-r--r--   0 runner    (1001) docker     (123)   168217 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)   149724 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/examples/boardtest_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 17:47:58.000000 adafruit-circuitpython-boardtest-1.2.17/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:47:46.000000 adafruit-circuitpython-boardtest-1.2.17/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:06.818864 adafruit-circuitpython-boardtest-1.2.17/setup.cfg
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-boardtest-1.2.17/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/.gitignore` & `adafruit-circuitpython-boardtest-1.2.17/.gitignore`

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

### Comparing `adafruit-circuitpython-boardtest-1.2.16/.pre-commit-config.yaml` & `adafruit-circuitpython-boardtest-1.2.17/.pre-commit-config.yaml`

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
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/.pylintrc` & `adafruit-circuitpython-boardtest-1.2.17/.pylintrc`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
-#
-# SPDX-License-Identifier: Unlicense
-
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
@@ -26,15 +22,15 @@
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
 
@@ -54,16 +50,16 @@
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
 
@@ -225,20 +221,14 @@
 
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
@@ -257,81 +247,53 @@
 
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
 
@@ -339,17 +301,14 @@
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

### Comparing `adafruit-circuitpython-boardtest-1.2.16/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-boardtest-1.2.17/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/LICENSE` & `adafruit-circuitpython-boardtest-1.2.17/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-boardtest-1.2.17/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/LICENSES/MIT.txt` & `adafruit-circuitpython-boardtest-1.2.17/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/LICENSES/Unlicense.txt` & `adafruit-circuitpython-boardtest-1.2.17/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/PKG-INFO` & `adafruit-circuitpython-boardtest-1.2.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-boardtest
-Version: 1.2.16
+Version: 1.2.17
 Summary: Helper for verifying a board definition works as expected
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BoardTest
 Keywords: adafruit,boardtest,board,test,testing,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/README.rst` & `adafruit-circuitpython-boardtest-1.2.17/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_gpio.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_gpio.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,27 +30,28 @@
 import supervisor
 
 try:
     from typing import Any, Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 LED_ON_DELAY_TIME = 0.2  # Seconds
 LED_OFF_DELAY_TIME = 0.2  # Seconds
 LED_PIN_NAMES = ["L", "LED", "RED_LED", "GREEN_LED", "BLUE_LED"]
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
+
 # Determine if given value is a number
 def _is_number(val: Any) -> bool:
     try:
         float(val)
         return True
     except ValueError:
         return False
@@ -60,15 +61,14 @@
 def _deinit_pins(gpios: Sequence[digitalio.DigitalInOut]) -> None:
     for g in gpios:
         g.deinit()
 
 
 # Toggle IO pins while waiting for answer
 def _toggle_wait(gpios: Sequence[digitalio.DigitalInOut]) -> bool:
-
     timestamp = time.monotonic()
     led_state = False
     print("Are the pins listed above toggling? [y/n]")
     while True:
         if led_state:
             if time.monotonic() > timestamp + LED_ON_DELAY_TIME:
                 led_state = False
@@ -81,15 +81,14 @@
             gpio.value = led_state
         if supervisor.runtime.serial_bytes_available:
             answer = input()
             return bool(answer == "y")
 
 
 def run_test(pins: Sequence[str]) -> Tuple[str, List[str]]:
-
     """
     Toggles all available GPIO on and off repeatedly.
 
     :param list[str] pins: list of pins to run the test on
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
@@ -98,15 +97,14 @@
 
     # Create a list of digital GPIO
     digital_pins = [p for p in pins if p[0] == "D" and _is_number(p[1])]
 
     # Toggle LEDs if we find any
     gpio_pins = analog_pins + digital_pins
     if gpio_pins:
-
         # Create a list of IO objects for us to toggle
         gpios = [digitalio.DigitalInOut(getattr(board, p)) for p in gpio_pins]
 
         # Print out the LEDs found
         print("GPIO pins found:", end=" ")
         for pin in gpio_pins:
             print(pin, end=" ")
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_i2c.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_i2c.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import busio
 
 try:
     from typing import Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 SDA_PIN_NAME = "SDA"
 SCL_PIN_NAME = "SCL"
 NUM_I2C_TESTS = 10  # Number of times to write and read EEPROM values
 EEPROM_I2C_MAX_ADDR = 255  # Self-imposed max memory address
@@ -51,19 +51,19 @@
 EEPROM_I2C_ADDR = 0x50
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
+
 # Open comms to I2C EEPROM by trying a write to memory address
 def _eeprom_i2c_wait(
     i2c: busio.I2C, i2c_addr: int, mem_addr: int, timeout: float = 1.0
 ) -> bool:
-
     # Try to access the I2C EEPROM (it becomes unresonsive during a write)
     timestamp = time.monotonic()
     while time.monotonic() < timestamp + timeout:
         try:
             i2c.writeto(i2c_addr, bytearray([mem_addr]), end=1)
             return True
         except OSError:
@@ -72,15 +72,14 @@
     return False
 
 
 # Write to address. Returns status (True for successful write, False otherwise)
 def _eeprom_i2c_write_byte(
     i2c: busio.I2C, i2c_addr: int, mem_addr: int, mem_data: int
 ) -> bool:
-
     # Make sure address is only one byte:
     if mem_addr > 255:
         return False
 
     # Make sure data is only one byte:
     if mem_data > 255:
         return False
@@ -94,15 +93,14 @@
     return True
 
 
 # Read from address. Returns tuple [status, result]
 def _eeprom_i2c_read_byte(
     i2c: busio.I2C, i2c_addr: int, mem_addr: int, timeout: float = 1.0
 ) -> Tuple[bool, bytearray]:
-
     # Make sure address is only one byte:
     if mem_addr > 255:
         return False, bytearray()
 
     # Try writing to address (EEPROM is unresponsive while writing)
     if not _eeprom_i2c_wait(i2c, i2c_addr, mem_addr, timeout):
         return False, bytearray()
@@ -113,27 +111,25 @@
 
     return True, buf
 
 
 def run_test(
     pins: Sequence[str], sda_pin: str = SDA_PIN_NAME, scl_pin: str = SCL_PIN_NAME
 ) -> Tuple[str, List[str]]:
-
     """
     Performs random writes and reads to I2C EEPROM.
 
     :param list[str] pins: list of pins to run the test on
     :param str sda_pin: pin name of I2C SDA
     :param str scl_pin: pin name of I2C SCL
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Write values to I2C EEPROM and verify the values match
     if list(set(pins).intersection(set([sda_pin, scl_pin]))):
-
         # Tell user to connect EEPROM chip
         print(
             "Connect a Microchip AT24HC04B EEPROM I2C chip. "
             + "Press enter to continue."
         )
         input()
 
@@ -143,15 +139,14 @@
         # Wait for I2C lock
         while not i2c.try_lock():
             pass
 
         # Pick a random address, write to it, read from it, and see if they match
         pass_test = True
         for _ in range(NUM_I2C_TESTS):
-
             # Randomly pick an address and a data value (one byte)
             mem_addr = random.randint(0, EEPROM_I2C_MAX_ADDR)
             mem_data = random.randint(0, 255)
             print("Address:\t" + hex(mem_addr))
             print("Writing:\t" + hex(mem_data))
 
             # Try writing this random value to the random address
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_led.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_led.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,34 +29,34 @@
 import supervisor
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 LED_ON_DELAY_TIME = 0.2  # Seconds
 LED_OFF_DELAY_TIME = 0.2  # Seconds
 LED_PIN_NAMES = ["L", "LED", "RED_LED", "YELLOW_LED", "GREEN_LED", "BLUE_LED"]
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
+
 # Toggle IO pins while waiting for answer
 def _toggle_wait(led_pins: Sequence[str]) -> bool:
     timestamp = time.monotonic()
     led_state = False
     print("Are the pins listed above toggling? [y/n]")
     while True:
-
         # Cycle through each pin in the list
         for pin in led_pins:
             led = digitalio.DigitalInOut(getattr(board, pin))
             led.direction = digitalio.Direction.OUTPUT
             blinking = True
 
             # Blink each LED once while looking for input
@@ -79,28 +79,26 @@
                     answer = input()
                     if answer == "y":
                         return True
                     return False
 
 
 def run_test(pins: Sequence[str]) -> Tuple[str, List[str]]:
-
     """
     Toggles the onboard LED(s) on and off.
 
     :param list[str] pins: list of pins to run the test on
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Look for pins with LED names
     led_pins = list(set(pins).intersection(set(LED_PIN_NAMES)))
 
     # Toggle LEDs if we find any
     if led_pins:
-
         # Print out the LEDs found
         print("LEDs found:", end=" ")
         for pin in led_pins:
             print(pin, end=" ")
         print("\n")
 
         # Blink LEDs and wait for user to verify test
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_sd.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import storage
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 MOSI_PIN_NAME = "SD_MOSI"
 MISO_PIN_NAME = "SD_MISO"
 SCK_PIN_NAME = "SD_SCK"
 CS_PIN_NAME = "SD_CS"
@@ -66,30 +66,28 @@
     pins: Sequence[str],
     mosi_pin: str = MOSI_PIN_NAME,
     miso_pin: str = MISO_PIN_NAME,
     sck_pin: str = SCK_PIN_NAME,
     cs_pin: str = CS_PIN_NAME,
     filename: str = FILENAME,
 ) -> Tuple[str, List[str]]:
-
     """
     Performs random writes and reads to file on attached SD card.
 
     :param list[str] pins: list of pins to run the test on
     :param str mosi_pin: pin name of SPI MOSI
     :param str miso_pin: pin name of SPI MISO
     :param str sck_pin: pin name of SPI SCK
     :param str cs_pin: pin name of SPI CS
     :param str filename: name of file to use as test on SD card
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Write characters to file on SD card and verify they were written
     if list(set(pins).intersection(set([mosi_pin, miso_pin, sck_pin]))):
-
         # Tell user to connect SD card
         print("Insert SD card into holder and connect SPI lines to holder.")
         print("Connect " + cs_pin + " to the CS (DAT3) pin on the SD " + "card holder.")
         print("WARNING: " + filename + " will be created or overwritten.")
         print("Press enter to continue.")
         input()
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_sd_cd.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_sd_cd.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,41 +30,39 @@
 import digitalio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 SD_CD_PIN_NAME = "SD_CD"
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
 
 def run_test(
     pins: Sequence[str], cd_pin: str = SD_CD_PIN_NAME
 ) -> Tuple[str, List[str]]:
-
     """
     Checks status of CD pin as user inserts and removes SD card.
 
     :param list[str] pins: list of pins to run the test on
     :param str cd_pin: pin name of chip detect (CD) line
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Ask user to insert and remove SD card
     if list(set(pins).intersection(set([cd_pin]))):
-
         # Configure CD pin as input with pullup
         cdt = digitalio.DigitalInOut(getattr(board, cd_pin))
         cdt.direction = digitalio.Direction.INPUT
         cdt.pull = digitalio.Pull.UP
 
         # Tell user to insert SD card
         print("Connect " + cd_pin + " to CD pin on SD card holder.")
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_spi.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_spi.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import busio
 
 try:
     from typing import Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 MOSI_PIN_NAME = "MOSI"
 MISO_PIN_NAME = "MISO"
 SCK_PIN_NAME = "SCK"
 CS_PIN_NAME = "D2"
@@ -64,23 +64,22 @@
 EEPROM_I2C_MAX_ADDR = 255  # Self-imposed max memory address
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
+
 # Wait for WIP bit to go low
 def _eeprom_spi_wait(
     spi: busio.SPI, csel: digitalio.DigitalInOut, timeout: float = 1.0
 ) -> bool:
-
     # Continually read from STATUS register
     timestamp = time.monotonic()
     while time.monotonic() < timestamp + timeout:
-
         # Perfrom RDSR operation
         csel.value = False
         result = bytearray(1)
         spi.write(bytearray([EEPROM_SPI_RDSR]))
         spi.readinto(result)
         csel.value = True
 
@@ -95,15 +94,14 @@
 def _eeprom_spi_write_byte(
     spi: busio.SPI,
     csel: digitalio.DigitalInOut,
     address: int,
     data: int,
     timeout: float = 1.0,
 ) -> bool:
-
     # Make sure address is only one byte:
     if address > 255:
         return False
 
     # Make sure data is only one byte:
     if data > 255:
         return False
@@ -125,15 +123,14 @@
     return True
 
 
 # Read from address. Returns tuple [status, result]
 def _eeprom_spi_read_byte(
     spi: busio.SPI, csel: digitalio.DigitalInOut, address: int, timeout: float = 1.0
 ) -> Tuple[bool, bytearray]:
-
     # Make sure address is only one byte:
     if address > 255:
         return False, bytearray()
 
     # Wait for WIP to be low
     if not _eeprom_spi_wait(spi, csel, timeout):
         return False, bytearray()
@@ -151,29 +148,27 @@
 def run_test(
     pins: Sequence[str],
     mosi_pin: str = MOSI_PIN_NAME,
     miso_pin: str = MISO_PIN_NAME,
     sck_pin: str = SCK_PIN_NAME,
     cs_pin: str = CS_PIN_NAME,
 ) -> Tuple[str, List[str]]:
-
     """
     Performs random writes and reads to file on attached SD card.
 
     :param list[str] pins: list of pins to run the test on
     :param str mosi_pin: pin name of SPI MOSI
     :param str miso_pin: pin name of SPI MISO
     :param str sck_pin: pin name of SPI SCK
     :param str cs_pin: pin name of SPI CS
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Write values to SPI EEPROM and verify the values match
     if list(set(pins).intersection(set([mosi_pin, miso_pin, sck_pin]))):
-
         # Tell user to connect EEPROM chip
         print("Connect a Microchip 25AA040A EEPROM SPI chip.")
         print("Connect " + cs_pin + " to the CS pin on the 25AA040.")
         print("Press enter to continue.")
         input()
 
         # Configure CS pin
@@ -192,15 +187,14 @@
         while not spi.try_lock():
             pass
         spi.configure(baudrate=BAUD_RATE, phase=0, polarity=0)
 
         # Pick a random address, write to it, read from it, and see if they match
         pass_test = True
         for _ in range(NUM_SPI_TESTS):
-
             # Randomly pick an address and a data value (one byte)
             mem_addr = random.randint(0, EEPROM_SPI_MAX_ADDR)
             mem_data = random.randint(0, 255)
             print("Address:\t" + hex(mem_addr))
             print("Writing:\t" + hex(mem_data))
 
             # Try writing this random value to the random address
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_uart.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_uart.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import busio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 TX_PIN_NAME = "TX"
 RX_PIN_NAME = "RX"
 BAUD_RATE = 9600
 NUM_UART_BYTES = 40  # Number of bytes to transmit over UART
@@ -53,28 +53,26 @@
 
 def run_test(
     pins: Sequence[str],
     tx_pin: str = TX_PIN_NAME,
     rx_pin: str = RX_PIN_NAME,
     baud_rate: int = BAUD_RATE,
 ) -> Tuple[str, List[str]]:
-
     """
     Performs random writes out of TX pin and reads on RX.
 
     :param list[str] pins: list of pins to run the test on
     :param str tx_pin: pin name of UART TX
     :param str rx_pin: pin name of UART RX
     :param int baudrate: the baudrate to use
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Echo some values over the UART
     if list(set(pins).intersection(set([tx_pin, rx_pin]))):
-
         # Tell user to create loopback connection
         print("Connect a wire from TX to RX. Press enter to continue.")
         input()
 
         # Initialize UART
         uart = busio.UART(
             getattr(board, tx_pin), getattr(board, rx_pin), baudrate=baud_rate
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_boardtest/boardtest_voltage_monitor.py` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_boardtest/boardtest_voltage_monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,43 +32,41 @@
 import analogio
 
 try:
     from typing import Sequence, Tuple, List
 except ImportError:
     pass
 
-__version__ = "1.2.16"
+__version__ = "1.2.17"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest.git"
 
 # Constants
 VOLTAGE_MONITOR_PIN_NAMES = ["VOLTAGE_MONITOR", "BATTERY"]
 ANALOG_REF = 3.3  # Reference analog voltage
 ANALOGIN_BITS = 16  # ADC resolution (bits) for CircuitPython
 
 # Test result strings
 PASS = "PASS"
 FAIL = "FAIL"
 NA = "N/A"
 
 
 def run_test(pins: Sequence[str]) -> Tuple[str, List[str]]:
-
     """
     Prints out voltage on the battery monitor or voltage monitor pin.
 
     :param list[str] pins: list of pins to run the test on
     :return: tuple(str, list[str]): test result followed by list of pins tested
     """
 
     # Look for pins with battery monitoring names
     monitor_pins = list(set(pins).intersection(set(VOLTAGE_MONITOR_PIN_NAMES)))
 
     # Print out voltage found on these pins
     if monitor_pins:
-
         # Print out the monitor pins found
         print("Voltage monitor pins found:", end=" ")
         for pin in monitor_pins:
             print(pin, end=" ")
         print("\n")
 
         # Print out the voltage found on each pin
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/PKG-INFO` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-boardtest
-Version: 1.2.16
+Version: 1.2.17
 Summary: Helper for verifying a board definition works as expected
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BoardTest
 Keywords: adafruit,boardtest,board,test,testing,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt` & `adafruit-circuitpython-boardtest-1.2.17/adafruit_circuitpython_boardtest.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

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
 adafruit_boardtest/__init__.py
 adafruit_boardtest/boardtest_gpio.py
 adafruit_boardtest/boardtest_i2c.py
 adafruit_boardtest/boardtest_led.py
```

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/_static/favicon.ico` & `adafruit-circuitpython-boardtest-1.2.17/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/api.rst` & `adafruit-circuitpython-boardtest-1.2.17/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/conf.py` & `adafruit-circuitpython-boardtest-1.2.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/index.rst` & `adafruit-circuitpython-boardtest-1.2.17/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.fzz` & `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.fzz`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/test_jig.png` & `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/docs/test_jig_bb.png` & `adafruit-circuitpython-boardtest-1.2.17/docs/test_jig_bb.png`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/examples/boardtest_simpletest.py` & `adafruit-circuitpython-boardtest-1.2.17/examples/boardtest_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-boardtest-1.2.16/pyproject.toml` & `adafruit-circuitpython-boardtest-1.2.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-boardtest"
 description = "Helper for verifying a board definition works as expected"
-version = "1.2.16"
+version = "1.2.17"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BoardTest"}
 keywords = [
     "adafruit",
```

