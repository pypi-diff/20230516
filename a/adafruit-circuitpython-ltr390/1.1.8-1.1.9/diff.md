# Comparing `tmp/adafruit-circuitpython-ltr390-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-ltr390-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ltr390-1.1.8.tar", last modified: Tue Aug  9 19:46:55 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ltr390-1.1.9.tar", last modified: Mon Aug 22 18:42:29 2022, max compression
```

## Comparing `adafruit-circuitpython-ltr390-1.1.8.tar` & `adafruit-circuitpython-ltr390-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.670071 adafruit-circuitpython-ltr390-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.670071 adafruit-circuitpython-ltr390-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.670071 adafruit-circuitpython-ltr390-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-08-09 19:46:55.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      990 2022-08-09 19:46:55.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-09 19:46:55.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-09 19:46:55.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-09 19:46:55.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    16203 2022-08-09 19:46:48.000000 adafruit-circuitpython-ltr390-1.1.8/adafruit_ltr390.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      566 2022-08-09 19:46:48.000000 adafruit-circuitpython-ltr390-1.1.8/examples/ltr390_alert_test.py
--rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-09 19:46:48.000000 adafruit-circuitpython-ltr390-1.1.8/examples/ltr390_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-09 19:46:48.000000 adafruit-circuitpython-ltr390-1.1.8/examples/ltr390_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-09 19:46:48.000000 adafruit-circuitpython-ltr390-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-09 19:46:40.000000 adafruit-circuitpython-ltr390-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-09 19:46:55.674071 adafruit-circuitpython-ltr390-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3565 2022-08-22 18:42:29.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      990 2022-08-22 18:42:29.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:42:29.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-22 18:42:29.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:42:29.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    16203 2022-08-22 18:42:21.000000 adafruit-circuitpython-ltr390-1.1.9/adafruit_ltr390.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5758 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      566 2022-08-22 18:42:21.000000 adafruit-circuitpython-ltr390-1.1.9/examples/ltr390_alert_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      821 2022-08-22 18:42:21.000000 adafruit-circuitpython-ltr390-1.1.9/examples/ltr390_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-22 18:42:21.000000 adafruit-circuitpython-ltr390-1.1.9/examples/ltr390_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1192 2022-08-22 18:42:21.000000 adafruit-circuitpython-ltr390-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-22 18:42:12.000000 adafruit-circuitpython-ltr390-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:42:29.600500 adafruit-circuitpython-ltr390-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ltr390-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-ltr390-1.1.9/.github/workflows/build.yml`

 * *Files 0% similar despite different names*

```diff
@@ -67,11 +67,11 @@
       run: |
         echo ::set-output name=pyproject-toml::$( find . -wholename './pyproject.toml' )
     - name: Build Python package
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       run: |
         pip install --upgrade build twine
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/1.2.3/" $file;
+            sed -i -e "s/0.0.0+auto.0/1.2.3/" $file;
         done;
         python -m build
         twine check dist/*
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-ltr390-1.1.9/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -78,11 +78,11 @@
     - name: Build and publish
       if: contains(steps.need-pypi.outputs.pyproject-toml, 'pyproject.toml')
       env:
         TWINE_USERNAME: ${{ secrets.pypi_username }}
         TWINE_PASSWORD: ${{ secrets.pypi_password }}
       run: |
         for file in $(find -not -path "./.*" -not -path "./docs*" \( -name "*.py" -o -name "*.toml" \) ); do
-            sed -i -e "s/0.0.0-auto.0/${{github.event.release.tag_name}}/" $file;
+            sed -i -e "s/0.0.0+auto.0/${{github.event.release.tag_name}}/" $file;
         done;
         python -m build
         twine upload dist/*
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.gitignore` & `adafruit-circuitpython-ltr390-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ltr390-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/.pylintrc` & `adafruit-circuitpython-ltr390-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ltr390-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/LICENSE` & `adafruit-circuitpython-ltr390-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ltr390-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ltr390-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ltr390-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/PKG-INFO` & `adafruit-circuitpython-ltr390-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ltr390
-Version: 1.1.8
+Version: 1.1.9
 Summary: Adafruit CircuitPython library for the LTR390
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LTR390
 Keywords: adafruit,blinka,circuitpython,micropython,ltr390,UV,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/README.rst` & `adafruit-circuitpython-ltr390-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/PKG-INFO` & `adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ltr390
-Version: 1.1.8
+Version: 1.1.9
 Summary: Adafruit CircuitPython library for the LTR390
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LTR390
 Keywords: adafruit,blinka,circuitpython,micropython,ltr390,UV,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/adafruit_circuitpython_ltr390.egg-info/SOURCES.txt` & `adafruit-circuitpython-ltr390-1.1.9/adafruit_circuitpython_ltr390.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/adafruit_ltr390.py` & `adafruit-circuitpython-ltr390-1.1.9/adafruit_ltr390.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 from struct import unpack_from, pack_into
 from micropython import const
 from adafruit_bus_device import i2c_device
 from adafruit_register.i2c_struct import ROUnaryStruct, Struct
 from adafruit_register.i2c_bits import RWBits
 from adafruit_register.i2c_bit import RWBit, ROBit
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LTR390.git"
 
 _DEFAULT_I2C_ADDR = const(0x53)
 _CTRL = const(0x00)  # Main control register
 _MEAS_RATE = const(0x04)  # Resolution and data rate
 _GAIN = const(0x05)  # ALS and UVS gain range
 _PART_ID = const(0x06)  # Part id/revision register
```

### Comparing `adafruit-circuitpython-ltr390-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ltr390-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/docs/conf.py` & `adafruit-circuitpython-ltr390-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/docs/examples.rst` & `adafruit-circuitpython-ltr390-1.1.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/docs/index.rst` & `adafruit-circuitpython-ltr390-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/examples/ltr390_alert_test.py` & `adafruit-circuitpython-ltr390-1.1.9/examples/ltr390_alert_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/examples/ltr390_configuration_example.py` & `adafruit-circuitpython-ltr390-1.1.9/examples/ltr390_configuration_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr390-1.1.8/pyproject.toml` & `adafruit-circuitpython-ltr390-1.1.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ltr390"
 description = "Adafruit CircuitPython library for the LTR390"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LTR390"}
 keywords = [
     "adafruit",
```

