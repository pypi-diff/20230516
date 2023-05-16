# Comparing `tmp/adafruit-circuitpython-charlcd-3.4.6.tar.gz` & `tmp/adafruit-circuitpython-charlcd-3.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-charlcd-3.4.6.tar", last modified: Mon Nov 28 18:14:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-charlcd-3.4.7.tar", last modified: Tue May 16 17:48:17 2023, max compression
```

## Comparing `adafruit-circuitpython-charlcd-3.4.6.tar` & `adafruit-circuitpython-charlcd-3.4.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.947754 adafruit-circuitpython-charlcd-3.4.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.939754 adafruit-circuitpython-charlcd-3.4.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.939754 adafruit-circuitpython-charlcd-3.4.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1103 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5402 2022-11-28 18:14:36.947754 adafruit-circuitpython-charlcd-3.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4643 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    25670 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd.py
--rw-r--r--   0 runner    (1001) docker     (122)     2449 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_i2c.py
--rw-r--r--   0 runner    (1001) docker     (122)     6497 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_rgb_i2c.py
--rw-r--r--   0 runner    (1001) docker     (122)     2798 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_spi.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5402 2022-11-28 18:14:36.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1513 2022-11-28 18:14:36.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:14:36.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      159 2022-11-28 18:14:36.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-11-28 18:14:36.000000 adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.943754 adafruit-circuitpython-charlcd-3.4.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      362 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5842 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)     1616 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     2298 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:14:36.947754 adafruit-circuitpython-charlcd-3.4.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_custom_character_nyan_cat.py
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_customcharacter.py
--rw-r--r--   0 runner    (1001) docker     (122)     1522 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_i2c_mono_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1744 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_i2c_rgb_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1125 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_keypad_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1729 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_mono_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2058 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rgb_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1734 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rpi_mono_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rpi_rgb_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1669 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_spi_mono_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1231 2022-11-28 18:14:27.000000 adafruit-circuitpython-charlcd-3.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      256 2022-11-28 18:14:16.000000 adafruit-circuitpython-charlcd-3.4.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:14:36.947754 adafruit-circuitpython-charlcd-3.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.614350 adafruit-circuitpython-charlcd-3.4.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.606349 adafruit-circuitpython-charlcd-3.4.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.606349 adafruit-circuitpython-charlcd-3.4.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.606349 adafruit-circuitpython-charlcd-3.4.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.610350 adafruit-circuitpython-charlcd-3.4.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-16 17:48:17.614350 adafruit-circuitpython-charlcd-3.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4643 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.610350 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25667 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_rgb_i2c.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_spi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.610350 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-05-16 17:48:17.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-16 17:48:17.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:17.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-16 17:48:17.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-16 17:48:17.000000 adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.610350 adafruit-circuitpython-charlcd-3.4.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.610350 adafruit-circuitpython-charlcd-3.4.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5842 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:17.614350 adafruit-circuitpython-charlcd-3.4.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_custom_character_nyan_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_customcharacter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_i2c_mono_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_i2c_rgb_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_keypad_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_mono_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rgb_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rpi_mono_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rpi_rgb_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_spi_mono_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-16 17:48:08.000000 adafruit-circuitpython-charlcd-3.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-16 17:47:57.000000 adafruit-circuitpython-charlcd-3.4.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:17.614350 adafruit-circuitpython-charlcd-3.4.7/setup.cfg
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-charlcd-3.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/.gitignore` & `adafruit-circuitpython-charlcd-3.4.7/.gitignore`

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

### Comparing `adafruit-circuitpython-charlcd-3.4.6/.pre-commit-config.yaml` & `adafruit-circuitpython-charlcd-3.4.7/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-charlcd-3.4.6/.pylintrc` & `adafruit-circuitpython-charlcd-3.4.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-charlcd-3.4.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/LICENSE` & `adafruit-circuitpython-charlcd-3.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-charlcd-3.4.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/LICENSES/MIT.txt` & `adafruit-circuitpython-charlcd-3.4.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-charlcd-3.4.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/PKG-INFO` & `adafruit-circuitpython-charlcd-3.4.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-charlcd
-Version: 3.4.6
+Version: 3.4.7
 Summary: CircuitPython library for standard character LCDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_CharLCD
 Keywords: adafruit,character,lcd,rgb,16x2,20x4,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/README.rst` & `adafruit-circuitpython-charlcd-3.4.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd.py` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 except ImportError:
     pass
 
 import time
 import digitalio
 from micropython import const
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_CharLCD.git"
 
 # Commands
 _LCD_CLEARDISPLAY = const(0x01)
 _LCD_RETURNHOME = const(0x02)
 _LCD_ENTRYMODESET = const(0x04)
 _LCD_DISPLAYCONTROL = const(0x08)
@@ -131,15 +131,14 @@
         d5: digitalio.DigitalInOut,
         d6: digitalio.DigitalInOut,
         d7: digitalio.DigitalInOut,
         columns: int,
         lines: int,
         # pylint: enable=invalid-name
     ) -> None:
-
         self.columns = columns
         self.lines = lines
         #  save pin numbers
         self.reset = rs
         self.enable = en
         self.dl4 = d4
         self.dl5 = d5
@@ -567,15 +566,14 @@
         db6: digitalio.DigitalInOut,
         db7: digitalio.DigitalInOut,
         columns: int,
         lines: int,
         backlight_pin: Optional[digitalio.DigitalInOut] = None,
         backlight_inverted: bool = False,
     ):
-
         # Backlight pin and inversion
         self.backlight_pin = backlight_pin
         self.backlight_inverted = backlight_inverted
 
         #  Setup backlight
         if backlight_pin is not None:
             self.backlight_pin.direction = digitalio.Direction.OUTPUT
@@ -651,15 +649,14 @@
         columns: int,
         lines: int,
         red: Union[pwmio.PWMOut, digitalio.DigitalInOut],
         green: Union[pwmio.PWMOut, digitalio.DigitalInOut],
         blue: Union[pwmio.PWMOut, digitalio.DigitalInOut],
         read_write: Optional[digitalio.DigitalInOut] = None,
     ) -> None:
-
         # Define read_write (rw) pin
         self.read_write = read_write
 
         # Setup rw pin if used
         if read_write is not None:
             self.read_write.direction = digitalio.Direction.OUTPUT
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_i2c.py` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_i2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     import busio
 except ImportError:
     pass
 
 from adafruit_mcp230xx.mcp23008 import MCP23008
 from adafruit_character_lcd.character_lcd import Character_LCD_Mono
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_CharLCD.git"
 
 
 class Character_LCD_I2C(Character_LCD_Mono):
     # pylint: disable=too-few-public-methods, too-many-arguments
     """Character LCD connected to I2C/SPI backpack using its I2C connection.
     This is a subclass of `Character_LCD_Mono` and implements all the same
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_rgb_i2c.py` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_rgb_i2c.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 except ImportError:
     pass
 
 import digitalio
 from adafruit_mcp230xx.mcp23017 import MCP23017
 from adafruit_character_lcd.character_lcd import Character_LCD_RGB
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_CharLCD.git"
 
 
 class Character_LCD_RGB_I2C(Character_LCD_RGB):
     """RGB Character LCD connected to I2C shield or Pi plate using I2C connection.
     This is a subclass of `Character_LCD_RGB` and implements all of the same
     functions and functionality.
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_character_lcd/character_lcd_spi.py` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_character_lcd/character_lcd_spi.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     import digitalio
 except ImportError:
     pass
 
 import adafruit_74hc595
 from adafruit_character_lcd.character_lcd import Character_LCD_Mono
 
-__version__ = "3.4.6"
+__version__ = "3.4.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_CharLCD.git"
 
 
 class Character_LCD_SPI(Character_LCD_Mono):  # pylint: disable=too-few-public-methods
     """Character LCD connected to I2C/SPI backpack using its SPI connection.
     This is a subclass of `Character_LCD_Mono` and implements all of the same
     functions and functionality.
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/PKG-INFO` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-charlcd
-Version: 3.4.6
+Version: 3.4.7
 Summary: CircuitPython library for standard character LCDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_CharLCD
 Keywords: adafruit,character,lcd,rgb,16x2,20x4,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-charlcd-3.4.6/adafruit_circuitpython_charlcd.egg-info/SOURCES.txt` & `adafruit-circuitpython-charlcd-3.4.7/adafruit_circuitpython_charlcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/docs/_static/favicon.ico` & `adafruit-circuitpython-charlcd-3.4.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/docs/conf.py` & `adafruit-circuitpython-charlcd-3.4.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/docs/examples.rst` & `adafruit-circuitpython-charlcd-3.4.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/docs/index.rst` & `adafruit-circuitpython-charlcd-3.4.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_custom_character_nyan_cat.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_custom_character_nyan_cat.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_customcharacter.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_customcharacter.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_i2c_mono_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_i2c_mono_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_i2c_rgb_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_i2c_rgb_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_keypad_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_keypad_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_mono_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_mono_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rgb_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rgb_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rpi_mono_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rpi_mono_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_rpi_rgb_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_rpi_rgb_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/examples/charlcd_spi_mono_simpletest.py` & `adafruit-circuitpython-charlcd-3.4.7/examples/charlcd_spi_mono_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-charlcd-3.4.6/pyproject.toml` & `adafruit-circuitpython-charlcd-3.4.7/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-charlcd"
 description = "CircuitPython library for standard character LCDs."
-version = "3.4.6"
+version = "3.4.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_CharLCD"}
 keywords = [
     "adafruit",
```

