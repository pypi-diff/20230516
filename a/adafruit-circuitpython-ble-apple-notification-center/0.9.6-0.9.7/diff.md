# Comparing `tmp/adafruit-circuitpython-ble-apple-notification-center-0.9.6.tar.gz` & `tmp/adafruit-circuitpython-ble-apple-notification-center-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-apple-notification-center-0.9.6.tar", last modified: Mon Nov 15 18:35:58 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-apple-notification-center-0.9.7.tar", last modified: Fri Feb  4 19:54:02 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6.tar` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.930774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.930774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.930774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2607 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      205 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.930774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3845 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     8639 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_ble_apple_notification_center.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.930774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4742 2021-11-15 18:35:58.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-11-15 18:35:58.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:35:58.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-11-15 18:35:58.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-11-15 18:35:58.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/examples/ble_apple_notification_center_new.py
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/examples/ble_apple_notification_center_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:35:58.934774 adafruit-circuitpython-ble-apple-notification-center-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2107 2021-11-15 18:35:47.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.915499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3833 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     8639 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_ble_apple_notification_center.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4630 2022-02-04 19:54:02.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-02-04 19:54:02.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 19:54:02.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-02-04 19:54:02.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-02-04 19:54:02.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5619 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/examples/ble_apple_notification_center_new.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/examples/ble_apple_notification_center_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 19:54:02.919499 adafruit-circuitpython-ble-apple-notification-center-0.9.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2009 2022-02-04 19:53:49.000000 adafruit-circuitpython-ble-apple-notification-center-0.9.7/setup.py
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # SPDX-FileCopyrightText: 2021 Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 Thank you for contributing! Before you submit a pull request, please read the following.
 
-Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://circuitpython.readthedocs.io/en/latest/docs/design_guide.html
+Make sure any changes you're submitting are in line with the CircuitPython Design Guide, available here: https://docs.circuitpython.org/en/latest/docs/design_guide.html
 
 If your changes are to documentation, please verify that the documentation builds locally by following the steps found here: https://adafru.it/build-docs
 
 Before submitting the pull request, make sure you've run Pylint and Black locally on your code. You can do this manually or using pre-commit. Instructions are available here: https://adafru.it/check-your-code
 
 Please remove all of this text before submitting. Include an explanation or list of changes included in your PR, as well as, if applicable, a link to any related issues.
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/build.yml` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/build.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/.github/workflows/release.yml` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,18 +20,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.7
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.7
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - uses: actions/checkout@v1
       with:
         submodules: true
     - name: Install deps
@@ -59,15 +59,15 @@
     - uses: actions/checkout@v1
     - name: Check For setup.py
       id: need-pypi
       run: |
         echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
     - name: Set up Python
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v2
       with:
         python-version: '3.x'
     - name: Install dependencies
       if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
       run: |
         python -m pip install --upgrade pip
         pip install setuptools wheel twine
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/.pylintrc` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSE` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/PKG-INFO` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-apple-notification-center
-Version: 0.9.6
+Version: 0.9.7
 Summary: BLE library for the Apple Notification Center
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_apple_notification_center ble ancs apple notification
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_apple_notification_center/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/
+    :target: https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/workflows/Build%20CI/badge.svg
@@ -115,15 +113,15 @@
         for notification_id in ans.active_notifications:
             notification = ans.active_notifications[notification_id]
             print(notification.app_id, notification.title)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/README.rst` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_apple_notification_center/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/
+    :target: https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/workflows/Build%20CI/badge.svg
@@ -94,15 +94,15 @@
         for notification_id in ans.active_notifications:
             notification = ans.active_notifications[notification_id]
             print(notification.app_id, notification.title)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_ble_apple_notification_center.py` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_ble_apple_notification_center.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-apple-notification-center
-Version: 0.9.6
+Version: 0.9.7
 Summary: BLE library for the Apple Notification Center
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ble_apple_notification_center ble ancs apple notification
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_apple_notification_center/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/
+    :target: https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/workflows/Build%20CI/badge.svg
@@ -115,15 +113,15 @@
         for notification_id in ans.active_notifications:
             notification = ans.active_notifications[notification_id]
             print(notification.app_id, notification.title)
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ble_apple_notification_center/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_apple_notification_center/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/adafruit_circuitpython_ble_apple_notification_center.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/adafruit_circuitpython_ble_apple_notification_center.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/conf.py` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = ["bleak"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "python": ("https://docs.python.org/3", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/docs/index.rst` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/docs/index.rst`

 * *Files 12% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     CircuitPlayground Bluefruit <https://www.adafruit.com/product/4333>
     Feather nRF52840 <https://www.adafruit.com/product/4062>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Apple_Notification_Center/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/examples/ble_apple_notification_center_new.py` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/examples/ble_apple_notification_center_new.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/examples/ble_apple_notification_center_simpletest.py` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/examples/ble_apple_notification_center_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-apple-notification-center-0.9.6/setup.py` & `adafruit-circuitpython-ble-apple-notification-center-0.9.7/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,16 +40,14 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
         "Topic :: System :: Hardware",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
     ],
     # What does your project relate to?
     keywords="adafruit blinka circuitpython micropython ble_apple_notification_center ble "
     "ancs apple notification",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     # TODO: IF LIBRARY FILES ARE A PACKAGE FOLDER,
```

