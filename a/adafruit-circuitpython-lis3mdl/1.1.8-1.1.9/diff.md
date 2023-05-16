# Comparing `tmp/adafruit-circuitpython-lis3mdl-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-lis3mdl-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lis3mdl-1.1.8.tar", last modified: Wed Feb 10 22:19:51 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-lis3mdl-1.1.9.tar", last modified: Tue Mar  2 23:50:52 2021, max compression
```

## Comparing `adafruit-circuitpython-lis3mdl-1.1.8.tar` & `adafruit-circuitpython-lis3mdl-1.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.036625 adafruit-circuitpython-lis3mdl-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2545 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      205 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      441 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16230 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2663 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-02-10 22:19:50.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      898 2021-02-10 22:19:50.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-10 22:19:50.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-02-10 22:19:50.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-02-10 22:19:50.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    10092 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/adafruit_lis3mdl.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      266 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5688 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      382 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)      997 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      665 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_compass.py
--rw-r--r--   0 runner    (1001) docker     (116)      978 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_data_rate_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      985 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_lsm6ds_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      722 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_range_test.py
--rw-r--r--   0 runner    (1001) docker     (116)      458 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      184 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-02-10 22:19:51.040625 adafruit-circuitpython-lis3mdl-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2101 2021-02-10 22:19:41.000000 adafruit-circuitpython-lis3mdl-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.111970 adafruit-circuitpython-lis3mdl-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      205 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2663 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     4188 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      898 2021-03-02 23:50:52.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       81 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       17 2021-03-02 23:50:51.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)    10092 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/adafruit_lis3mdl.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (116)      266 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)     5688 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      382 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (116)      997 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)      665 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_compass.py
+-rw-r--r--   0 runner    (1001) docker     (116)      978 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_data_rate_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      985 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_lsm6ds_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      722 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_range_test.py
+-rw-r--r--   0 runner    (1001) docker     (116)      458 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)      184 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:50:52.115970 adafruit-circuitpython-lis3mdl-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     2101 2021-03-02 23:50:42.000000 adafruit-circuitpython-lis3mdl-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/build.yml`

 * *Files 8% similar despite different names*

```diff
@@ -46,18 +46,14 @@
       run: |
         pip install --force-reinstall pylint Sphinx sphinx-rtd-theme pre-commit
     - name: Library version
       run: git describe --dirty --always --tags
     - name: Pre-commit hooks
       run: |
         pre-commit run --all-files
-    - name: PyLint
-      run: |
-        pylint $( find . -path './adafruit*.py' )
-        ([[ ! -d "examples" ]] || pylint --disable=missing-docstring,invalid-name,bad-whitespace $( find . -path "./examples/*.py" ))
     - name: Build assets
       run: circuitpython-build-bundles --filename_prefix ${{ steps.repo-name.outputs.repo-name }} --library_location .
     - name: Archive bundles
       uses: actions/upload-artifact@v2
       with:
         name: bundles
         path: ${{ github.workspace }}/bundles/
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-lis3mdl-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/.pylintrc` & `adafruit-circuitpython-lis3mdl-1.1.9/.pylintrc`

 * *Files 0% similar despite different names*

```diff
@@ -246,15 +246,15 @@
 # Ignore comments when computing similarities.
 ignore-comments=yes
 
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
-ignore-imports=no
+ignore-imports=yes
 
 # Minimum lines number of a similarity.
 min-similarity-lines=4
 
 
 [BASIC]
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lis3mdl-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/LICENSE` & `adafruit-circuitpython-lis3mdl-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lis3mdl-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/PKG-INFO` & `adafruit-circuitpython-lis3mdl-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis3mdl
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython helper library for the LIS3MDL 3-axis magnetometer
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/README.rst` & `adafruit-circuitpython-lis3mdl-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO` & `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis3mdl
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython helper library for the LIS3MDL 3-axis magnetometer
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS3MDL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt` & `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_circuitpython_lis3mdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/adafruit_lis3mdl.py` & `adafruit-circuitpython-lis3mdl-1.1.9/adafruit_lis3mdl.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-lis3mdl-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/docs/conf.py` & `adafruit-circuitpython-lis3mdl-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/docs/index.rst` & `adafruit-circuitpython-lis3mdl-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_compass.py` & `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_compass.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_data_rate_test.py` & `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_data_rate_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_lsm6ds_test.py` & `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_lsm6ds_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/examples/lis3mdl_range_test.py` & `adafruit-circuitpython-lis3mdl-1.1.9/examples/lis3mdl_range_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis3mdl-1.1.8/setup.py` & `adafruit-circuitpython-lis3mdl-1.1.9/setup.py`

 * *Files identical despite different names*

