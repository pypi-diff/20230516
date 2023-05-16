# Comparing `tmp/adafruit-circuitpython-il91874-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-il91874-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-il91874-1.2.8.tar", last modified: Mon Aug 22 18:40:41 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-il91874-1.2.9.tar", last modified: Wed Aug 24 23:35:26 2022, max compression
```

## Comparing `adafruit-circuitpython-il91874-1.2.8.tar` & `adafruit-circuitpython-il91874-1.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.620598 adafruit-circuitpython-il91874-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.604598 adafruit-circuitpython-il91874-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.608598 adafruit-circuitpython-il91874-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.612598 adafruit-circuitpython-il91874-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.612598 adafruit-circuitpython-il91874-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-08-22 18:40:41.620598 adafruit-circuitpython-il91874-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.616598 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-08-22 18:40:41.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      988 2022-08-22 18:40:41.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:40:41.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-22 18:40:41.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:40:41.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3465 2022-08-22 18:40:34.000000 adafruit-circuitpython-il91874-1.2.8/adafruit_il91874.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.616598 adafruit-circuitpython-il91874-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.616598 adafruit-circuitpython-il91874-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5425 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:41.620598 adafruit-circuitpython-il91874-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   360122 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-08-22 18:40:34.000000 adafruit-circuitpython-il91874-1.2.8/examples/il91874_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-22 18:40:34.000000 adafruit-circuitpython-il91874-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:40:26.000000 adafruit-circuitpython-il91874-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:40:41.620598 adafruit-circuitpython-il91874-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.130930 adafruit-circuitpython-il91874-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.134930 adafruit-circuitpython-il91874-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.134930 adafruit-circuitpython-il91874-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.134930 adafruit-circuitpython-il91874-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3599 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.134930 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4373 2022-08-24 23:35:26.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      988 2022-08-24 23:35:26.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 23:35:26.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-24 23:35:26.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-24 23:35:26.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3493 2022-08-24 23:35:17.000000 adafruit-circuitpython-il91874-1.2.9/adafruit_il91874.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)   360122 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)     2020 2022-08-24 23:35:17.000000 adafruit-circuitpython-il91874-1.2.9/examples/il91874_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-24 23:35:17.000000 adafruit-circuitpython-il91874-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-24 23:35:09.000000 adafruit-circuitpython-il91874-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-24 23:35:26.138930 adafruit-circuitpython-il91874-1.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-il91874-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-il91874-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-il91874-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-il91874-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/.gitignore` & `adafruit-circuitpython-il91874-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-il91874-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/.pylintrc` & `adafruit-circuitpython-il91874-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-il91874-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/LICENSE` & `adafruit-circuitpython-il91874-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-il91874-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-il91874-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-il91874-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/PKG-INFO` & `adafruit-circuitpython-il91874-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il91874
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython `displayio` driver for IL91874-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IL91874
 Keywords: adafruit,blinka,circuitpython,micropython,il91874,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-il91874-1.2.8/README.rst` & `adafruit-circuitpython-il91874-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/PKG-INFO` & `adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il91874
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython `displayio` driver for IL91874-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IL91874
 Keywords: adafruit,blinka,circuitpython,micropython,il91874,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-il91874-1.2.8/adafruit_circuitpython_il91874.egg-info/SOURCES.txt` & `adafruit-circuitpython-il91874-1.2.9/adafruit_circuitpython_il91874.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/adafruit_il91874.py` & `adafruit-circuitpython-il91874-1.2.9/adafruit_il91874.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_IL91874.git"
 
 _START_SEQUENCE = (
     b"\x04\x00"  # Power on
     b"\x00\x01\xaf"  # panel setting
     b"\x30\x01\x3a"  # PLL
     b"\x01\x05\x03\x00\x2b\x2b\x09"  # power setting
@@ -65,15 +65,15 @@
 
 _STOP_SEQUENCE = b"\x02\x01\x17"  # Power off
 
 # pylint: disable=too-few-public-methods
 class IL91874(displayio.EPaperDisplay):
     """IL91874 display driver"""
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.FourWire, **kwargs) -> None:
         start_sequence = bytearray(_START_SEQUENCE)
 
         width = kwargs["width"]
         height = kwargs["height"]
         if "rotation" in kwargs and kwargs["rotation"] % 180 != 0:
             width, height = height, width
         start_sequence[-7] = (width >> 8) & 0xFF
```

### Comparing `adafruit-circuitpython-il91874-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-il91874-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/docs/conf.py` & `adafruit-circuitpython-il91874-1.2.9/docs/conf.py`

 * *Files 5% similar despite different names*

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
@@ -39,15 +40,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit IL91874 Library"
-copyright = "2019 Scott Shawcroft"
+creation_year = "2019"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Scott Shawcroft"
 author = "Scott Shawcroft"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-il91874-1.2.8/docs/index.rst` & `adafruit-circuitpython-il91874-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/examples/display-ruler.bmp` & `adafruit-circuitpython-il91874-1.2.9/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/examples/il91874_simpletest.py` & `adafruit-circuitpython-il91874-1.2.9/examples/il91874_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il91874-1.2.8/pyproject.toml` & `adafruit-circuitpython-il91874-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-il91874"
 description = "CircuitPython `displayio` driver for IL91874-based ePaper displays"
-version = "1.2.8"
+version = "1.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IL91874"}
 keywords = [
     "adafruit",
```

