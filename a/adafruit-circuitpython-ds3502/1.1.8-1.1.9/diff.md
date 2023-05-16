# Comparing `tmp/adafruit-circuitpython-ds3502-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-ds3502-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ds3502-1.1.8.tar", last modified: Mon Nov 15 19:42:42 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-ds3502-1.1.9.tar", last modified: Fri Feb  4 20:10:06 2022, max compression
```

## Comparing `adafruit-circuitpython-ds3502-1.1.8.tar` & `adafruit-circuitpython-ds3502-1.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.091364 adafruit-circuitpython-ds3502-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      198 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2021-11-15 19:42:42.091364 adafruit-circuitpython-ds3502-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4482 2021-11-15 19:42:41.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      955 2021-11-15 19:42:41.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 19:42:41.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-15 19:42:41.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-15 19:42:41.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2500 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/adafruit_ds3502.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.087364 adafruit-circuitpython-ds3502-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.091364 adafruit-circuitpython-ds3502-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5700 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:42:42.091364 adafruit-circuitpython-ds3502-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      602 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_blinka_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_set_default.py
--rw-r--r--   0 runner    (1001) docker     (121)     1130 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 19:42:42.091364 adafruit-circuitpython-ds3502-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2097 2021-11-15 19:42:31.000000 adafruit-circuitpython-ds3502-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.675856 adafruit-circuitpython-ds3502-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      198 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3625 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4370 2022-02-04 20:10:06.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      955 2022-02-04 20:10:06.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:10:06.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 20:10:06.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:10:06.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2500 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/adafruit_ds3502.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5680 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_blinka_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      715 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_set_default.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1130 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:10:06.679856 adafruit-circuitpython-ds3502-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1999 2022-02-04 20:09:56.000000 adafruit-circuitpython-ds3502-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-ds3502-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ds3502-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

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

### Comparing `adafruit-circuitpython-ds3502-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ds3502-1.1.9/.github/workflows/build.yml`

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

### Comparing `adafruit-circuitpython-ds3502-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-ds3502-1.1.9/.github/workflows/release.yml`

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

### Comparing `adafruit-circuitpython-ds3502-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ds3502-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/.pylintrc` & `adafruit-circuitpython-ds3502-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ds3502-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/LICENSE` & `adafruit-circuitpython-ds3502-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ds3502-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ds3502-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ds3502-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/PKG-INFO` & `adafruit-circuitpython-ds3502-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ds3502
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the Maxim DS3502 I2C Potentionmeter
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DS3502
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ds3502 potentiometer pot resistance
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds3502/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ds3502/en/latest/
+    :target: https://docs.circuitpython.org/projects/ds3502/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS3502/workflows/Build%20CI/badge.svg
@@ -121,15 +119,15 @@
         print("")
         sleep(1.0)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ds3502/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds3502/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS3502/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ds3502-1.1.8/README.rst` & `adafruit-circuitpython-ds3502-1.1.9/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds3502/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ds3502/en/latest/
+    :target: https://docs.circuitpython.org/projects/ds3502/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS3502/workflows/Build%20CI/badge.svg
@@ -100,15 +100,15 @@
         print("")
         sleep(1.0)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ds3502/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds3502/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS3502/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/PKG-INFO` & `adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ds3502
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the Maxim DS3502 I2C Potentionmeter
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_DS3502
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython ds3502 potentiometer pot resistance
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
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ds3502/badge/?version=latest
-    :target: https://circuitpython.readthedocs.io/projects/ds3502/en/latest/
+    :target: https://docs.circuitpython.org/projects/ds3502/en/latest/
     :alt: Documentation Status
 
 .. image:: https://img.shields.io/discord/327254708534116352.svg
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_DS3502/workflows/Build%20CI/badge.svg
@@ -121,15 +119,15 @@
         print("")
         sleep(1.0)
 
 
 Documentation
 =============
 
-API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/ds3502/en/latest/>`_.
+API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ds3502/en/latest/>`_.
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_DS3502/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-ds3502-1.1.8/adafruit_circuitpython_ds3502.egg-info/SOURCES.txt` & `adafruit-circuitpython-ds3502-1.1.9/adafruit_circuitpython_ds3502.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/adafruit_ds3502.py` & `adafruit-circuitpython-ds3502-1.1.9/adafruit_ds3502.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ds3502-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/docs/conf.py` & `adafruit-circuitpython-ds3502-1.1.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,24 +25,24 @@
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = ["micropython", "adafruit_register", "adafruit_bus_device"]
 
 
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

### Comparing `adafruit-circuitpython-ds3502-1.1.8/docs/index.rst` & `adafruit-circuitpython-ds3502-1.1.9/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
     * `Adafruit DS3502 <https://www.adafruit.com/product/4286>`_
 
 .. toctree::
     :caption: Other Links
 
     Download <https://github.com/adafruit/Adafruit_CircuitPython_DS3502/releases/latest>
-    CircuitPython Reference Documentation <https://circuitpython.readthedocs.io>
+    CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
 
 Indices and tables
```

### Comparing `adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_blinka_simpletest.py` & `adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_blinka_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_set_default.py` & `adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_set_default.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/examples/ds3502_simpletest.py` & `adafruit-circuitpython-ds3502-1.1.9/examples/ds3502_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ds3502-1.1.8/setup.py` & `adafruit-circuitpython-ds3502-1.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,16 +44,14 @@
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
     keywords="adafruit blinka circuitpython micropython ds3502 potentiometer pot resistance",
     # You can just specify the packages manually here if your project is
     # simple. Or you can use find_packages().
     # TODO: IF LIBRARY FILES ARE A PACKAGE FOLDER,
     #       CHANGE `py_modules=['...']` TO `packages=['...']`
```

