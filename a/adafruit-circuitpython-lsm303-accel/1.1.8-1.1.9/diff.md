# Comparing `tmp/adafruit-circuitpython-lsm303-accel-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-lsm303-accel-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lsm303-accel-1.1.8.tar", last modified: Mon Nov 15 17:51:07 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-lsm303-accel-1.1.9.tar", last modified: Mon Jan  3 20:58:14 2022, max compression
```

## Comparing `adafruit-circuitpython-lsm303-accel-1.1.8.tar` & `adafruit-circuitpython-lsm303-accel-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.478771 adafruit-circuitpython-lsm303-accel-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.478771 adafruit-circuitpython-lsm303-accel-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.478771 adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.478771 adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2961 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3825 2021-11-15 17:51:07.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1036 2021-11-15 17:51:07.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 17:51:07.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-15 17:51:07.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-15 17:51:07.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    13389 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_lsm303_accel.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      131 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1380 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      445 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_fast.py
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_inclinometer.py
--rw-r--r--   0 runner    (1001) docker     (121)      528 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      369 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_tap_detection.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 17:51:07.482771 adafruit-circuitpython-lsm303-accel-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2058 2021-11-15 17:50:56.000000 adafruit-circuitpython-lsm303-accel-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.232849 adafruit-circuitpython-lsm303-accel-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.232849 adafruit-circuitpython-lsm303-accel-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.232849 adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.232849 adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2961 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3825 2022-01-03 20:58:14.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1036 2022-01-03 20:58:14.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 20:58:14.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-01-03 20:58:14.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-01-03 20:58:14.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    13332 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_lsm303_accel.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      131 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1380 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      445 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_fast.py
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_inclinometer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      528 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      369 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_tap_detection.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 20:58:14.236849 adafruit-circuitpython-lsm303-accel-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2058 2022-01-03 20:58:00.000000 adafruit-circuitpython-lsm303-accel-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lsm303-accel-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-lsm303-accel-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-lsm303-accel-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/.pylintrc` & `adafruit-circuitpython-lsm303-accel-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lsm303-accel-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/LICENSE` & `adafruit-circuitpython-lsm303-accel-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lsm303-accel-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/PKG-INFO` & `adafruit-circuitpython-lsm303-accel-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm303-accel
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for LSM303 's 3-axis accelerometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LSM303_Accel
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit lsm303 6dof 6-dof accelerometer axisbreakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/README.rst` & `adafruit-circuitpython-lsm303-accel-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/PKG-INFO` & `adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm303-accel
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for LSM303 's 3-axis accelerometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LSM303_Accel
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit lsm303 6dof 6-dof accelerometer axisbreakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_circuitpython_lsm303_accel.egg-info/SOURCES.txt` & `adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_circuitpython_lsm303_accel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/adafruit_lsm303_accel.py` & `adafruit-circuitpython-lsm303-accel-1.1.9/adafruit_lsm303_accel.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,18 +25,16 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
+import struct
+
 from micropython import const
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register.i2c_struct import UnaryStruct
 from adafruit_register.i2c_bit import RWBit, ROBit
 from adafruit_register.i2c_bits import RWBits
 from adafruit_register.i2c_struct_array import StructArray
```

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-lsm303-accel-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/docs/conf.py` & `adafruit-circuitpython-lsm303-accel-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/docs/examples.rst` & `adafruit-circuitpython-lsm303-accel-1.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/docs/index.rst` & `adafruit-circuitpython-lsm303-accel-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_inclinometer.py` & `adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_inclinometer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/examples/lsm303_accel_simpletest.py` & `adafruit-circuitpython-lsm303-accel-1.1.9/examples/lsm303_accel_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm303-accel-1.1.8/setup.py` & `adafruit-circuitpython-lsm303-accel-1.1.9/setup.py`

 * *Files identical despite different names*

