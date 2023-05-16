# Comparing `tmp/adafruit-circuitpython-bluefruitspi-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-bluefruitspi-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bluefruitspi-1.1.8.tar", last modified: Fri Feb  4 20:37:09 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-bluefruitspi-1.1.9.tar", last modified: Mon Mar 28 19:13:13 2022, max compression
```

## Comparing `adafruit-circuitpython-bluefruitspi-1.1.8.tar` & `adafruit-circuitpython-bluefruitspi-1.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.983782 adafruit-circuitpython-bluefruitspi-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.983782 adafruit-circuitpython-bluefruitspi-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.983782 adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.983782 adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5398 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4624 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    13406 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_bluefruitspi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5398 2022-02-04 20:37:09.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-02-04 20:37:09.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:37:09.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:37:09.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-02-04 20:37:09.000000 adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      271 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_neocolorpicker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_ruggedechotest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:37:09.987782 adafruit-circuitpython-bluefruitspi-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-02-04 20:36:58.000000 adafruit-circuitpython-bluefruitspi-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.728493 adafruit-circuitpython-bluefruitspi-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.720493 adafruit-circuitpython-bluefruitspi-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1105 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-03-28 19:13:13.728493 adafruit-circuitpython-bluefruitspi-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4595 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    13410 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_bluefruitspi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5369 2022-03-28 19:13:13.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-03-28 19:13:13.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-28 19:13:13.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-03-28 19:13:13.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-28 19:13:13.000000 adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.724493 adafruit-circuitpython-bluefruitspi-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      271 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      968 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-28 19:13:13.728493 adafruit-circuitpython-bluefruitspi-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3198 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_neocolorpicker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3268 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_ruggedechotest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-28 19:13:13.728493 adafruit-circuitpython-bluefruitspi-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1897 2022-03-28 19:13:00.000000 adafruit-circuitpython-bluefruitspi-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bluefruitspi-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-bluefruitspi-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-bluefruitspi-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/.pylintrc` & `adafruit-circuitpython-bluefruitspi-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bluefruitspi-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/LICENSE` & `adafruit-circuitpython-bluefruitspi-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bluefruitspi-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/PKG-INFO` & `adafruit-circuitpython-bluefruitspi-1.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bluefruitspi
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython helper class to work with the Adafruit Bluefruit LE SPI Friend.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BluefruitSPI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit ble bluetooth bluefruit spi friend hardware micropython circuitpython
 Platform: UNKNOWN
@@ -138,20 +138,17 @@
         print("Connection lost.")
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bluefruitspi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BluefruitSPI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/README.rst` & `adafruit-circuitpython-bluefruitspi-1.1.9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -119,18 +119,15 @@
         print("Connection lost.")
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bluefruitspi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BluefruitSPI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_bluefruitspi.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_bluefruitspi.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,14 +158,15 @@
             self._keycode_template[2], _KEY_CODE_CMD[32:48], False  #  0-00-00-00\n
         )
 
     def send_keyboard_code(self, evt):
         """
         Put an AT+BLEKEYBOARDCODE command into the FIFO buffer.
         Call pop_keyboard_code() to send a single packet to the Bluefruit.
+
         :param evt: bytearray(8) representing keyboard code to send
         """
         evt = ba.hexlify(evt)
         self._keycode_template[1][7:9] = evt[0:2]
         # self._keycode_template[1][10:12] = evt[2:4]  # Should always be 0
         self._keycode_template[1][13:15] = evt[4:6]
         self._keycode_template[1][16:18] = evt[6:8]
@@ -184,14 +185,15 @@
             with self._spi_device as spi:
                 spi.write(data, end=24)
 
     @staticmethod
     def _create_sdep_raw(dest, payload, more):
         """
         Create an SDEP packet
+
         :param dest: bytearray(20) to place SDEP packet in
         :param payload: iterable with length <= 16 containing the payload data
         :param more: True to set the more bit, False otherwise
         """
         _more = 0x80 if more else 0
         plen = len(payload)
         struct.pack_into(
@@ -206,14 +208,15 @@
 
     def _cmd(self, cmd):  # pylint: disable=too-many-branches
         """
         Executes the supplied AT command, which must be terminated with
         a new-line character.
         Returns msgtype, rspid, rsp, which are 8-bit int, 16-bit int and a
         bytearray.
+
         :param cmd: The new-line terminated AT command to execute.
         """
         # Make sure we stay within the 255 byte limit
         if len(cmd) > 127:
             if self._debug:
                 print("ERROR: Command too long.")
             raise ValueError("Command too long.")
@@ -298,14 +301,15 @@
     def connected(self):
         """Whether the Bluefruit module is connected to the central"""
         return int(self.command_check_OK(b"AT+GAPGETCONN")) == 1
 
     def uart_tx(self, data):
         """
         Sends the specific bytestring out over BLE UART.
+
         :param data: The bytestring to send.
         """
         return self._cmd(b"AT+BLEUARTTX=" + data + b"\r\n")
 
     def uart_rx(self):
         """
         Reads byte data from the BLE UART FIFO.
```

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/PKG-INFO` & `adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bluefruitspi
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython helper class to work with the Adafruit Bluefruit LE SPI Friend.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BluefruitSPI
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit ble bluetooth bluefruit spi friend hardware micropython circuitpython
 Platform: UNKNOWN
@@ -138,20 +138,17 @@
         print("Connection lost.")
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/bluefruitspi/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BluefruitSPI/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/adafruit_circuitpython_bluefruitspi.egg-info/SOURCES.txt` & `adafruit-circuitpython-bluefruitspi-1.1.9/adafruit_circuitpython_bluefruitspi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-bluefruitspi-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/docs/conf.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/docs/index.rst` & `adafruit-circuitpython-bluefruitspi-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_neocolorpicker.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_neocolorpicker.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_ruggedechotest.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_ruggedechotest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/examples/bluefruitspi_simpletest.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/examples/bluefruitspi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bluefruitspi-1.1.8/setup.py` & `adafruit-circuitpython-bluefruitspi-1.1.9/setup.py`

 * *Files identical despite different names*

