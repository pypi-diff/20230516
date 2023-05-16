# Comparing `tmp/adafruit-circuitpython-crickit-2.3.8.tar.gz` & `tmp/adafruit-circuitpython-crickit-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-crickit-2.3.8.tar", last modified: Tue Jun  7 17:08:07 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-crickit-2.3.9.tar", last modified: Thu Jun  9 18:27:48 2022, max compression
```

## Comparing `adafruit-circuitpython-crickit-2.3.8.tar` & `adafruit-circuitpython-crickit-2.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.888230 adafruit-circuitpython-crickit-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.888230 adafruit-circuitpython-crickit-2.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.888230 adafruit-circuitpython-crickit-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.888230 adafruit-circuitpython-crickit-2.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-06-07 17:08:07.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-06-07 17:08:07.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:08:07.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-07 17:08:07.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-07 17:08:07.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)    12440 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/adafruit_crickit.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/api.rst.license
--rwxr-xr-x   0 runner    (1001) docker     (121)     5587 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1187 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_continuous_servo_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      393 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_dc_motor_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      505 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_drive_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_multi_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      851 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_neopixel_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      329 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_servo_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      412 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_signal_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_stepper_motor_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/examples/crickit_touch_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      178 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:08:07.892230 adafruit-circuitpython-crickit-2.3.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1910 2022-06-07 17:07:51.000000 adafruit-circuitpython-crickit-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.600753 adafruit-circuitpython-crickit-2.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.604753 adafruit-circuitpython-crickit-2.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4264 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4996 2022-06-09 18:27:48.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-06-09 18:27:48.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:27:48.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-09 18:27:48.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:27:48.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12440 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/adafruit_crickit.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/api.rst.license
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5587 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      148 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_continuous_servo_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_dc_motor_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      505 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_drive_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1497 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_multi_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_neopixel_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      329 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_servo_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      412 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_signal_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_stepper_motor_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/examples/crickit_touch_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      178 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:27:48.608753 adafruit-circuitpython-crickit-2.3.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1910 2022-06-09 18:27:37.000000 adafruit-circuitpython-crickit-2.3.9/setup.py
```

### Comparing `adafruit-circuitpython-crickit-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-crickit-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-crickit-2.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-crickit-2.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/.gitignore` & `adafruit-circuitpython-crickit-2.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-crickit-2.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/.pylintrc` & `adafruit-circuitpython-crickit-2.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-crickit-2.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/LICENSE` & `adafruit-circuitpython-crickit-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-crickit-2.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-crickit-2.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-crickit-2.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/PKG-INFO` & `adafruit-circuitpython-crickit-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-crickit
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for controlling a Crickit robotics board.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Crickit
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit crickit robotics hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-crickit-2.3.8/README.rst` & `adafruit-circuitpython-crickit-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/PKG-INFO` & `adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-crickit
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for controlling a Crickit robotics board.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Crickit
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit crickit robotics hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-crickit-2.3.8/adafruit_circuitpython_crickit.egg-info/SOURCES.txt` & `adafruit-circuitpython-crickit-2.3.9/adafruit_circuitpython_crickit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/adafruit_crickit.py` & `adafruit-circuitpython-crickit-2.3.9/adafruit_crickit.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-crickit-2.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/docs/conf.py` & `adafruit-circuitpython-crickit-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/docs/index.rst` & `adafruit-circuitpython-crickit-2.3.9/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     Adafruit Crickit for Circuit Playground Express <https://www.adafruit.com/3093>
     Adafruit Crickit FeatherWing <https://www.adafruit.com/3343>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_Crickit/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_Crickit/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-crickit-2.3.8/examples/crickit_multi_example.py` & `adafruit-circuitpython-crickit-2.3.9/examples/crickit_multi_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/examples/crickit_neopixel_simpletest.py` & `adafruit-circuitpython-crickit-2.3.9/examples/crickit_neopixel_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-crickit-2.3.8/setup.py` & `adafruit-circuitpython-crickit-2.3.9/setup.py`

 * *Files identical despite different names*

