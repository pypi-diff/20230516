# Comparing `tmp/adafruit-circuitpython-ble-lywsd03mmc-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-ble-lywsd03mmc-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-lywsd03mmc-1.0.8.tar", last modified: Thu Jun  9 17:58:03 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-lywsd03mmc-1.0.9.tar", last modified: Mon Aug  8 00:31:49 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8.tar` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.227680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.231680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.231680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.231680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2552 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     2760 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_ble_lywsd03mmc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.231680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-06-09 17:58:03.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-06-09 17:58:03.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 17:58:03.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-09 17:58:03.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-06-09 17:58:03.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5623 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/examples/ble_lywsd03mmc_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 17:58:03.235680 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-09 17:57:47.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.463834 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.467835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.467835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.467835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2554 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_ble_lywsd03mmc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.467835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3340 2022-08-08 00:31:49.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-08-08 00:31:49.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-08 00:31:49.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-08-08 00:31:49.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-08 00:31:49.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5623 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      994 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/examples/ble_lywsd03mmc_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-08 00:31:49.471835 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-08-08 00:31:28.000000 adafruit-circuitpython-ble-lywsd03mmc-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.gitignore` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/.pylintrc` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSE` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/PKG-INFO` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-lywsd03mmc
-Version: 1.0.8
+Version: 1.0.9
 Summary: BLE Support for Xiaomi LYWSD03MMC Thermometer/Hygrometer
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_LYWSD03MMC
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_lywsd03mmc ble lywsd03mmc xiaomi mijia thermometer hygrometer
 Platform: UNKNOWN
@@ -66,16 +66,16 @@
     sudo pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_lywsd03mmc/en/latest/>`_.
```

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/README.rst` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     sudo pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_lywsd03mmc/en/latest/>`_.
```

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_ble_lywsd03mmc.py` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_ble_lywsd03mmc.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,16 +71,12 @@
     def temperature_humidity(self) -> Optional[Tuple[float, int]]:
         """Return a tuple of (temperature, humidity)."""
         if self._readings_buf is None:
             self._readings_buf = bytearray(self.readings.incoming_packet_length)
         data = self._readings_buf
         length = self.readings.readinto(data)
         if length > 0:
-            low_temp, high_temp, hum = struct.unpack_from("<BBB", data)
-            sign = high_temp & 0x80
-            temp = ((high_temp & 0x7F) << 8) | low_temp
-            if sign:
-                temp = temp - 32767
+            temp, hum = struct.unpack_from("<hB", data)
             temp = temp / 100
             return (temp, hum)
         # No data.
         return None
```

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-lywsd03mmc
-Version: 1.0.8
+Version: 1.0.9
 Summary: BLE Support for Xiaomi LYWSD03MMC Thermometer/Hygrometer
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_LYWSD03MMC
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_lywsd03mmc ble lywsd03mmc xiaomi mijia thermometer hygrometer
 Platform: UNKNOWN
@@ -66,16 +66,16 @@
     sudo pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-lywsd03mmc
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_lywsd03mmc/en/latest/>`_.
```

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/adafruit_circuitpython_ble_lywsd03mmc.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/adafruit_circuitpython_ble_lywsd03mmc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/conf.py` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/docs/index.rst` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/examples/ble_lywsd03mmc_simpletest.py` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/examples/ble_lywsd03mmc_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-lywsd03mmc-1.0.8/setup.py` & `adafruit-circuitpython-ble-lywsd03mmc-1.0.9/setup.py`

 * *Files identical despite different names*

