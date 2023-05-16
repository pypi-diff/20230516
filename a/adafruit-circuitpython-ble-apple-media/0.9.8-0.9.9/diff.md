# Comparing `tmp/adafruit-circuitpython-ble-apple-media-0.9.8.tar.gz` & `tmp/adafruit-circuitpython-ble-apple-media-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-apple-media-0.9.8.tar", last modified: Tue Jun  7 17:21:56 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-apple-media-0.9.9.tar", last modified: Thu Jun  9 18:43:25 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-apple-media-0.9.8.tar` & `adafruit-circuitpython-ble-apple-media-0.9.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.083287 adafruit-circuitpython-ble-apple-media-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.091287 adafruit-circuitpython-ble-apple-media-0.9.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.091287 adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.091287 adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     9707 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_ble_apple_media.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-06-07 17:21:56.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-06-07 17:21:56.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:21:56.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:21:56.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-07 17:21:56.000000 adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1077 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/examples/ble_apple_media_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:21:56.095287 adafruit-circuitpython-ble-apple-media-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-06-07 17:21:42.000000 adafruit-circuitpython-ble-apple-media-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.511502 adafruit-circuitpython-ble-apple-media-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.503502 adafruit-circuitpython-ble-apple-media-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.503502 adafruit-circuitpython-ble-apple-media-0.9.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.503502 adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     9707 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_ble_apple_media.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4315 2022-06-09 18:43:25.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      950 2022-06-09 18:43:25.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:43:25.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 18:43:25.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-06-09 18:43:25.000000 adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5472 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:43:25.507502 adafruit-circuitpython-ble-apple-media-0.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/examples/ble_apple_media_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:43:25.511502 adafruit-circuitpython-ble-apple-media-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1942 2022-06-09 18:43:10.000000 adafruit-circuitpython-ble-apple-media-0.9.9/setup.py
```

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-apple-media-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-ble-apple-media-0.9.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.gitignore` & `adafruit-circuitpython-ble-apple-media-0.9.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-apple-media-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/.pylintrc` & `adafruit-circuitpython-ble-apple-media-0.9.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-apple-media-0.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/LICENSE` & `adafruit-circuitpython-ble-apple-media-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-apple-media-0.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/PKG-INFO` & `adafruit-circuitpython-ble-apple-media-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-apple-media
-Version: 0.9.8
+Version: 0.9.9
 Summary: Support for the Apple Media Service which provides media playback info and control.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Media
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_apple_media apple media ble
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/README.rst` & `adafruit-circuitpython-ble-apple-media-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_ble_apple_media.py` & `adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_ble_apple_media.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-apple-media
-Version: 0.9.8
+Version: 0.9.9
 Summary: Support for the Apple Media Service which provides media playback info and control.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Media
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_apple_media apple media ble
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/adafruit_circuitpython_ble_apple_media.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-apple-media-0.9.9/adafruit_circuitpython_ble_apple_media.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-apple-media-0.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/docs/conf.py` & `adafruit-circuitpython-ble-apple-media-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/docs/index.rst` & `adafruit-circuitpython-ble-apple-media-0.9.9/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     Adafruit Feather nRF52840 Express <https://www.adafruit.com/product/4062>
 
     Adafruit ItsyBitsy nRF52840 Express - Bluetooth LE <https://www.adafruit.com/product/4481>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Media/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Media/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/examples/ble_apple_media_simpletest.py` & `adafruit-circuitpython-ble-apple-media-0.9.9/examples/ble_apple_media_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-media-0.9.8/setup.py` & `adafruit-circuitpython-ble-apple-media-0.9.9/setup.py`

 * *Files identical despite different names*

