# Comparing `tmp/adafruit-circuitpython-icm20x-2.0.8.tar.gz` & `tmp/adafruit-circuitpython-icm20x-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-icm20x-2.0.8.tar", last modified: Mon Jun  7 20:12:59 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-icm20x-2.0.9.tar", last modified: Mon Nov 15 17:39:03 2021, max compression
```

## Comparing `adafruit-circuitpython-icm20x-2.0.8.tar` & `adafruit-circuitpython-icm20x-2.0.9.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.186598 adafruit-circuitpython-icm20x-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.190598 adafruit-circuitpython-icm20x-2.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.190598 adafruit-circuitpython-icm20x-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      197 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.190598 adafruit-circuitpython-icm20x-2.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3192 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.190598 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4903 2021-06-07 20:12:59.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2021-06-07 20:12:59.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-06-07 20:12:59.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-06-07 20:12:59.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-06-07 20:12:59.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    27022 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/adafruit_icm20x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      292 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20649_full_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      419 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20649_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_accel_data_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      720 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_gyro_data_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      701 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_mag_data_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-06-07 20:12:59.194598 adafruit-circuitpython-icm20x-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2149 2021-06-07 20:12:49.000000 adafruit-circuitpython-icm20x-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.654372 adafruit-circuitpython-icm20x-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.654372 adafruit-circuitpython-icm20x-2.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.654372 adafruit-circuitpython-icm20x-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3357 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4247 2021-11-15 17:39:03.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1117 2021-11-15 17:39:03.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 17:39:03.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-11-15 17:39:03.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-11-15 17:39:03.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    27013 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/adafruit_icm20x.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      292 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5687 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1286 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1405 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20649_full_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      419 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20649_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_accel_data_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      720 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_gyro_data_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      701 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_mag_data_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      490 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 17:39:03.658372 adafruit-circuitpython-icm20x-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2149 2021-11-15 17:38:54.000000 adafruit-circuitpython-icm20x-2.0.9/setup.py
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-icm20x-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-icm20x-2.0.9/.github/workflows/build.yml`

 * *Files 15% similar despite different names*

```diff
@@ -38,17 +38,17 @@
       with:
         repository: adafruit/actions-ci-circuitpython-libs
         path: actions-ci
     - name: Install dependencies
       # (e.g. - apt-get: gettext, etc; pip: circuitpython-build-tools, requirements.txt; etc.)
       run: |
         source actions-ci/install.sh
-    - name: Pip install pylint, Sphinx, pre-commit
+    - name: Pip install Sphinx, pre-commit
       run: |
-        pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit
+        pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-icm20x-2.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-icm20x-2.0.9/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -14,21 +14,29 @@
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v2.3.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/pycqa/pylint
-    rev: pylint-2.7.1
+    rev: v2.11.1
     hooks:
     -   id: pylint
         name: pylint (library code)
         types: [python]
-        exclude: "^(docs/|examples/|setup.py$)"
--   repo: local
-    hooks:
-    -   id: pylint_examples
-        name: pylint (examples code)
+        args:
+          - --disable=consider-using-f-string
+        exclude: "^(docs/|examples/|tests/|setup.py$)"
+    -   id: pylint
+        name: pylint (example code)
         description: Run pylint rules on "examples/*.py" files
-        entry: /usr/bin/env bash -c
-        args: ['([[ ! -d "examples" ]] || for example in $(find . -path "./examples/*.py"); do pylint --disable=missing-docstring,invalid-name $example; done)']
-        language: system
+        types: [python]
+        files: "^examples/"
+        args:
+        - --disable=missing-docstring,invalid-name,consider-using-f-string,duplicate-code
+    -   id: pylint
+        name: pylint (test code)
+        description: Run pylint rules on "tests/*.py" files
+        types: [python]
+        files: "^tests/"
+        args:
+        - --disable=missing-docstring,consider-using-f-string,duplicate-code
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/.pylintrc` & `adafruit-circuitpython-icm20x-2.0.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
 # disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation
+disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -248,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=12
+min-similarity-lines=4
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-icm20x-2.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/LICENSE` & `adafruit-circuitpython-icm20x-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-icm20x-2.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-icm20x-2.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-icm20x-2.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/PKG-INFO` & `adafruit-circuitpython-icm20x-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,132 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-icm20x
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-icm20x/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/icm20x/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/actions
-            :alt: Build Status
-        
-        Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        * `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-icm20x/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-icm20x
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-icm20x
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-icm20x
-        
-        Usage Example
-        =============
-        
-        For use with the ICM20649:
-        
-        .. code-block:: python3
-        
-            import time
-            import board
-            import adafruit_icm20x
-        
-            i2c = board.I2C()   # uses board.SCL and board.SDA
-            icm = adafruit_icm20x.ICM20649(i2c)
-        
-            while True:
-                print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
-                print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
-                print("")
-                time.sleep(0.5)
-        
-        For use with the ICM20948:
-        
-        .. code-block:: python3
-        
-            import time
-            import board
-            import adafruit_icm20x
-        
-            i2c = board.I2C()  # uses board.SCL and board.SDA
-            icm = adafruit_icm20x.ICM20948(i2c)
-        
-            while True:
-                print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
-                print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
-                print("Magnetometer X:%.2f, Y: %.2f, Z: %.2f uT" % (icm.magnetic))
-                print("")
-                time.sleep(0.5)
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/blob/main/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit blinka circuitpython micropython icm20649 icm20948 icm20x gyro accelerometer high-G 6-axis wide range
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-icm20x/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/icm20x/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/actions
+    :alt: Build Status
+
+Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+* `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-icm20x/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-icm20x
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-icm20x
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-icm20x
+
+Usage Example
+=============
+
+For use with the ICM20649:
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_icm20x
+
+    i2c = board.I2C()   # uses board.SCL and board.SDA
+    icm = adafruit_icm20x.ICM20649(i2c)
+
+    while True:
+        print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
+        print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
+        print("")
+        time.sleep(0.5)
+
+For use with the ICM20948:
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_icm20x
+
+    i2c = board.I2C()  # uses board.SCL and board.SDA
+    icm = adafruit_icm20x.ICM20948(i2c)
+
+    while True:
+        print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
+        print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
+        print("Magnetometer X:%.2f, Y: %.2f, Z: %.2f uT" % (icm.magnetic))
+        print("")
+        time.sleep(0.5)
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/icm20x/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/README.rst` & `adafruit-circuitpython-icm20x-2.0.9/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,19 @@
     while True:
         print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
         print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
         print("Magnetometer X:%.2f, Y: %.2f, Z: %.2f uT" % (icm.magnetic))
         print("")
         time.sleep(0.5)
 
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/icm20x/en/latest/>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/PKG-INFO` & `adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,124 +1,132 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-icm20x
-Version: 2.0.8
+Version: 2.0.9
 Summary: Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
-Description: Introduction
-        ============
-        
-        .. image:: https://readthedocs.org/projects/adafruit-circuitpython-icm20x/badge/?version=latest
-            :target: https://circuitpython.readthedocs.io/projects/icm20x/en/latest/
-            :alt: Documentation Status
-        
-        .. image:: https://img.shields.io/discord/327254708534116352.svg
-            :target: https://adafru.it/discord
-            :alt: Discord
-        
-        .. image:: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/workflows/Build%20CI/badge.svg
-            :target: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/actions
-            :alt: Build Status
-        
-        Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
-        
-        
-        Dependencies
-        =============
-        This driver depends on:
-        
-        * `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
-        * `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
-        * `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
-        
-        Please ensure all dependencies are available on the CircuitPython filesystem.
-        This is easily achieved by downloading
-        `the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
-        
-        Installing from PyPI
-        =====================
-        
-        On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
-        PyPI <https://pypi.org/project/adafruit-circuitpython-icm20x/>`_. To install for current user:
-        
-        .. code-block:: shell
-        
-            pip3 install adafruit-circuitpython-icm20x
-        
-        To install system-wide (this may be required in some cases):
-        
-        .. code-block:: shell
-        
-            sudo pip3 install adafruit-circuitpython-icm20x
-        
-        To install in a virtual environment in your current project:
-        
-        .. code-block:: shell
-        
-            mkdir project-name && cd project-name
-            python3 -m venv .env
-            source .env/bin/activate
-            pip3 install adafruit-circuitpython-icm20x
-        
-        Usage Example
-        =============
-        
-        For use with the ICM20649:
-        
-        .. code-block:: python3
-        
-            import time
-            import board
-            import adafruit_icm20x
-        
-            i2c = board.I2C()   # uses board.SCL and board.SDA
-            icm = adafruit_icm20x.ICM20649(i2c)
-        
-            while True:
-                print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
-                print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
-                print("")
-                time.sleep(0.5)
-        
-        For use with the ICM20948:
-        
-        .. code-block:: python3
-        
-            import time
-            import board
-            import adafruit_icm20x
-        
-            i2c = board.I2C()  # uses board.SCL and board.SDA
-            icm = adafruit_icm20x.ICM20948(i2c)
-        
-            while True:
-                print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
-                print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
-                print("Magnetometer X:%.2f, Y: %.2f, Z: %.2f uT" % (icm.magnetic))
-                print("")
-                time.sleep(0.5)
-        
-        Contributing
-        ============
-        
-        Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/blob/main/CODE_OF_CONDUCT.md>`_
-        before contributing to help this project stay welcoming.
-        
-        Documentation
-        =============
-        
-        For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-        
 Keywords: adafruit blinka circuitpython micropython icm20649 icm20948 icm20x gyro accelerometer high-G 6-axis wide range
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+Introduction
+============
+
+.. image:: https://readthedocs.org/projects/adafruit-circuitpython-icm20x/badge/?version=latest
+    :target: https://circuitpython.readthedocs.io/projects/icm20x/en/latest/
+    :alt: Documentation Status
+
+.. image:: https://img.shields.io/discord/327254708534116352.svg
+    :target: https://adafru.it/discord
+    :alt: Discord
+
+.. image:: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/workflows/Build%20CI/badge.svg
+    :target: https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/actions
+    :alt: Build Status
+
+Library for the ST ICM-20X Wide-Range 6-DoF Accelerometer and Gyro Family
+
+
+Dependencies
+=============
+This driver depends on:
+
+* `Adafruit CircuitPython <https://github.com/adafruit/circuitpython>`_
+* `Bus Device <https://github.com/adafruit/Adafruit_CircuitPython_BusDevice>`_
+* `Register <https://github.com/adafruit/Adafruit_CircuitPython_Register>`_
+
+Please ensure all dependencies are available on the CircuitPython filesystem.
+This is easily achieved by downloading
+`the Adafruit library and driver bundle <https://circuitpython.org/libraries>`_.
+
+Installing from PyPI
+=====================
+
+On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
+PyPI <https://pypi.org/project/adafruit-circuitpython-icm20x/>`_. To install for current user:
+
+.. code-block:: shell
+
+    pip3 install adafruit-circuitpython-icm20x
+
+To install system-wide (this may be required in some cases):
+
+.. code-block:: shell
+
+    sudo pip3 install adafruit-circuitpython-icm20x
+
+To install in a virtual environment in your current project:
+
+.. code-block:: shell
+
+    mkdir project-name && cd project-name
+    python3 -m venv .env
+    source .env/bin/activate
+    pip3 install adafruit-circuitpython-icm20x
+
+Usage Example
+=============
+
+For use with the ICM20649:
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_icm20x
+
+    i2c = board.I2C()   # uses board.SCL and board.SDA
+    icm = adafruit_icm20x.ICM20649(i2c)
+
+    while True:
+        print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
+        print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
+        print("")
+        time.sleep(0.5)
+
+For use with the ICM20948:
+
+.. code-block:: python3
+
+    import time
+    import board
+    import adafruit_icm20x
+
+    i2c = board.I2C()  # uses board.SCL and board.SDA
+    icm = adafruit_icm20x.ICM20948(i2c)
+
+    while True:
+        print("Acceleration: X:%.2f, Y: %.2f, Z: %.2f m/s^2" % (icm.acceleration))
+        print("Gyro X:%.2f, Y: %.2f, Z: %.2f rads/s" % (icm.gyro))
+        print("Magnetometer X:%.2f, Y: %.2f, Z: %.2f uT" % (icm.magnetic))
+        print("")
+        time.sleep(0.5)
+
+Documentation
+=============
+
+API documentation for this library can be found on `Read the Docs <https://circuitpython.readthedocs.io/projects/icm20x/en/latest/>`_.
+
+Contributing
+============
+
+Contributions are welcome! Please read our `Code of Conduct
+<https://github.com/adafruit/Adafruit_CircuitPython_ICM20X/blob/main/CODE_OF_CONDUCT.md>`_
+before contributing to help this project stay welcoming.
+
+Documentation
+=============
+
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
+
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/adafruit_circuitpython_icm20x.egg-info/SOURCES.txt` & `adafruit-circuitpython-icm20x-2.0.9/adafruit_circuitpython_icm20x.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
-.readthedocs.yml
+.readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_icm20x.py
 requirements.txt
 setup.py
@@ -24,14 +24,15 @@
 docs/api.rst
 docs/api.rst.license
 docs/conf.py
 docs/examples.rst
 docs/examples.rst.license
 docs/index.rst
 docs/index.rst.license
+docs/requirements.txt
 docs/_static/favicon.ico
 docs/_static/favicon.ico.license
 examples/icm20x_icm20649_full_test.py
 examples/icm20x_icm20649_simpletest.py
 examples/icm20x_icm20948_accel_data_rate_test.py
 examples/icm20x_icm20948_gyro_data_rate_test.py
 examples/icm20x_icm20948_mag_data_rate_test.py
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/adafruit_icm20x.py` & `adafruit-circuitpython-icm20x-2.0.9/adafruit_icm20x.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ICM20X.git"
 # Common imports; remove if unused or pylint will complain
 from time import sleep
-import adafruit_bus_device.i2c_device as i2c_device
+from adafruit_bus_device import i2c_device
 
 from adafruit_register.i2c_struct import UnaryStruct, ROUnaryStruct, Struct
 from adafruit_register.i2c_bit import RWBit, ROBit
 from adafruit_register.i2c_bits import RWBits
 
 _ICM20649_DEFAULT_ADDRESS = 0x68  # icm20649 default i2c address
 _ICM20948_DEFAULT_ADDRESS = 0x69  # icm20649 default i2c address
```

### Comparing `adafruit-circuitpython-icm20x-2.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-icm20x-2.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/docs/conf.py` & `adafruit-circuitpython-icm20x-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/docs/examples.rst` & `adafruit-circuitpython-icm20x-2.0.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/docs/index.rst` & `adafruit-circuitpython-icm20x-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20649_full_test.py` & `adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20649_full_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_accel_data_rate_test.py` & `adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_accel_data_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_gyro_data_rate_test.py` & `adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_gyro_data_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/examples/icm20x_icm20948_mag_data_rate_test.py` & `adafruit-circuitpython-icm20x-2.0.9/examples/icm20x_icm20948_mag_data_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-icm20x-2.0.8/setup.py` & `adafruit-circuitpython-icm20x-2.0.9/setup.py`

 * *Files identical despite different names*

