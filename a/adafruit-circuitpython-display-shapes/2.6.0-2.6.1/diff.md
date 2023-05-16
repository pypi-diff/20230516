# Comparing `tmp/adafruit-circuitpython-display_shapes-2.6.0.tar.gz` & `tmp/adafruit-circuitpython-display_shapes-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-display_shapes-2.6.0.tar", last modified: Mon Jan  9 00:55:16 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-display_shapes-2.6.1.tar", last modified: Tue May 16 17:49:29 2023, max compression
```

## Comparing `adafruit-circuitpython-display_shapes-2.6.0.tar` & `adafruit-circuitpython-display_shapes-2.6.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.861248 adafruit-circuitpython-display_shapes-2.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.849248 adafruit-circuitpython-display_shapes-2.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.853248 adafruit-circuitpython-display_shapes-2.6.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.853248 adafruit-circuitpython-display_shapes-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.853248 adafruit-circuitpython-display_shapes-2.6.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-09 00:55:16.861248 adafruit-circuitpython-display_shapes-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.853248 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-01-09 00:55:16.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-01-09 00:55:16.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 00:55:16.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-09 00:55:16.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-01-09 00:55:16.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.857248 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/circle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     9344 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/multisparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/rect.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/roundrect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/sparkline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/triangle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.857248 adafruit-circuitpython-display_shapes-2.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.857248 adafruit-circuitpython-display_shapes-2.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 00:55:16.861248 adafruit-circuitpython-display_shapes-2.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_circle_animation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_simpletest_magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4011 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5690 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_ticks.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8544 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_triple.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-01-09 00:55:08.000000 adafruit-circuitpython-display_shapes-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-09 00:55:00.000000 adafruit-circuitpython-display_shapes-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-09 00:55:16.861248 adafruit-circuitpython-display_shapes-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.785800 adafruit-circuitpython-display_shapes-2.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-16 17:49:29.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/circle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/multisparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/roundrect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/sparkline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/triangle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.789800 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_circle_animation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest_magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4010 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5689 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_ticks.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8543 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_triple.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-16 17:49:22.000000 adafruit-circuitpython-display_shapes-2.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 17:49:12.000000 adafruit-circuitpython-display_shapes-2.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:49:29.793800 adafruit-circuitpython-display_shapes-2.6.1/setup.cfg
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-display_shapes-2.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/.gitignore` & `adafruit-circuitpython-display_shapes-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/.pre-commit-config.yaml` & `adafruit-circuitpython-display_shapes-2.6.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/.pylintrc` & `adafruit-circuitpython-display_shapes-2.6.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-display_shapes-2.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/LICENSE` & `adafruit-circuitpython-display_shapes-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/LICENSES/MIT.txt` & `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-display_shapes-2.6.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/PKG-INFO` & `adafruit-circuitpython-display_shapes-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display_shapes
-Version: 2.6.0
+Version: 2.6.1
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/README.rst` & `adafruit-circuitpython-display_shapes-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-display-shapes
-Version: 2.6.0
+Version: 2.6.1
 Summary: Various common shapes for use with displayio
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes
 Keywords: adafruit,blinka,circuitpython,micropython,display_shapes,shapes,displayio,drawing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_circuitpython_display_shapes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/circle.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/circle.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.roundrect import RoundRect
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Circle(RoundRect):
     # pylint: disable=too-few-public-methods, invalid-name
     """A circle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/line.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/line.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Line(Polygon):
     # pylint: disable=too-many-arguments,invalid-name, too-few-public-methods
     """A line.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/multisparkline.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/multisparkline.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         # y_bottom: The actual minimum value of the vertical scale, will be
         # updated if autorange
         self.y_tops = self.y_maxs.copy()
         # y_top: The actual maximum value of the vertical scale, will be
         # updated if autorange
         self._palette = displayio.Palette(self._lines + 1)
         self._palette.make_transparent(0)
-        for (i, color) in enumerate(colors):
+        for i, color in enumerate(colors):
             self._palette[i + 1] = color
         self._bitmap = displayio.Bitmap(width, height, self._lines + 1)
 
         super().__init__(self._bitmap, pixel_shader=self._palette, x=x, y=y)
 
     # pylint: enable=too-many-arguments
 
@@ -168,15 +168,15 @@
         :param bool update: trigger recreation of primitives
 
         Note: when adding multiple values per sparkline it is more efficient to call
         this method with parameter 'update=False' and then to manually
         call the update()-method
         """
 
-        for (i, value) in enumerate(values):
+        for i, value in enumerate(values):
             if value is not None:
                 top = self.y_tops[i]
                 bottom = self.y_bottoms[i]
                 if (
                     self._buffers[i].len() >= self._max_items
                 ):  # if list is full, remove the first item
                     first = self._buffers[i].pop()
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/polygon.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional, List, Tuple
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Polygon(displayio.TileGrid):
     """A polygon.
 
     :param list points: A list of (x, y) tuples of the points
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/rect.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/rect.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Rect(displayio.TileGrid):
     """A rectangle.
 
     :param int x: The x-position of the top left corner.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/roundrect.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/roundrect.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 import displayio
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class RoundRect(displayio.TileGrid):
     # pylint: disable=too-many-arguments
     """A round-corner rectangle.
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/sparkline.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/sparkline.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/adafruit_display_shapes/triangle.py` & `adafruit-circuitpython-display_shapes-2.6.1/adafruit_display_shapes/triangle.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 try:
     from typing import Optional
 except ImportError:
     pass
 
 from adafruit_display_shapes.polygon import Polygon
 
-__version__ = "2.6.0"
+__version__ = "2.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes.git"
 
 
 class Triangle(Polygon):
     # pylint: disable=too-many-arguments,invalid-name
     """A triangle.
 
@@ -43,14 +43,15 @@
     :param int x2: The x-position of the third vertex.
     :param int y2: The y-position of the third vertex.
     :param int|None fill: The color to fill the triangle. Can be a hex value for a color or
                     ``None`` for transparent.
     :param int|None outline: The outline of the triangle. Can be a hex value for a color or
                     ``None`` for no outline.
     """
+
     # pylint: disable=too-many-locals
     def __init__(
         self,
         x0: int,
         y0: int,
         x1: int,
         y1: int,
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/docs/_static/favicon.ico` & `adafruit-circuitpython-display_shapes-2.6.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/docs/api.rst` & `adafruit-circuitpython-display_shapes-2.6.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/docs/conf.py` & `adafruit-circuitpython-display_shapes-2.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/docs/examples.rst` & `adafruit-circuitpython-display_shapes-2.6.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/docs/index.rst` & `adafruit-circuitpython-display_shapes-2.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_circle_animation.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_circle_animation.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 delta_x = 2
 delta_y = 2
 
 # Showing the items on the screen
 display.show(main_group)
 
 while True:
-
     if circle.y + circle_radius >= display.height - circle_radius:
         delta_y = -1
     if circle.x + circle_radius >= display.width - circle_radius:
         delta_x = -1
     if circle.x - circle_radius <= 0 - circle_radius:
         delta_x = 1
     if circle.y - circle_radius <= 0 - circle_radius:
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_simpletest.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_simpletest_magtag.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_simpletest_magtag.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_simpletest.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_simpletest.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,14 @@
 
 
 # Add my_group (containing the sparkline) to the display
 display.show(my_group)
 
 # Start the main loop
 while True:
-
     # turn off the auto_refresh of the display while modifying the sparkline
     display.auto_refresh = False
 
     # add_value: add a new value to a sparkline
     # Note: The y-range for mySparkline1 is set to 0 to 10, so all these random
     # values (between 0 and 10) will fit within the visible range of this sparkline
     sparkline1.add_value(random.uniform(0, 10))
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_ticks.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_ticks.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
 
 
 # Set the display to show my_group that contains the sparkline and other graphics
 display.show(my_group)
 
 # Start the main loop
 while True:
-
     # Turn off auto_refresh to prevent partial updates of the screen during updates
     # of the sparkline drawing
     display.auto_refresh = False
 
     # add_value: add a new value to a sparkline
     # Note: The y-range for mySparkline1 is set to 0 to 10, so all these random
     # values (between 0 and 10) will fit within the visible range of this sparkline
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/examples/display_shapes_sparkline_triple.py` & `adafruit-circuitpython-display_shapes-2.6.1/examples/display_shapes_sparkline_triple.py`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,14 @@
 # sparklines
 display.show(my_group)
 
 i = 0  # This is a counter for changing the random values for mySparkline3
 
 # Start the main loop
 while True:
-
     # Turn off auto_refresh to prevent partial updates of the screen during updates
     # of the sparklines
     display.auto_refresh = False
 
     # add_value: add a new value to a sparkline
     # Note: The y-range for sparkline1 is set to -1 to 1.25, so all these random
     # values (between 0 and 1) will fit within the visible range of this sparkline
```

### Comparing `adafruit-circuitpython-display_shapes-2.6.0/pyproject.toml` & `adafruit-circuitpython-display_shapes-2.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-display_shapes"
 description = "Various common shapes for use with displayio"
-version = "2.6.0"
+version = "2.6.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Display_Shapes"}
 keywords = [
     "adafruit",
```

