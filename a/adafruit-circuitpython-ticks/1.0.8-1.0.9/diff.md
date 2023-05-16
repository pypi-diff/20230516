# Comparing `tmp/adafruit-circuitpython-ticks-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-ticks-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ticks-1.0.8.tar", last modified: Tue Oct 18 15:09:08 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ticks-1.0.9.tar", last modified: Wed Jan 11 17:28:44 2023, max compression
```

## Comparing `adafruit-circuitpython-ticks-1.0.8.tar` & `adafruit-circuitpython-ticks-1.0.9.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.561258 adafruit-circuitpython-ticks-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.565258 adafruit-circuitpython-ticks-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.565258 adafruit-circuitpython-ticks-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.565258 adafruit-circuitpython-ticks-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.565258 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4047 2022-10-18 15:09:08.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-10-18 15:09:08.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 15:09:08.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-18 15:09:08.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-10-18 15:09:08.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5750 2022-10-18 15:09:01.000000 adafruit-circuitpython-ticks-1.0.8/adafruit_ticks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5878 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      888 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-10-18 15:09:01.000000 adafruit-circuitpython-ticks-1.0.8/examples/ticks_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1229 2022-10-18 15:09:01.000000 adafruit-circuitpython-ticks-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-10-18 15:08:52.000000 adafruit-circuitpython-ticks-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 15:09:08.569258 adafruit-circuitpython-ticks-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.880612 adafruit-circuitpython-ticks-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.880612 adafruit-circuitpython-ticks-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.880612 adafruit-circuitpython-ticks-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.880612 adafruit-circuitpython-ticks-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.880612 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-01-11 17:28:44.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-01-11 17:28:44.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 17:28:44.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-11 17:28:44.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-11 17:28:44.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-01-11 17:28:36.000000 adafruit-circuitpython-ticks-1.0.9/adafruit_ticks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-01-11 17:28:36.000000 adafruit-circuitpython-ticks-1.0.9/examples/ticks_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-01-11 17:28:36.000000 adafruit-circuitpython-ticks-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-01-11 17:28:28.000000 adafruit-circuitpython-ticks-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 17:28:44.884612 adafruit-circuitpython-ticks-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ticks-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/.gitignore` & `adafruit-circuitpython-ticks-1.0.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ticks-1.0.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/.pylintrc` & `adafruit-circuitpython-ticks-1.0.9/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ticks-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/LICENSE` & `adafruit-circuitpython-ticks-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ticks-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ticks-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ticks-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/PKG-INFO` & `adafruit-circuitpython-ticks-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ticks
-Version: 1.0.8
+Version: 1.0.9
 Summary: Work with intervals and deadlines in milliseconds
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ticks.git
 Keywords: adafruit,blinka,circuitpython,micropython,ticks,time,clock,deadline,interval
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/README.rst` & `adafruit-circuitpython-ticks-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/PKG-INFO` & `adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ticks
-Version: 1.0.8
+Version: 1.0.9
 Summary: Work with intervals and deadlines in milliseconds
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ticks.git
 Keywords: adafruit,blinka,circuitpython,micropython,ticks,time,clock,deadline,interval
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/adafruit_circuitpython_ticks.egg-info/SOURCES.txt` & `adafruit-circuitpython-ticks-1.0.9/adafruit_circuitpython_ticks.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ticks.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ticks.egg-info/PKG-INFO
 adafruit_circuitpython_ticks.egg-info/SOURCES.txt
 adafruit_circuitpython_ticks.egg-info/dependency_links.txt
 adafruit_circuitpython_ticks.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/adafruit_ticks.py` & `adafruit-circuitpython-ticks-1.0.9/adafruit_ticks.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 from micropython import const
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ticks.git"
 
 _TICKS_PERIOD = const(1 << 29)
 _TICKS_MAX = const(_TICKS_PERIOD - 1)
 _TICKS_HALFPERIOD = const(_TICKS_PERIOD // 2)
 
 # Get the correct implementation of ticks_ms.  There are three possibilities:
@@ -130,10 +130,10 @@
     assuming that they are within 2**28 ticks"""
     diff = (ticks1 - ticks2) & _TICKS_MAX
     diff = ((diff + _TICKS_HALFPERIOD) & _TICKS_MAX) - _TICKS_HALFPERIOD
     return diff
 
 
 def ticks_less(ticks1: int, ticks2: int) -> bool:
-    """Return true iff ticks1 is less than ticks2,
+    """Return true if ticks1 is before ticks2 and false otherwise,
     assuming that they are within 2**28 ticks"""
     return ticks_diff(ticks1, ticks2) < 0
```

### Comparing `adafruit-circuitpython-ticks-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ticks-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/docs/conf.py` & `adafruit-circuitpython-ticks-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/docs/index.rst` & `adafruit-circuitpython-ticks-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/examples/ticks_simpletest.py` & `adafruit-circuitpython-ticks-1.0.9/examples/ticks_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ticks-1.0.8/pyproject.toml` & `adafruit-circuitpython-ticks-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ticks"
 description = "Work with intervals and deadlines in milliseconds"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ticks.git"}
 keywords = [
     "adafruit",
```

