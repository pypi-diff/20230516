# Comparing `tmp/adafruit-circuitpython-fingerprint-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-fingerprint-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fingerprint-2.2.8.tar", last modified: Mon Aug 22 18:39:14 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-fingerprint-2.2.9.tar", last modified: Fri Aug 26 02:23:42 2022, max compression
```

## Comparing `adafruit-circuitpython-fingerprint-2.2.8.tar` & `adafruit-circuitpython-fingerprint-2.2.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.289806 adafruit-circuitpython-fingerprint-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-08-22 18:39:14.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-22 18:39:14.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:39:14.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-22 18:39:14.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-22 18:39:14.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19588 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/adafruit_fingerprint.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5371 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     6552 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_r503.py
--rw-r--r--   0 runner    (1001) docker     (121)     9311 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_r503_rpi.py
--rw-r--r--   0 runner    (1001) docker     (121)     6094 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_simpletest_rpi.py
--rw-r--r--   0 runner    (1001) docker     (121)     7088 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_template_file_compare.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-22 18:39:06.000000 adafruit-circuitpython-fingerprint-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-22 18:38:56.000000 adafruit-circuitpython-fingerprint-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:39:14.293806 adafruit-circuitpython-fingerprint-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.425984 adafruit-circuitpython-fingerprint-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.425984 adafruit-circuitpython-fingerprint-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.425984 adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.425984 adafruit-circuitpython-fingerprint-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2666 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.425984 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-08-26 02:23:42.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-08-26 02:23:42.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:23:42.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-26 02:23:42.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-08-26 02:23:42.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19588 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/adafruit_fingerprint.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5591 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      196 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1039 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     6552 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_r503.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9311 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_r503_rpi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6094 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8257 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_simpletest_rpi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7088 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_template_file_compare.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-26 02:23:34.000000 adafruit-circuitpython-fingerprint-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-08-26 02:23:25.000000 adafruit-circuitpython-fingerprint-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:23:42.429984 adafruit-circuitpython-fingerprint-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fingerprint-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-fingerprint-2.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.gitignore` & `adafruit-circuitpython-fingerprint-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-fingerprint-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/.pylintrc` & `adafruit-circuitpython-fingerprint-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fingerprint-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/LICENSE` & `adafruit-circuitpython-fingerprint-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fingerprint-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-fingerprint-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fingerprint-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/PKG-INFO` & `adafruit-circuitpython-fingerprint-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fingerprint
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for UART fingerprint sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Fingerprint
 Keywords: adafruit,uart,fingerprint,finger,print,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/README.rst` & `adafruit-circuitpython-fingerprint-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/PKG-INFO` & `adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fingerprint
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for UART fingerprint sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Fingerprint
 Keywords: adafruit,uart,fingerprint,finger,print,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/adafruit_circuitpython_fingerprint.egg-info/SOURCES.txt` & `adafruit-circuitpython-fingerprint-2.2.9/adafruit_circuitpython_fingerprint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/adafruit_fingerprint.py` & `adafruit-circuitpython-fingerprint-2.2.9/adafruit_fingerprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     pass
 
 import struct
 
 from micropython import const
 from busio import UART
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Fingerprint.git"
 
 _STARTCODE = const(0xEF01)
 _COMMANDPACKET = const(0x1)
 _DATAPACKET = const(0x2)
 _ACKPACKET = const(0x7)
 _ENDDATAPACKET = const(0x8)
```

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-fingerprint-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/docs/conf.py` & `adafruit-circuitpython-fingerprint-2.2.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -36,15 +37,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit Fingerprint Library"
-copyright = "2017 ladyada"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/docs/index.rst` & `adafruit-circuitpython-fingerprint-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_r503.py` & `adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_r503.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_r503_rpi.py` & `adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_r503_rpi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_simpletest.py` & `adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_simpletest_rpi.py` & `adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_simpletest_rpi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/examples/fingerprint_template_file_compare.py` & `adafruit-circuitpython-fingerprint-2.2.9/examples/fingerprint_template_file_compare.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fingerprint-2.2.8/pyproject.toml` & `adafruit-circuitpython-fingerprint-2.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-fingerprint"
 description = "CircuitPython library for UART fingerprint sensor."
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Fingerprint"}
 keywords = [
     "adafruit",
```

