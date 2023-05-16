# Comparing `tmp/adafruit-circuitpython-max31856-0.9.8.tar.gz` & `tmp/adafruit-circuitpython-max31856-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-max31856-0.9.8.tar", last modified: Mon Nov 15 17:52:15 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-max31856-0.9.9.tar", last modified: Fri Feb  4 20:16:24 2022, max compression
```

## Comparing `adafruit-circuitpython-max31856-0.9.8.tar` & `adafruit-circuitpython-max31856-0.9.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.253760 adafruit-circuitpython-max31856-0.9.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.253760 adafruit-circuitpython-max31856-0.9.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.253760 adafruit-circuitpython-max31856-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2928 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3795 2021-11-15 17:52:14.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      944 2021-11-15 17:52:15.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 17:52:14.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 17:52:14.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-15 17:52:14.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    10070 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/adafruit_max31856.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      267 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5721 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      426 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1158 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      519 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/examples/max31856_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1849 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/examples/max31856_thresholds_and_faults.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 17:52:15.257760 adafruit-circuitpython-max31856-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-11-15 17:51:57.000000 adafruit-circuitpython-max31856-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.878895 adafruit-circuitpython-max31856-0.9.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.882895 adafruit-circuitpython-max31856-0.9.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.882895 adafruit-circuitpython-max31856-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.882895 adafruit-circuitpython-max31856-0.9.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2916 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.882895 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3683 2022-02-04 20:16:24.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      944 2022-02-04 20:16:24.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:16:24.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:16:24.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-02-04 20:16:24.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10070 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/adafruit_max31856.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      426 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1152 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      519 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/examples/max31856_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1849 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/examples/max31856_thresholds_and_faults.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:16:24.886896 adafruit-circuitpython-max31856-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-02-04 20:16:11.000000 adafruit-circuitpython-max31856-0.9.9/setup.py
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-max31856-0.9.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

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

### Comparing `adafruit-circuitpython-max31856-0.9.8/.github/workflows/build.yml` & `adafruit-circuitpython-max31856-0.9.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-max31856-0.9.8/.github/workflows/release.yml` & `adafruit-circuitpython-max31856-0.9.9/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,18 +20,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
-      uses: actions/setup-python@v1
+    - name: Set up Python 3.x
+      uses: actions/setup-python@v2
       with:
-        python-version: 3.6
+        python-version: "3.x"
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
@@ -63,15 +63,15 @@
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

### Comparing `adafruit-circuitpython-max31856-0.9.8/.pre-commit-config.yaml` & `adafruit-circuitpython-max31856-0.9.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/.pylintrc` & `adafruit-circuitpython-max31856-0.9.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-max31856-0.9.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/LICENSE` & `adafruit-circuitpython-max31856-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-max31856-0.9.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/LICENSES/MIT.txt` & `adafruit-circuitpython-max31856-0.9.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-max31856-0.9.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/PKG-INFO` & `adafruit-circuitpython-max31856-0.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max31856
-Version: 0.9.8
+Version: 0.9.9
 Summary: CircuitPython library for the MAX31856 Universal Thermocouple Amplifier.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MAX31856
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit max31856 universal thermocouple amplifierhardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-max31856/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/max31856/en/latest/
+    :target: https://docs.circuitpython.org/projects/max31856/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MAX31856/workflows/Build%20CI/badge.svg
@@ -94,15 +92,15 @@
       # print the temperature!
       print(thermocouple.temperature)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/max31856/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/max31856/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/siddacious/Adafruit_CircuitPython_MAX31856/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/README.rst` & `adafruit-circuitpython-max31856-0.9.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-max31856/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/max31856/en/latest/
+    :target: https://docs.circuitpython.org/projects/max31856/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MAX31856/workflows/Build%20CI/badge.svg
@@ -73,15 +73,15 @@
       # print the temperature!
       print(thermocouple.temperature)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/max31856/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/max31856/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/siddacious/Adafruit_CircuitPython_MAX31856/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/PKG-INFO` & `adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max31856
-Version: 0.9.8
+Version: 0.9.9
 Summary: CircuitPython library for the MAX31856 Universal Thermocouple Amplifier.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MAX31856
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit max31856 universal thermocouple amplifierhardware micropython circuitpython
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-max31856/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/max31856/en/latest/
+    :target: https://docs.circuitpython.org/projects/max31856/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_MAX31856/workflows/Build%20CI/badge.svg
@@ -94,15 +92,15 @@
       # print the temperature!
       print(thermocouple.temperature)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/max31856/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/max31856/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/siddacious/Adafruit_CircuitPython_MAX31856/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/adafruit_circuitpython_max31856.egg-info/SOURCES.txt` & `adafruit-circuitpython-max31856-0.9.9/adafruit_circuitpython_max31856.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/adafruit_max31856.py` & `adafruit-circuitpython-max31856-0.9.9/adafruit_max31856.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/docs/_static/favicon.ico` & `adafruit-circuitpython-max31856-0.9.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/docs/conf.py` & `adafruit-circuitpython-max31856-0.9.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 # autodoc_mock_imports = ["digitalio", "busio", "micropython", "adafruit_bus_device"]
 
 
 intersphinx_mapping = {
-    "python": ("https://docs.python.org/3.4", None),
+    "python": ("https://docs.python.org/3", None),
     "BusDevice": (
-        "https://circuitpython.readthedocs.io/projects/busdevice/en/latest/",
+        "https://docs.circuitpython.org/projects/busdevice/en/latest/",
         None,
     ),
     "Register": (
-        "https://circuitpython.readthedocs.io/projects/register/en/latest/",
+        "https://docs.circuitpython.org/projects/register/en/latest/",
         None,
     ),
-    "CircuitPython": ("https://circuitpython.readthedocs.io/en/latest/", None),
+    "CircuitPython": ("https://docs.circuitpython.org/en/latest/", None),
 }
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 source_suffix = ".rst"
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/docs/index.rst` & `adafruit-circuitpython-max31856-0.9.9/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     Adafruit Universal Thermocouple Amplifier MAX31856 Breakout <https://www.adafruit.com/product/3263>
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/siddacious/Adafruit_CircuitPython_MAX31856/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-max31856-0.9.8/examples/max31856_simpletest.py` & `adafruit-circuitpython-max31856-0.9.9/examples/max31856_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/examples/max31856_thresholds_and_faults.py` & `adafruit-circuitpython-max31856-0.9.9/examples/max31856_thresholds_and_faults.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31856-0.9.8/setup.py` & `adafruit-circuitpython-max31856-0.9.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,16 +41,14 @@
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
     keywords="adafruit max31856 universal thermocouple amplifier"
     "hardware micropython circuitpython",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     py_modules=["adafruit_max31856"],
```

