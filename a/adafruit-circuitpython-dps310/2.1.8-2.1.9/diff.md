# Comparing `tmp/adafruit-circuitpython-dps310-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-dps310-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dps310-2.1.8.tar", last modified: Fri Aug 26 02:13:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-dps310-2.1.9.tar", last modified: Tue Sep 27 14:51:21 2022, max compression
```

## Comparing `adafruit-circuitpython-dps310-2.1.8.tar` & `adafruit-circuitpython-dps310-2.1.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.774085 adafruit-circuitpython-dps310-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.774085 adafruit-circuitpython-dps310-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.774085 adafruit-circuitpython-dps310-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.774085 adafruit-circuitpython-dps310-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-08-26 02:13:57.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-26 02:13:57.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:13:57.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:13:57.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:13:57.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/
--rw-r--r--   0 runner    (1001) docker     (121)      377 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11459 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)     9996 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      409 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/examples/dps310_low_power_weather_station.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/examples/dps310_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/examples/dps310_simpletest_advanced.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-08-26 02:13:48.000000 adafruit-circuitpython-dps310-2.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:13:38.000000 adafruit-circuitpython-dps310-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:13:57.778085 adafruit-circuitpython-dps310-2.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.712842 adafruit-circuitpython-dps310-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.712842 adafruit-circuitpython-dps310-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4517 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5306 2022-09-27 14:51:21.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-09-27 14:51:21.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 14:51:21.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-09-27 14:51:21.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-27 14:51:21.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/
+-rw-r--r--   0 runner    (1001) docker     (121)      377 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11778 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10244 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      409 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5915 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      844 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1111 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/examples/dps310_low_power_weather_station.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/examples/dps310_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      391 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/examples/dps310_simpletest_advanced.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1261 2022-09-27 14:51:14.000000 adafruit-circuitpython-dps310-2.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-09-27 14:51:07.000000 adafruit-circuitpython-dps310-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 14:51:21.716842 adafruit-circuitpython-dps310-2.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-dps310-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dps310-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-dps310-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-dps310-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/.gitignore` & `adafruit-circuitpython-dps310-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-dps310-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/.pylintrc` & `adafruit-circuitpython-dps310-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dps310-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/LICENSE` & `adafruit-circuitpython-dps310-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dps310-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-dps310-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dps310-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/PKG-INFO` & `adafruit-circuitpython-dps310-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dps310
-Version: 2.1.8
+Version: 2.1.9
 Summary: Library for the DPS310 Precision Barometric Pressure Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DPS310
 Keywords: adafruit,blinka,circuitpython,micropython,dps310,pressure,sensor,barometric,altimeter,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dps310-2.1.8/README.rst` & `adafruit-circuitpython-dps310-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/PKG-INFO` & `adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dps310
-Version: 2.1.8
+Version: 2.1.9
 Summary: Library for the DPS310 Precision Barometric Pressure Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DPS310
 Keywords: adafruit,blinka,circuitpython,micropython,dps310,pressure,sensor,barometric,altimeter,altitude
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dps310-2.1.8/adafruit_circuitpython_dps310.egg-info/SOURCES.txt` & `adafruit-circuitpython-dps310-2.1.9/adafruit_circuitpython_dps310.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/advanced.py` & `adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/advanced.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,42 +28,49 @@
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DPS310.git"
 
 from time import sleep
 from micropython import const
 from adafruit_register.i2c_bits import RWBits
 from adafruit_dps310.basic import DPS310
 
+try:
+    from typing import Iterable, Optional, Tuple, Union
+except ImportError:
+    pass
+
 # pylint: disable=no-member,unnecessary-pass
 
 
 class CV:
     """struct helper"""
 
     @classmethod
-    def add_values(cls, value_tuples):
+    def add_values(
+        cls, value_tuples: Iterable[Tuple[str, int, Union[str, int], Optional[float]]]
+    ):
         """Add CV values to the class"""
         cls.string = {}
         cls.lsb = {}
 
         for value_tuple in value_tuples:
             name, value, string, lsb = value_tuple
             setattr(cls, name, value)
             cls.string[value] = string
             cls.lsb[value] = lsb
 
     @classmethod
-    def is_valid(cls, value):
+    def is_valid(cls, value: int) -> bool:
         """Validate that a given value is a member"""
         return value in cls.string
 
 
 class Mode(CV):
     """Options for ``mode``
 
@@ -192,15 +199,15 @@
             pressure = dps310.pressure
 
     """
     # Register definitions
     _pressure_ratebits = RWBits(3, _DPS310_PRSCFG, 4)
     _temp_ratebits = RWBits(3, _DPS310_TMPCFG, 4)
 
-    def initialize(self):
+    def initialize(self) -> None:
         """Initialize the sensor to continuous measurement"""
 
         self.reset()
 
         self.pressure_rate = Rate.RATE_64_HZ
         self.pressure_oversample_count = SampleCount.COUNT_64
         self.temperature_rate = Rate.RATE_64_HZ
@@ -208,19 +215,19 @@
         self.mode = Mode.CONT_PRESTEMP
 
         # wait until we have at least one good measurement
         self.wait_temperature_ready()
         self.wait_pressure_ready()
 
     @property
-    def temperature_ready(self):
+    def temperature_ready(self) -> bool:
         """Returns true if there is a temperature reading ready"""
         return self._temp_ready
 
-    def wait_temperature_ready(self):
+    def wait_temperature_ready(self) -> None:
         """Wait until a temperature measurement is available.
 
         To avoid waiting indefinitely this function raises an
         error if the sensor isn't configured for temperate measurements,
         ie. ``Mode.ONE_TEMPERATURE``, ``Mode.CONT_TEMP`` or ``Mode.CONT_PRESTEMP``.
         See the `Mode` documentation for details.
         """
@@ -229,19 +236,19 @@
                 "Sensor mode is set to idle or pressure measurement,\
                     can't wait for a temperature measurement"
             )
         while self._temp_ready is False:
             sleep(0.001)
 
     @property
-    def pressure_ready(self):
+    def pressure_ready(self) -> bool:
         """Returns true if pressure readings are ready"""
         return self._pressure_ready
 
-    def wait_pressure_ready(self):
+    def wait_pressure_ready(self) -> None:
         """Wait until a pressure measurement is available
 
         To avoid waiting indefinitely this function raises an
         error if the sensor isn't configured for pressure measurements,
         ie.  ``Mode.ONE_PRESSURE``, ``Mode.CONT_PRESSURE`` or ``Mode.CONT_PRESTEMP``
         See the `Mode` documentation for details.
         """
@@ -250,67 +257,67 @@
                 "Sensor mode is set to idle or temperature measurement,\
                     can't wait for a pressure measurement"
             )
         while self._pressure_ready is False:
             sleep(0.001)
 
     @property
-    def mode(self):
+    def mode(self) -> int:
         """The measurement mode. Must be a `Mode`. See the `Mode` documentation for details"""
         return self._mode_bits
 
     @mode.setter
-    def mode(self, value):
+    def mode(self, value: int) -> None:
         if not Mode.is_valid(value):
             raise AttributeError("mode must be an `Mode`")
 
         self._mode_bits = value
 
     @property
-    def pressure_rate(self):
+    def pressure_rate(self) -> int:
         """Configure the pressure measurement rate. Must be a `Rate`"""
         return self._pressure_ratebits
 
     @pressure_rate.setter
-    def pressure_rate(self, value):
+    def pressure_rate(self, value: int) -> None:
         if not Rate.is_valid(value):
             raise AttributeError("pressure_rate must be a Rate")
         self._pressure_ratebits = value
 
     @property
-    def pressure_oversample_count(self):
+    def pressure_oversample_count(self) -> int:
         """The number of samples taken per pressure measurement. Must be a ``SampleCount``"""
         return self._pressure_osbits
 
     @pressure_oversample_count.setter
-    def pressure_oversample_count(self, value):
+    def pressure_oversample_count(self, value: int) -> None:
         if not SampleCount.is_valid(value):
             raise AttributeError("pressure_oversample_count must be a SampleCount")
 
         self._pressure_osbits = value
         self._pressure_shiftbit = value > SampleCount.COUNT_8
         self._pressure_scale = self._oversample_scalefactor[value]
 
     @property
-    def temperature_rate(self):
+    def temperature_rate(self) -> int:
         """Configure the temperature measurement rate. Must be a `Rate`"""
         return self._temp_ratebits
 
     @temperature_rate.setter
-    def temperature_rate(self, value):
+    def temperature_rate(self, value: int) -> None:
         if not Rate.is_valid(value):
             raise AttributeError("temperature_rate must be a Rate")
         self._temp_ratebits = value
 
     @property
-    def temperature_oversample_count(self):
+    def temperature_oversample_count(self) -> int:
         """The number of samples taken per temperature measurement. Must be a ``SampleCount``"""
         return self._temp_osbits
 
     @temperature_oversample_count.setter
-    def temperature_oversample_count(self, value):
+    def temperature_oversample_count(self, value: int) -> None:
         if not SampleCount.is_valid(value):
             raise AttributeError("temperature_oversample_count must be a SampleCount")
 
         self._temp_osbits = value
         self._temp_scale = self._oversample_scalefactor[value]
         self._temp_shiftbit = value > SampleCount.COUNT_8
```

### Comparing `adafruit-circuitpython-dps310-2.1.8/adafruit_dps310/basic.py` & `adafruit-circuitpython-dps310-2.1.9/adafruit_dps310/basic.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,26 +27,32 @@
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
-__version__ = "2.1.8"
+__version__ = "2.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DPS310.git"
 
 # Common imports; remove if unused or pylint will complain
 import math
 from time import sleep
 from micropython import const
 from adafruit_bus_device import i2c_device
 from adafruit_register.i2c_struct import UnaryStruct, ROUnaryStruct
 from adafruit_register.i2c_bit import RWBit, ROBit
 from adafruit_register.i2c_bits import RWBits, ROBits
 
+try:
+    import typing  # pylint: disable=unused-import
+    from busio import I2C
+except ImportError:
+    pass
+
 _DPS310_DEFAULT_ADDRESS = const(0x77)  # DPS310 default i2c address
 _DPS310_DEVICE_ID = const(0x10)  # DPS310 device identifier
 
 _DPS310_PRSB2 = const(0x00)  # Highest byte of pressure data
 _DPS310_TMPB2 = const(0x03)  # Highest byte of temperature data
 _DPS310_PRSCFG = const(0x06)  # Pressure configuration
 _DPS310_TMPCFG = const(0x07)  # Temperature configuration
@@ -114,15 +120,15 @@
 
     _calib_coeff_temp_src_bit = ROBit(_DPS310_TMPCOEFSRCE, 7)
 
     _reg0e = RWBits(8, 0x0E, 0)
     _reg0f = RWBits(8, 0x0F, 0)
     _reg62 = RWBits(8, 0x62, 0)
 
-    def __init__(self, i2c_bus, address=_DPS310_DEFAULT_ADDRESS):
+    def __init__(self, i2c_bus: I2C, address: int = _DPS310_DEFAULT_ADDRESS) -> None:
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
 
         if self._device_id != _DPS310_DEVICE_ID:
             raise RuntimeError("Failed to find DPS310 - check your wiring!")
         self._pressure_scale = None
         self._temp_scale = None
         self._c0 = None
@@ -146,15 +152,15 @@
             1040384,
             2088960,
         )
         self._sea_level_pressure = 1013.25
 
         self.initialize()
 
-    def initialize(self):
+    def initialize(self) -> None:
         """Initialize the sensor to continuous measurement"""
 
         self.reset()
 
         self._pressure_osbits = 6
         self._pressure_shiftbit = True
         self._pressure_scale = self._oversample_scalefactor[6]
@@ -167,41 +173,41 @@
 
         # wait until we have at least one good measurement
         self.wait_temperature_ready()
         self.wait_pressure_ready()
 
     # (https://github.com/Infineon/DPS310-Pressure-Sensor#temperature-measurement-issue)
     # similar to DpsClass::correctTemp(void) from infineon's c++ library
-    def _correct_temp(self):
+    def _correct_temp(self) -> None:
         """Correct temperature readings on ICs with a fuse bit problem"""
         self._reg0e = 0xA5
         self._reg0f = 0x96
         self._reg62 = 0x02
         self._reg0e = 0
         self._reg0f = 0
 
         # perform a temperature measurement
         # the most recent temperature will be saved internally
         # and used for compensation when calculating pressure
         _unused = self._raw_temperature
 
-    def reset(self):
+    def reset(self) -> None:
         """Reset the sensor"""
         self._reset_register = 0x89
         # wait for hardware reset to finish
         sleep(0.010)
         while not self._sensor_ready:
             sleep(0.001)
         self._correct_temp()
         self._read_calibration()
         # make sure we're using the temperature source used for calibration
         self._temp_measurement_src_bit = self._calib_coeff_temp_src_bit
 
     @property
-    def pressure(self):
+    def pressure(self) -> float:
         """Returns the current pressure reading in hectoPascals (hPa)"""
 
         temp_reading = self._raw_temperature
         raw_temperature = self._twos_complement(temp_reading, 24)
 
         pressure_reading = self._raw_pressure
         raw_pressure = self._twos_complement(pressure_reading, 24)
@@ -217,61 +223,61 @@
             * (self._c01 + scaled_rawpres * (self._c11 + scaled_rawpres * self._c21))
         )
 
         final_pressure = pres_calc / 100
         return final_pressure
 
     @property
-    def altitude(self):
+    def altitude(self) -> float:
         """The altitude in meters based on the sea level pressure
         (:attr:`sea_level_pressure`) - which you must enter
         ahead of time
         """
         return 44330 * (
             1.0 - math.pow(self.pressure / self._sea_level_pressure, 0.1903)
         )
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """The current temperature reading in degrees Celsius"""
         _scaled_rawtemp = self._raw_temperature / self._temp_scale
         _temperature = _scaled_rawtemp * self._c1 + self._c0 / 2.0
         return _temperature
 
     @property
-    def sea_level_pressure(self):
+    def sea_level_pressure(self) -> float:
         """The local sea level pressure in hectoPascals (aka millibars). This is used
         for calculation of :attr:`altitude`. Values are typically in the range
         980 - 1030."""
         return self._sea_level_pressure
 
     @sea_level_pressure.setter
-    def sea_level_pressure(self, value):
+    def sea_level_pressure(self, value: float) -> None:
         self._sea_level_pressure = value
 
-    def wait_temperature_ready(self):
+    def wait_temperature_ready(self) -> None:
         """Wait until a temperature measurement is available."""
 
         while self._temp_ready is False:
             sleep(0.001)
 
-    def wait_pressure_ready(self):
+    def wait_pressure_ready(self) -> None:
         """Wait until a pressure measurement is available"""
 
         while self._pressure_ready is False:
             sleep(0.001)
 
     @staticmethod
-    def _twos_complement(val, bits):
+    def _twos_complement(val: int, bits: int) -> int:
         if val & (1 << (bits - 1)):
             val -= 1 << bits
 
         return val
 
-    def _read_calibration(self):
+    def _read_calibration(self) -> None:
 
         while not self._coefficients_ready:
             sleep(0.001)
 
         buffer = bytearray(19)
         coeffs = [None] * 18
         for offset in range(18):
```

### Comparing `adafruit-circuitpython-dps310-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-dps310-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/docs/conf.py` & `adafruit-circuitpython-dps310-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/docs/examples.rst` & `adafruit-circuitpython-dps310-2.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/docs/index.rst` & `adafruit-circuitpython-dps310-2.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/examples/dps310_low_power_weather_station.py` & `adafruit-circuitpython-dps310-2.1.9/examples/dps310_low_power_weather_station.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dps310-2.1.8/pyproject.toml` & `adafruit-circuitpython-dps310-2.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dps310"
 description = "Library for the DPS310 Precision Barometric Pressure Sensor"
-version = "2.1.8"
+version = "2.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DPS310"}
 keywords = [
     "adafruit",
```

