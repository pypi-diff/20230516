# Comparing `tmp/datadiligence-0.1.4.tar.gz` & `tmp/datadiligence-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadiligence-0.1.4.tar", last modified: Mon May 15 12:02:10 2023, max compression
+gzip compressed data, was "datadiligence-0.1.5.tar", last modified: Tue May 16 18:49:28 2023, max compression
```

## Comparing `datadiligence-0.1.4.tar` & `datadiligence-0.1.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.970846 datadiligence-0.1.4/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      596 2023-05-05 19:41:32.000000 datadiligence-0.1.4/.coveragerc
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.961078 datadiligence-0.1.4/.github/
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.963729 datadiligence-0.1.4/.github/workflows/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      831 2023-05-05 19:41:32.000000 datadiligence-0.1.4/.github/workflows/python-package.yml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      587 2023-05-05 19:41:32.000000 datadiligence-0.1.4/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2023-05-05 19:41:32.000000 datadiligence-0.1.4/.readthedocs.yml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      149 2023-05-05 19:41:32.000000 datadiligence-0.1.4/AUTHORS.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      328 2023-05-15 11:15:31.000000 datadiligence-0.1.4/CHANGELOG.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12356 2023-05-05 19:41:32.000000 datadiligence-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1080 2023-05-05 19:41:32.000000 datadiligence-0.1.4/LICENSE.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-05-15 12:02:10.970939 datadiligence-0.1.4/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3279 2023-05-05 19:41:32.000000 datadiligence-0.1.4/README.rst
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.965144 datadiligence-0.1.4/docs/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/Makefile
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.965271 datadiligence-0.1.4/docs/_static/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/_static/.gitignore
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6444 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/advanced.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/authors.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/changelog.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9764 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/conf.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       33 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/contributing.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1421 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/index.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/license.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9449 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/quickstart.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/readme.rst
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2023-05-05 19:41:32.000000 datadiligence-0.1.4/docs/requirements.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.965695 datadiligence-0.1.4/examples/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      154 2023-05-05 19:41:32.000000 datadiligence-0.1.4/examples/http_headers.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      936 2023-05-05 19:41:32.000000 datadiligence-0.1.4/examples/pre_and_post_processing.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      481 2023-05-05 19:41:32.000000 datadiligence-0.1.4/examples/spawning_api.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2023-05-05 19:41:32.000000 datadiligence-0.1.4/pyproject.toml
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1622 2023-05-15 12:02:10.971332 datadiligence-0.1.4/setup.cfg
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      708 2023-05-05 19:41:32.000000 datadiligence-0.1.4/setup.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.961433 datadiligence-0.1.4/src/
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.966320 datadiligence-0.1.4/src/datadiligence/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      916 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3316 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/bootstrap.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.967729 datadiligence-0.1.4/src/datadiligence/evaluators/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      200 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/evaluators/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      966 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/evaluators/base.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      642 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/evaluators/http.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      924 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/evaluators/postprocess.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2116 2023-05-15 11:49:05.000000 datadiligence-0.1.4/src/datadiligence/evaluators/preprocess.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2243 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/exceptions.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.968856 datadiligence-0.1.4/src/datadiligence/rules/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      128 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/rules/__init__.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1045 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/rules/base.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      447 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/rules/c2pa.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5283 2023-05-15 10:59:43.000000 datadiligence-0.1.4/src/datadiligence/rules/http.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)    10044 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/rules/spawning.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      576 2023-05-05 19:41:32.000000 datadiligence-0.1.4/src/datadiligence/utils.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.967071 datadiligence-0.1.4/src/datadiligence.egg-info/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/PKG-INFO
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1428 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/SOURCES.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/dependency_links.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/not-zip-safe
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      124 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/requires.txt
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)       14 2023-05-15 12:02:10.000000 datadiligence-0.1.4/src/datadiligence.egg-info/top_level.txt
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.970222 datadiligence-0.1.4/tests/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      281 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/conftest.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.970574 datadiligence-0.1.4/tests/samples/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      841 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/samples/custom.py
-drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-15 12:02:10.970714 datadiligence-0.1.4/tests/server/
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1884 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/server/app.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5227 2023-05-15 11:48:17.000000 datadiligence-0.1.4/tests/test_bootstrapper.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      263 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/test_cp2a.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7753 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/test_evaluators.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7159 2023-05-15 11:44:30.000000 datadiligence-0.1.4/tests/test_spawningapi.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)      468 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tests/test_utils.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7261 2023-05-15 10:57:08.000000 datadiligence-0.1.4/tests/test_xrobotsheader.py
--rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2821 2023-05-05 19:41:32.000000 datadiligence-0.1.4/tox.ini
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.822848 datadiligence-0.1.5/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      596 2023-05-05 19:41:32.000000 datadiligence-0.1.5/.coveragerc
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.813686 datadiligence-0.1.5/.github/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.816362 datadiligence-0.1.5/.github/workflows/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      831 2023-05-05 19:41:32.000000 datadiligence-0.1.5/.github/workflows/python-package.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      587 2023-05-05 19:41:32.000000 datadiligence-0.1.5/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      530 2023-05-05 19:41:32.000000 datadiligence-0.1.5/.readthedocs.yml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      149 2023-05-05 19:41:32.000000 datadiligence-0.1.5/AUTHORS.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      390 2023-05-16 18:47:26.000000 datadiligence-0.1.5/CHANGELOG.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    12356 2023-05-05 19:41:32.000000 datadiligence-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1080 2023-05-05 19:41:32.000000 datadiligence-0.1.5/LICENSE.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-05-16 18:49:28.822995 datadiligence-0.1.5/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3279 2023-05-05 19:41:32.000000 datadiligence-0.1.5/README.rst
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.817913 datadiligence-0.1.5/docs/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1154 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/Makefile
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.818038 datadiligence-0.1.5/docs/_static/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       18 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/_static/.gitignore
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     6444 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/advanced.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       41 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/authors.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       43 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/changelog.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9764 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/conf.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       33 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/contributing.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1421 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/index.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       67 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/license.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     9449 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/quickstart.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       39 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/readme.rst
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      233 2023-05-05 19:41:32.000000 datadiligence-0.1.5/docs/requirements.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.818429 datadiligence-0.1.5/examples/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      154 2023-05-05 19:41:32.000000 datadiligence-0.1.5/examples/http_headers.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      936 2023-05-05 19:41:32.000000 datadiligence-0.1.5/examples/pre_and_post_processing.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      481 2023-05-05 19:41:32.000000 datadiligence-0.1.5/examples/spawning_api.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      346 2023-05-05 19:41:32.000000 datadiligence-0.1.5/pyproject.toml
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1622 2023-05-16 18:49:28.823349 datadiligence-0.1.5/setup.cfg
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      708 2023-05-05 19:41:32.000000 datadiligence-0.1.5/setup.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.814069 datadiligence-0.1.5/src/
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.818899 datadiligence-0.1.5/src/datadiligence/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      916 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     3316 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/bootstrap.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.820205 datadiligence-0.1.5/src/datadiligence/evaluators/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      200 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/evaluators/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      966 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/evaluators/base.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      642 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/evaluators/http.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      924 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/evaluators/postprocess.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2116 2023-05-15 11:49:05.000000 datadiligence-0.1.5/src/datadiligence/evaluators/preprocess.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2243 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/exceptions.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.821197 datadiligence-0.1.5/src/datadiligence/rules/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      128 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/rules/__init__.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1045 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/rules/base.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      447 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/rules/c2pa.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5283 2023-05-15 10:59:43.000000 datadiligence-0.1.5/src/datadiligence/rules/http.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)    10044 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/rules/spawning.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      576 2023-05-05 19:41:32.000000 datadiligence-0.1.5/src/datadiligence/utils.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.819503 datadiligence-0.1.5/src/datadiligence.egg-info/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     4080 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/PKG-INFO
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1428 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/SOURCES.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/dependency_links.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)        1 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/not-zip-safe
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      124 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/requires.txt
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)       14 2023-05-16 18:49:28.000000 datadiligence-0.1.5/src/datadiligence.egg-info/top_level.txt
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.822382 datadiligence-0.1.5/tests/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      281 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/conftest.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.822603 datadiligence-0.1.5/tests/samples/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      841 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/samples/custom.py
+drwxr-xr-x   0 nicholaspadgett   (501) staff       (20)        0 2023-05-16 18:49:28.822721 datadiligence-0.1.5/tests/server/
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     1884 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/server/app.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     5227 2023-05-15 11:48:17.000000 datadiligence-0.1.5/tests/test_bootstrapper.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      263 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/test_cp2a.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7753 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/test_evaluators.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7159 2023-05-15 11:44:30.000000 datadiligence-0.1.5/tests/test_spawningapi.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)      468 2023-05-05 19:41:32.000000 datadiligence-0.1.5/tests/test_utils.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     7261 2023-05-15 10:57:08.000000 datadiligence-0.1.5/tests/test_xrobotsheader.py
+-rw-r--r--   0 nicholaspadgett   (501) staff       (20)     2821 2023-05-16 18:25:14.000000 datadiligence-0.1.5/tox.ini
```

### Comparing `datadiligence-0.1.4/.coveragerc` & `datadiligence-0.1.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/.github/workflows/python-package.yml` & `datadiligence-0.1.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/.gitignore` & `datadiligence-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/.readthedocs.yml` & `datadiligence-0.1.5/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/CONTRIBUTING.rst` & `datadiligence-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/LICENSE.txt` & `datadiligence-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/PKG-INFO` & `datadiligence-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datadiligence
-Version: 0.1.4
+Version: 0.1.5
 Summary: Respect generative AI opt-outs in your ML and training pipeline.
 Home-page: https://github.com/Spawning-Inc/datadiligence/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://datadiligence.readthedocs.io/en/latest/quickstart.html
 Project-URL: Source, https://github.com/Spawning-Inc/datadiligence/
 Project-URL: Changelog, https://datadiligence.readthedocs.io/en/latest/changelog.html
 Project-URL: Tracker, https://github.com/Spawning-Inc/datadiligence/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 
 .. image:: https://readthedocs.org/projects/datadiligence/badge/?version=latest
   :alt: ReadTheDocs
```

### Comparing `datadiligence-0.1.4/README.rst` & `datadiligence-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/docs/Makefile` & `datadiligence-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/docs/advanced.rst` & `datadiligence-0.1.5/docs/advanced.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/docs/conf.py` & `datadiligence-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/docs/index.rst` & `datadiligence-0.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/docs/quickstart.rst` & `datadiligence-0.1.5/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/examples/pre_and_post_processing.py` & `datadiligence-0.1.5/examples/pre_and_post_processing.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/setup.cfg` & `datadiligence-0.1.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [options]
 zip_safe = False
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
-python_requires = >=3.8
+python_requires = >=3.7
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	requests >= 2.19.1
 	aiohttp >= 3.6.0
 
 [options.packages.find]
 where = src
```

### Comparing `datadiligence-0.1.4/setup.py` & `datadiligence-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/__init__.py` & `datadiligence-0.1.5/src/datadiligence/__init__.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/bootstrap.py` & `datadiligence-0.1.5/src/datadiligence/bootstrap.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/evaluators/base.py` & `datadiligence-0.1.5/src/datadiligence/evaluators/base.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/evaluators/http.py` & `datadiligence-0.1.5/src/datadiligence/evaluators/http.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/evaluators/postprocess.py` & `datadiligence-0.1.5/src/datadiligence/evaluators/postprocess.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/evaluators/preprocess.py` & `datadiligence-0.1.5/src/datadiligence/evaluators/preprocess.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/exceptions.py` & `datadiligence-0.1.5/src/datadiligence/exceptions.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/rules/base.py` & `datadiligence-0.1.5/src/datadiligence/rules/base.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/rules/http.py` & `datadiligence-0.1.5/src/datadiligence/rules/http.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/rules/spawning.py` & `datadiligence-0.1.5/src/datadiligence/rules/spawning.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence/utils.py` & `datadiligence-0.1.5/src/datadiligence/utils.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/src/datadiligence.egg-info/PKG-INFO` & `datadiligence-0.1.5/src/datadiligence.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: datadiligence
-Version: 0.1.4
+Version: 0.1.5
 Summary: Respect generative AI opt-outs in your ML and training pipeline.
 Home-page: https://github.com/Spawning-Inc/datadiligence/
 Author: Nick Padgett
 Author-email: nick@spawning.ai
 License: MIT
 Project-URL: Documentation, https://datadiligence.readthedocs.io/en/latest/quickstart.html
 Project-URL: Source, https://github.com/Spawning-Inc/datadiligence/
 Project-URL: Changelog, https://datadiligence.readthedocs.io/en/latest/changelog.html
 Project-URL: Tracker, https://github.com/Spawning-Inc/datadiligence/issues
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst; charset=UTF-8
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 
 .. image:: https://readthedocs.org/projects/datadiligence/badge/?version=latest
   :alt: ReadTheDocs
```

### Comparing `datadiligence-0.1.4/src/datadiligence.egg-info/SOURCES.txt` & `datadiligence-0.1.5/src/datadiligence.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/samples/custom.py` & `datadiligence-0.1.5/tests/samples/custom.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/server/app.py` & `datadiligence-0.1.5/tests/server/app.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/test_bootstrapper.py` & `datadiligence-0.1.5/tests/test_bootstrapper.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/test_evaluators.py` & `datadiligence-0.1.5/tests/test_evaluators.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/test_spawningapi.py` & `datadiligence-0.1.5/tests/test_spawningapi.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tests/test_xrobotsheader.py` & `datadiligence-0.1.5/tests/test_xrobotsheader.py`

 * *Files identical despite different names*

### Comparing `datadiligence-0.1.4/tox.ini` & `datadiligence-0.1.5/tox.ini`

 * *Files identical despite different names*

