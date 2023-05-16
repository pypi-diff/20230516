# Comparing `tmp/adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8.tar", last modified: Thu Jun  9 18:36:15 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9.tar", last modified: Tue Aug  9 19:57:30 2022, max compression
```

## Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8.tar` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.733140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.737140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.741140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.741140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_ble_cycling_speed_and_cadence.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.741140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3413 2022-06-09 18:36:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1048 2022-06-09 18:36:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:36:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-06-09 18:36:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-06-09 18:36:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/examples/ble_cycling_speed_and_cadence_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:36:15.745140 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2005 2022-06-09 18:36:04.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.104018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1114 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-08-09 19:57:30.104018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2756 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     6746 2022-08-09 19:57:22.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_ble_cycling_speed_and_cadence.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3585 2022-08-09 19:57:30.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-08-09 19:57:30.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:57:30.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       55 2022-08-09 19:57:30.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-09 19:57:30.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.100018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.104018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)       68 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5649 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1120 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:57:30.104018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2477 2022-08-09 19:57:22.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/examples/ble_cycling_speed_and_cadence_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1333 2022-08-09 19:57:22.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-09 19:57:15.000000 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:57:30.104018 adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.github/workflows/build.yml`

 * *Files 16% similar despite different names*

```diff
@@ -43,33 +43,35 @@
       run: |
         source actions-ci/install.sh
     - name: Pip install Sphinx, pre-commit
       run: |
         pip install --force-reinstall Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
+    - name: Setup problem matchers
+      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
     - name: Build docs
       working-directory: docs
       run: sphinx-build -E -W -b html . _build/html
-    - name: Check For setup.py
+    - name: Check For pyproject.toml
       id: need-pypi
       run: |
-        echo ::set-output name=setup-py::$( find . -wholename './setup.py' )
+        echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
-      if: contains(steps.need-pypi.outputs.setup-py, 'setup.py')
+      if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
-        pip install --upgrade setuptools wheel twine readme_renderer testresources
-        python setup.py sdist
-        python setup.py bdist_wheel --universal
+        pip install --upgrade build twine
+        for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
+            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+        done;
+        python -m build
         twine check dist/*
-    - name: Setup problem matchers
-      uses: adafruit/circuitpython-action-library-ci-problem-matchers@v1
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.gitignore` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/.pylintrc` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSE` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/PKG-INFO` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-cycling-speed-and-cadence
-Version: 1.1.8
+Version: 1.1.9
 Summary: BLE Cycling Speed and Cadence Service
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ble_cycling_speed_and_cadence ble cycling speed cadence bicycle bike
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence
+Keywords: adafruit,blinka,circuitpython,micropython,ble_cycling_speed_and_cadence,ble,cycling,speed,cadence,bicycle,bike
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_cycling_speed_and_cadence/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_cycling_speed_and_cadence/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 BLE Cycling Speed and Cadence Service
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_cycling_speed_and_cadence/en/latest/>`_.
 
@@ -81,9 +84,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/README.rst` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 BLE Cycling Speed and Cadence Service
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -45,16 +49,16 @@
     sudo pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_cycling_speed_and_cadence/en/latest/>`_.
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_ble_cycling_speed_and_cadence.py` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_ble_cycling_speed_and_cadence.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from adafruit_ble.characteristics.int import Uint8Characteristic
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "0.0.0-auto.0"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence.git"
 
 CSCMeasurementValues = namedtuple(
     "CSCMeasurementValues",
     (
         "cumulative_wheel_revolutions",
         "last_wheel_event_time",
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-cycling-speed-and-cadence
-Version: 1.1.8
+Version: 1.1.9
 Summary: BLE Cycling Speed and Cadence Service
-Home-page: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence
-Author: Adafruit Industries
-Author-email: circuitpython@adafruit.com
+Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
-Keywords: adafruit blinka circuitpython micropython ble_cycling_speed_and_cadence ble cycling speed cadence bicycle bike
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence
+Keywords: adafruit,blinka,circuitpython,micropython,ble_cycling_speed_and_cadence,ble,cycling,speed,cadence,bicycle,bike
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Embedded Systems
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
+Provides-Extra: optional
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-ble_cycling_speed_and_cadence/badge/?version=latest
     :target: https://docs.circuitpython.org/projects/ble_cycling_speed_and_cadence/en/latest/
@@ -28,14 +27,18 @@
     :target: https://adafru.it/discord
     :alt: Discord
 
 .. image:: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/workflows/Build%20CI/badge.svg
     :target: https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/actions
     :alt: Build Status
 
+.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
+    :target: https://github.com/psf/black
+    :alt: Code Style: Black
+
 BLE Cycling Speed and Cadence Service
 
 
 Dependencies
 =============
 This driver depends on:
 
@@ -64,16 +67,16 @@
     sudo pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 To install in a virtual environment in your current project:
 
 .. code-block:: shell
 
     mkdir project-name && cd project-name
-    python3 -m venv .env
-    source .env/bin/activate
+    python3 -m venv .venv
+    source .venv/bin/activate
     pip3 install adafruit-circuitpython-ble-cycling-speed-and-cadence
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/ble_cycling_speed_and_cadence/en/latest/>`_.
 
@@ -81,9 +84,7 @@
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_BLE_Cycling_Speed_and_Cadence/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/adafruit_circuitpython_ble_cycling_speed_and_cadence.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 .pylintrc
 .readthedocs.yaml
 CODE_OF_CONDUCT.md
 LICENSE
 README.rst
 README.rst.license
 adafruit_ble_cycling_speed_and_cadence.py
+optional_requirements.txt
+pyproject.toml
 requirements.txt
-setup.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
 .github/workflows/release.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
```

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/conf.py` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/docs/index.rst` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.8/examples/ble_cycling_speed_and_cadence_simpletest.py` & `adafruit-circuitpython-ble-cycling-speed-and-cadence-1.1.9/examples/ble_cycling_speed_and_cadence_simpletest.py`

 * *Files identical despite different names*

