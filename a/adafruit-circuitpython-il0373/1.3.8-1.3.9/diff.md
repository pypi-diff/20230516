# Comparing `tmp/adafruit-circuitpython-il0373-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-il0373-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-il0373-1.3.8.tar", last modified: Fri May 21 16:36:22 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-il0373-1.3.9.tar", last modified: Fri Jul 16 14:00:04 2021, max compression
```

## Comparing `adafruit-circuitpython-il0373-1.3.8.tar` & `adafruit-circuitpython-il0373-1.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.947577 adafruit-circuitpython-il0373-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.939577 adafruit-circuitpython-il0373-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)    17967 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3226 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4936 2021-05-21 16:36:22.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-05-21 16:36:22.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-21 16:36:22.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-21 16:36:22.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-05-21 16:36:22.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5973 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/adafruit_il0373.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5424 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-21 16:36:22.943577 adafruit-circuitpython-il0373-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)   360122 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_1.54_color.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1785 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.13_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1714 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.9_color.py
--rw-r--r--   0 runner    (1001) docker     (121)     1140 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.9_grayscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_flexible_2.13_monochrome.py
--rw-r--r--   0 runner    (1001) docker     (121)     1070 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_flexible_2.9_monochrome.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/examples/il0373_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      119 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-21 16:36:22.947577 adafruit-circuitpython-il0373-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-05-21 16:36:13.000000 adafruit-circuitpython-il0373-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.901183 adafruit-circuitpython-il0373-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.893182 adafruit-circuitpython-il0373-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.897183 adafruit-circuitpython-il0373-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.897183 adafruit-circuitpython-il0373-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2437 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1110 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.897183 adafruit-circuitpython-il0373-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    17967 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-07-16 14:00:04.901183 adafruit-circuitpython-il0373-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3260 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.897183 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4986 2021-07-16 14:00:04.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1161 2021-07-16 14:00:04.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-16 14:00:04.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-07-16 14:00:04.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2021-07-16 14:00:04.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5973 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/adafruit_il0373.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.897183 adafruit-circuitpython-il0373-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.901183 adafruit-circuitpython-il0373-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5424 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-16 14:00:04.901183 adafruit-circuitpython-il0373-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)   360122 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1318 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_1.54_color.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1969 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.13_color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.9_color.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1324 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.9_grayscale.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_flexible_2.13_monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_flexible_2.9_monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/examples/il0373_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      119 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-16 14:00:04.901183 adafruit-circuitpython-il0373-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1991 2021-07-16 13:59:56.000000 adafruit-circuitpython-il0373-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-il0373-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-il0373-1.3.9/.github/workflows/build.yml`

 * *Files 12% similar despite different names*

```diff
@@ -18,18 +18,18 @@
       id: repo-name
       run: |
         echo ::set-output name=repo-name::$(
         echo ${{ github.repository }} |
         awk -F '\/' '{ print tolower($2) }' |
         tr '_' '-'
         )
-    - name: Set up Python 3.6
+    - name: Set up Python 3.7
       uses: actions/setup-python@v1
       with:
-        python-version: 3.6
+        python-version: 3.7
     - name: Versions
       run: |
         python3 --version
     - name: Checkout Current Repo
       uses: actions/checkout@v1
       with:
         submodules: true
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-il0373-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-il0373-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/.pylintrc` & `adafruit-circuitpython-il0373-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-il0373-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/LICENSE` & `adafruit-circuitpython-il0373-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-il0373-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/LICENSES/CC-BY-SA-4.0.txt` & `adafruit-circuitpython-il0373-1.3.9/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-il0373-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-il0373-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/PKG-INFO` & `adafruit-circuitpython-il0373-1.3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il0373
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython `displayio` driver for IL0373-based ePaper displays
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_IL0373
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
@@ -32,17 +32,14 @@
         
         Please ensure all dependencies are available on the CircuitPython filesystem.
         This is easily achieved by downloading
         `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
         
         Installing from PyPI
         =====================
-        .. note:: This library is not available on PyPI yet. Install documentation is included
-           as a standard element. Stay tuned for PyPI availability!
-        
         On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
         PyPI <https://pypi.org/project/adafruit-circuitpython-il0373/>`_. To install for current user:
         
         .. code-block:: shell
         
             pip3 install adafruit-circuitpython-il0373
         
@@ -90,30 +87,35 @@
                                              highlight_color=0xff0000)
         
             g = displayio.Group()
         
             f = open("/display-ruler.bmp", "rb")
         
             pic = displayio.OnDiskBitmap(f)
-            t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+            # CircuitPython 6 & 7 compatible
+            t = displayio.TileGrid(
+                pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+            )
+            # CircuitPython 7 compatible only
+            # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
             g.append(t)
         
             display.show(g)
         
             display.refresh()
         
             print("refreshed")
         
             time.sleep(120)
         
         Contributing
         ============
         
         Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/master/CODE_OF_CONDUCT.md>`_
+        <https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/main/CODE_OF_CONDUCT.md>`_
         before contributing to help this project stay welcoming.
         
         Documentation
         =============
         
         For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/README.rst` & `adafruit-circuitpython-il0373-1.3.9/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -24,17 +24,14 @@
 
 Please ensure all dependencies are available on the CircuitPython filesystem.
 This is easily achieved by downloading
 `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
 
 Installing from PyPI
 =====================
-.. note:: This library is not available on PyPI yet. Install documentation is included
-   as a standard element. Stay tuned for PyPI availability!
-
 On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
 PyPI <https://pypi.org/project/adafruit-circuitpython-il0373/>`_. To install for current user:
 
 .. code-block:: shell
 
     pip3 install adafruit-circuitpython-il0373
 
@@ -82,29 +79,34 @@
                                      highlight_color=0xff0000)
 
     g = displayio.Group()
 
     f = open("/display-ruler.bmp", "rb")
 
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
     print("refreshed")
 
     time.sleep(120)
 
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
-<https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/master/CODE_OF_CONDUCT.md>`_
+<https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
 Documentation
 =============
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/PKG-INFO` & `adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-il0373
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython `displayio` driver for IL0373-based ePaper displays
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_IL0373
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
@@ -32,17 +32,14 @@
         
         Please ensure all dependencies are available on the CircuitPython filesystem.
         This is easily achieved by downloading
         `the Adafruit library and driver bundle <https://github.com/adafruit/Adafruit_CircuitPython_Bundle>`_.
         
         Installing from PyPI
         =====================
-        .. note:: This library is not available on PyPI yet. Install documentation is included
-           as a standard element. Stay tuned for PyPI availability!
-        
         On supported GNU/Linux systems like the Raspberry Pi, you can install the driver locally `from
         PyPI <https://pypi.org/project/adafruit-circuitpython-il0373/>`_. To install for current user:
         
         .. code-block:: shell
         
             pip3 install adafruit-circuitpython-il0373
         
@@ -90,30 +87,35 @@
                                              highlight_color=0xff0000)
         
             g = displayio.Group()
         
             f = open("/display-ruler.bmp", "rb")
         
             pic = displayio.OnDiskBitmap(f)
-            t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+            # CircuitPython 6 & 7 compatible
+            t = displayio.TileGrid(
+                pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+            )
+            # CircuitPython 7 compatible only
+            # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
             g.append(t)
         
             display.show(g)
         
             display.refresh()
         
             print("refreshed")
         
             time.sleep(120)
         
         Contributing
         ============
         
         Contributions are welcome! Please read our `Code of Conduct
-        <https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/master/CODE_OF_CONDUCT.md>`_
+        <https://github.com/adafruit/Adafruit_CircuitPython_IL0373/blob/main/CODE_OF_CONDUCT.md>`_
         before contributing to help this project stay welcoming.
         
         Documentation
         =============
         
         For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/adafruit_circuitpython_il0373.egg-info/SOURCES.txt` & `adafruit-circuitpython-il0373-1.3.9/adafruit_circuitpython_il0373.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/adafruit_il0373.py` & `adafruit-circuitpython-il0373-1.3.9/adafruit_il0373.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-il0373-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/docs/conf.py` & `adafruit-circuitpython-il0373-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/docs/index.rst` & `adafruit-circuitpython-il0373-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/display-ruler.bmp` & `adafruit-circuitpython-il0373-1.3.9/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_1.54_color.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_flexible_2.9_monochrome.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-"""Simple test script for 1.54" 152x152 tri-color display.
+"""Simple test script for 2.9" 296x128 monochrome display.
 
 Supported products:
-  * Adafruit 1.54" Tri-Color Display Breakout
-    * https://www.adafruit.com/product/3625
+  * Adafruit Flexible 2.9" Monochrome
+    * https://www.adafruit.com/product/4262
   """
 
 import time
 import board
 import displayio
 import adafruit_il0373
 
@@ -24,29 +24,27 @@
 
 display_bus = displayio.FourWire(
     spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
 )
 time.sleep(1)
 
 display = adafruit_il0373.IL0373(
-    display_bus,
-    width=152,
-    height=152,
-    busy_pin=epd_busy,
-    highlight_color=0xFF0000,
-    rotation=180,
+    display_bus, width=296, height=128, rotation=90, busy_pin=epd_busy, swap_rams=True
 )
 
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
-    print("refreshed")
-
     time.sleep(120)
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.13_color.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.13_color.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,15 +43,20 @@
 # Create a display group for our screen objects
 g = displayio.Group()
 
 # Display a ruler graphic from the root directory of the CIRCUITPY drive
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
     # Create a Tilegrid with the bitmap and put in the displayio group
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     # Place the display group on the screen
     display.show(g)
 
     # Refresh the display to have it actually show the image
     # NOTE: Do not refresh eInk displays sooner than 180 seconds
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.9_color.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.9_color.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,15 +42,20 @@
 # Create a display group for our screen objects
 g = displayio.Group()
 
 # Display a ruler graphic from the root directory of the CIRCUITPY drive
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
     # Create a Tilegrid with the bitmap and put in the displayio group
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     # Place the display group on the screen
     display.show(g)
 
     # Refresh the display to have it actually show the image
     # NOTE: Do not refresh eInk displays sooner than 180 seconds
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_2.9_grayscale.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_flexible_2.13_monochrome.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,50 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-"""Simple test script for 2.9" 296x128 grayscale display.
+"""Simple test script for 2.13" 212x104 monochrome display.
 
 Supported products:
-  * Adafruit 2.9" Grayscale
-    * https://www.adafruit.com/product/4777
+  * Adafruit Flexible 2.13" Monochrome
+    * https://www.adafruit.com/product/4243
   """
 
 import time
-import busio
 import board
 import displayio
 import adafruit_il0373
 
 displayio.release_displays()
 
 # This pinout works on a Feather M4 and may need to be altered for other boards.
-spi = busio.SPI(board.SCK, board.MOSI)  # Uses SCK and MOSI
+spi = board.SPI()  # Uses SCK and MOSI
 epd_cs = board.D9
 epd_dc = board.D10
+epd_reset = board.D5
+epd_busy = board.D6
 
 display_bus = displayio.FourWire(
-    spi, command=epd_dc, chip_select=epd_cs, baudrate=1000000
+    spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
 )
 time.sleep(1)
 
 display = adafruit_il0373.IL0373(
-    display_bus,
-    width=296,
-    height=128,
-    rotation=270,
-    black_bits_inverted=False,
-    color_bits_inverted=False,
-    grayscale=True,
-    refresh_time=1,
+    display_bus, width=212, height=104, rotation=90, busy_pin=epd_busy, swap_rams=True
 )
 
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
-    print("refreshed")
-
     time.sleep(120)
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_flexible_2.13_monochrome.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_1.54_color.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-"""Simple test script for 2.13" 212x104 monochrome display.
+"""Simple test script for 1.54" 152x152 tri-color display.
 
 Supported products:
-  * Adafruit Flexible 2.13" Monochrome
-    * https://www.adafruit.com/product/4243
+  * Adafruit 1.54" Tri-Color Display Breakout
+    * https://www.adafruit.com/product/3625
   """
 
 import time
 import board
 import displayio
 import adafruit_il0373
 
@@ -24,22 +24,34 @@
 
 display_bus = displayio.FourWire(
     spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
 )
 time.sleep(1)
 
 display = adafruit_il0373.IL0373(
-    display_bus, width=212, height=104, rotation=90, busy_pin=epd_busy, swap_rams=True
+    display_bus,
+    width=152,
+    height=152,
+    busy_pin=epd_busy,
+    highlight_color=0xFF0000,
+    rotation=180,
 )
 
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
+    print("refreshed")
+
     time.sleep(120)
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_flexible_2.9_monochrome.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_2.9_grayscale.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,58 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
-"""Simple test script for 2.9" 296x128 monochrome display.
+"""Simple test script for 2.9" 296x128 grayscale display.
 
 Supported products:
-  * Adafruit Flexible 2.9" Monochrome
-    * https://www.adafruit.com/product/4262
+  * Adafruit 2.9" Grayscale
+    * https://www.adafruit.com/product/4777
   """
 
 import time
+import busio
 import board
 import displayio
 import adafruit_il0373
 
 displayio.release_displays()
 
 # This pinout works on a Feather M4 and may need to be altered for other boards.
-spi = board.SPI()  # Uses SCK and MOSI
+spi = busio.SPI(board.SCK, board.MOSI)  # Uses SCK and MOSI
 epd_cs = board.D9
 epd_dc = board.D10
-epd_reset = board.D5
-epd_busy = board.D6
 
 display_bus = displayio.FourWire(
-    spi, command=epd_dc, chip_select=epd_cs, reset=epd_reset, baudrate=1000000
+    spi, command=epd_dc, chip_select=epd_cs, baudrate=1000000
 )
 time.sleep(1)
 
 display = adafruit_il0373.IL0373(
-    display_bus, width=296, height=128, rotation=90, busy_pin=epd_busy, swap_rams=True
+    display_bus,
+    width=296,
+    height=128,
+    rotation=270,
+    black_bits_inverted=False,
+    color_bits_inverted=False,
+    grayscale=True,
+    refresh_time=1,
 )
 
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
+    print("refreshed")
+
     time.sleep(120)
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/examples/il0373_simpletest.py` & `adafruit-circuitpython-il0373-1.3.9/examples/il0373_simpletest.py`

 * *Files 24% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     display_bus, width=212, height=104, rotation=90, highlight_color=0xFF0000
 )
 
 g = displayio.Group()
 
 with open("/display-ruler.bmp", "rb") as f:
     pic = displayio.OnDiskBitmap(f)
-    t = displayio.TileGrid(pic, pixel_shader=displayio.ColorConverter())
+    # CircuitPython 6 & 7 compatible
+    t = displayio.TileGrid(
+        pic, pixel_shader=getattr(pic, "pixel_shader", displayio.ColorConverter())
+    )
+    # CircuitPython 7 compatible only
+    # t = displayio.TileGrid(pic, pixel_shader=pic.pixel_shader)
     g.append(t)
 
     display.show(g)
 
     display.refresh()
 
     print("refreshed")
```

### Comparing `adafruit-circuitpython-il0373-1.3.8/setup.py` & `adafruit-circuitpython-il0373-1.3.9/setup.py`

 * *Files identical despite different names*

