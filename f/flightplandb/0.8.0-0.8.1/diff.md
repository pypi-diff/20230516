# Comparing `tmp/flightplandb-0.8.0.tar.gz` & `tmp/flightplandb-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flightplandb-0.8.0.tar", last modified: Mon May  8 18:44:14 2023, max compression
+gzip compressed data, was "flightplandb-0.8.1.tar", last modified: Tue May 16 21:47:17 2023, max compression
```

## Comparing `flightplandb-0.8.0.tar` & `flightplandb-0.8.1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-08 18:43:57.000000 flightplandb-0.8.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-05-08 18:43:57.000000 flightplandb-0.8.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-08 18:43:57.000000 flightplandb-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-08 18:43:57.000000 flightplandb-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-08 18:44:14.637191 flightplandb-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-08 18:43:57.000000 flightplandb-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/artwork/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/artwork/ico/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/ico/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/artwork/png/
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/240x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/png/480x480.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/artwork/svg/
--rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-08 18:43:57.000000 flightplandb-0.8.0/artwork/svg/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/docs/source/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   118473 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/_static/css/colourscheme.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/datatypes.rst
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/internal.rst
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/main.rst
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/nav.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/plan.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/tags.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/user.rst
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/api/weather.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/docs/source/user/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-08 18:43:57.000000 flightplandb-0.8.0/docs/source/user/userdocs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-08 18:43:57.000000 flightplandb-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 18:44:14.637191 flightplandb-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.629191 flightplandb-0.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.633191 flightplandb-0.8.0/src/flightplandb/
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26569 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20538 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/internal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-08 18:43:57.000000 flightplandb-0.8.0/src/flightplandb/weather.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/src/flightplandb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-08 18:44:14.000000 flightplandb-0.8.0/src/flightplandb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 18:44:14.637191 flightplandb-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_nav.py
--rw-r--r--   0 runner    (1001) docker     (123)    26129 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-08 18:43:57.000000 flightplandb-0.8.0/tests/test_weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.273520 flightplandb-0.8.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.265520 flightplandb-0.8.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 21:47:00.000000 flightplandb-0.8.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-16 21:47:00.000000 flightplandb-0.8.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-16 21:47:00.000000 flightplandb-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 21:47:00.000000 flightplandb-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-16 21:47:17.273520 flightplandb-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-16 21:47:00.000000 flightplandb-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.265520 flightplandb-0.8.1/artwork/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/artwork/ico/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/ico/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/artwork/png/
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/png/120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11599 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/png/240x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/png/32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)    25027 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/png/480x480.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/artwork/svg/
+-rw-r--r--   0 runner    (1001) docker     (123)    11020 2023-05-16 21:47:00.000000 flightplandb-0.8.1/artwork/svg/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.265520 flightplandb-0.8.1/docs/source/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/docs/source/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   118473 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/_static/css/colourscheme.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/datatypes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/internal.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/main.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/nav.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/plan.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/tags.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/user.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/api/weather.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.269520 flightplandb-0.8.1/docs/source/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/user/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/user/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/user/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 21:47:00.000000 flightplandb-0.8.1/docs/source/user/userdocs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-05-16 21:47:00.000000 flightplandb-0.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:47:17.273520 flightplandb-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.265520 flightplandb-0.8.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.273520 flightplandb-0.8.1/src/flightplandb/
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26950 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20874 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/internal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12269 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-16 21:47:00.000000 flightplandb-0.8.1/src/flightplandb/weather.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.273520 flightplandb-0.8.1/src/flightplandb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2784 2023-05-16 21:47:17.000000 flightplandb-0.8.1/src/flightplandb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-16 21:47:17.000000 flightplandb-0.8.1/src/flightplandb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:47:17.000000 flightplandb-0.8.1/src/flightplandb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 21:47:17.000000 flightplandb-0.8.1/src/flightplandb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 21:47:17.000000 flightplandb-0.8.1/src/flightplandb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:47:17.273520 flightplandb-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_nav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26130 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12752 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-16 21:47:00.000000 flightplandb-0.8.1/tests/test_weather.py
```

### Comparing `flightplandb-0.8.0/.github/workflows/lint.yml` & `flightplandb-0.8.1/.github/workflows/lint.yml`

 * *Files 18% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 jobs:
   # no need to set up a matrix for the lint
   lint:
     runs-on: ubuntu-latest
     name: Lint
     steps:
       - name: Check out source repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up Python environment
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v3
         with:
           python-version: "3.11"
       - name: black
         uses: psf/black@stable
         with:
           options: "--check --verbose"
           src: "./src ./tests ./docs/source/conf.py"
       - name: flake8
-        uses: py-actions/flake8@v1
+        uses: py-actions/flake8@v2
         with:
           max-line-length: "88"  # match limit set by black
           args: "--extend-ignore E203"
       - name: isort
         uses: isort/isort-action@v1
```

### Comparing `flightplandb-0.8.0/.github/workflows/release.yml` & `flightplandb-0.8.1/.github/workflows/release.yml`

 * *Files 19% similar despite different names*

```diff
@@ -6,22 +6,21 @@
   workflow_dispatch:
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
-    - uses: actions/setup-python@v2
+    - uses: actions/checkout@v3
+    - uses: actions/setup-python@v3
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install build wheel twine
+        python -m pip install build twine
     - name: Build
       run: |
         python -m build
     - name: Publish
-      env:
-        TWINE_USERNAME: __token__
-        TWINE_PASSWORD: ${{ secrets.PYPI_PASSWORD }}
-      run: |
-        twine upload dist/* --skip-existing
+      uses: pypa/gh-action-pypi-publish@release/v1
+      with:
+        password: ${{ secrets.PYPI_API_TOKEN }}
+
```

### Comparing `flightplandb-0.8.0/.github/workflows/test.yml` & `flightplandb-0.8.1/.github/workflows/test.yml`

 * *Files 23% similar despite different names*

```diff
@@ -7,16 +7,16 @@
         python-version: [ '3.8', '3.9', '3.10', '3.11']
     runs-on: ubuntu-latest
 
     name: Unit tests, Python ${{ matrix.python-version }}
 
     steps:
       - name: Check out source repository
-        uses: actions/checkout@v2
+        uses: actions/checkout@v3
       - name: Set up Python environment
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v3
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install packages
         run: python -m pip install .[test]
       - name: Run unittests
         run: python -m pytest tests
```

### Comparing `flightplandb-0.8.0/.readthedocs.yaml` & `flightplandb-0.8.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/CHANGELOG.rst` & `flightplandb-0.8.1/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 Changelog
 --------------------
 
+0.8.1
+^^^^^^^^^^^^^^^^^^^^
+This makes the library compatible with mypy strict checking, and slightly cleans up the release workflow.
+
 0.8.0
 ^^^^^^^^^^^^^^^^^^^^
 This makes the entire library compatible with PEP-561, so that it can now be used with a static
 type checker like mypy. The codebase has been reformatted with black and isort, and the tags
 field of a PlanQuery now takes a list of strings, rather than a single string containing
 the tags separated by commas and spaces. ``pdf`` is now the only return format which returns bytes;
 ``native`` returns a dataclass and all other formats return a UTF-8 string.
 
 The changelog has also been updated to include the changes of version 0.5.0 and earlier.
 A pre-commit file has been added to ensure all checks will pass before committing.
 
-
 0.7.2
 ^^^^^^^^^^^^^^^^^^^^
 This fixes a bug in the core API interface where HTTP headers were being passed into
 requests as parameters.
 
 0.7.1
 ^^^^^^^^^^^^^^^^^^^^
```

### Comparing `flightplandb-0.8.0/LICENSE` & `flightplandb-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/PKG-INFO` & `flightplandb-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightplandb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python wrapper for the Flight Plan Database API
 Author-email: PH-KDX <smtp.python.email.sender@gmail.com>
 License: GPL v3
 Project-URL: Homepage, https://github.com/PH-KDX/flightplandb-py/
 Project-URL: Documentation, https://flightplandb-py.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/PH-KDX/flightplandb-py/issues
 Project-URL: Changelog, https://github.com/PH-KDX/flightplandb-py/blob/main/CHANGELOG.rst
```

### Comparing `flightplandb-0.8.0/README.md` & `flightplandb-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/ico/favicon.ico` & `flightplandb-0.8.1/artwork/ico/favicon.ico`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/png/120x120.png` & `flightplandb-0.8.1/artwork/png/120x120.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/png/240x240.png` & `flightplandb-0.8.1/artwork/png/240x240.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/png/32x32.png` & `flightplandb-0.8.1/artwork/png/32x32.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/png/480x480.png` & `flightplandb-0.8.1/artwork/png/480x480.png`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/artwork/svg/logo.svg` & `flightplandb-0.8.1/artwork/svg/logo.svg`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/Makefile` & `flightplandb-0.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/_static/css/colourscheme.css` & `flightplandb-0.8.1/docs/source/_static/css/colourscheme.css`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/api/plan.rst` & `flightplandb-0.8.1/docs/source/api/plan.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/conf.py` & `flightplandb-0.8.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/index.rst` & `flightplandb-0.8.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/user/introduction.rst` & `flightplandb-0.8.1/docs/source/user/introduction.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/docs/source/user/quickstart.rst` & `flightplandb-0.8.1/docs/source/user/quickstart.rst`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/pyproject.toml` & `flightplandb-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/src/flightplandb/__init__.py` & `flightplandb-0.8.1/src/flightplandb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 For more information on Flight Plan Database, read their excellent About page
 at https://flightplandatabase.com/about. For more information about this
 library, read the documentation at https://flightplandb-py.readthedocs.io/.
 """
 
 
 # Version of the flightplandb package
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 from . import api, datatypes, exceptions, internal, nav, plan, tags, user, weather
 
 __all__ = [
     "internal",
     "exceptions",
     "datatypes",
```

### Comparing `flightplandb-0.8.0/src/flightplandb/api.py` & `flightplandb-0.8.1/src/flightplandb/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """These functions return information about the API."""
-from typing import Optional
+from typing import Dict, Optional
 
 from flightplandb import internal
 from flightplandb.datatypes import StatusResponse
 
 
 async def header_value(header_key: str, key: Optional[str] = None) -> str:
     """Gets header value for key. Do not call directly.
@@ -112,15 +112,21 @@
     Returns
     -------
     StatusResponse
         OK 200 means the service is up and running.
     """
 
     resp = await internal.get(path="", key=key)
-    return StatusResponse(**resp)
+    if isinstance(resp, Dict):
+        return StatusResponse(**resp)
+    else:
+        raise ValueError(
+            "Could not convert response to a StatusResponse datatype; "
+            "it is not a valid mapping"
+        )
 
 
 async def revoke(key: str) -> StatusResponse:
     """Revoke the API key in use in the event it is compromised.
     See :ref:`authentication` for more details.
 
     Requires authentication.
@@ -137,8 +143,14 @@
         then the key has been revoked and any further requests will be
         rejected.
         Any other status code or message indicates an error has
         occurred and the errors array will give further details.
     """
 
     resp = await internal.get(path="/auth/revoke", key=key)
-    return StatusResponse(**resp)
+    if isinstance(resp, Dict):
+        return StatusResponse(**resp)
+    else:
+        raise ValueError(
+            "could not convert response to a StatusResponse datatype; "
+            "it is not a valid mapping"
+        )
```

### Comparing `flightplandb-0.8.0/src/flightplandb/datatypes.py` & `flightplandb-0.8.1/src/flightplandb/datatypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 #
 # You should have received a copy of the GNU General Public License along
 # with FlightplanDB-py.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from dataclasses import dataclass
 from datetime import datetime
-from typing import List, Optional, Union
+from typing import Any, Dict, List, Optional, Union
 
 from dateutil.parser import isoparse
 
 
-def _datetime_to_iso(timestamp: datetime):
+def _datetime_to_iso(timestamp: datetime) -> str:
     return timestamp.strftime("%Y-%m-%dT%H:%M:%S.%f")[:-3] + "Z"
 
 
 @dataclass
 class StatusResponse:
     """
     Returned for some functions to indicate execution status
@@ -40,15 +40,15 @@
     errors : Optional[List[str]]
         A list of any errors raised
     """
 
     message: str
     errors: Optional[List[str]]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class User:
     """Describes users registered on the website
 
@@ -83,21 +83,21 @@
     joined: Optional[datetime] = None
     lastSeen: Optional[datetime] = None
     plansCount: Optional[int] = 0
     plansDistance: Optional[float] = 0.0
     plansDownloads: Optional[int] = 0
     plansLikes: Optional[int] = 0
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.joined and isinstance(self.joined, str):
             self.joined = isoparse(self.joined)
         if self.lastSeen and isinstance(self.lastSeen, str):
             self.lastSeen = isoparse(self.lastSeen)
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
         if isinstance(resp_dict["joined"], datetime):
             resp_dict["joined"] = _datetime_to_iso(resp_dict["joined"])
         if isinstance(resp_dict["lastSeen"], datetime):
             resp_dict["lastSeen"] = _datetime_to_iso(resp_dict["lastSeen"])
         return resp_dict
 
@@ -119,15 +119,15 @@
     """
 
     id: int
     username: str
     location: Optional[str] = None
     gravatarHash: Optional[str] = None
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Application:
     """Describes application associated with a flight plan
 
@@ -141,15 +141,15 @@
         Application URL
     """
 
     id: int
     name: Optional[str] = None
     url: Optional[str] = None
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Via:
     """Describes routes to :class:`RouteNode` s
 
@@ -164,19 +164,19 @@
     """
 
     ident: str
     type: str
 
     validtypes = ["SID", "STAR", "AWY-HI", "AWY-LO", "NAT", "PACOT"]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid Via type")
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class RouteNode:
     """Describes nodes in :class:`Route` s
 
@@ -207,24 +207,24 @@
     ident: str
     type: str
     lat: float
     lon: float
     id: Optional[int] = None
     alt: Optional[float] = None
     name: Optional[str] = None
-    via: Optional[Via] = None
+    via: Optional[Union[Via, Dict[str, Any]]] = None
 
     validtypes = ["UKN", "APT", "NDB", "VOR", "FIX", "DME", "LATLON"]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid RouteNode type")
         self.via = Via(**self.via) if isinstance(self.via, dict) else self.via
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
         if resp_dict["via"] and isinstance(resp_dict["via"], Via):
             resp_dict["via"] = resp_dict["via"].to_api_dict()
         return resp_dict
 
 
 @dataclass
@@ -241,27 +241,23 @@
         Valid westbound flightlevels. Only used inside a NATS :class:`Track`.
     """
 
     nodes: List[RouteNode]
     eastLevels: Optional[List[str]] = None
     westLevels: Optional[List[str]] = None
 
-    def __post_init__(self):
-        self.nodes = list(
-            map(
-                lambda node: (RouteNode(**node) if (isinstance(node, dict)) else node),
-                self.nodes,
-            )
-        )
+    def __post_init__(self) -> None:
+        self.nodes = [
+            (RouteNode(**node) if (isinstance(node, dict)) else node)
+            for node in self.nodes
+        ]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
-        resp_dict["nodes"] = list(
-            map(lambda node: node.to_api_dict(), resp_dict["nodes"])
-        )
+        resp_dict["nodes"] = [node.to_api_dict() for node in resp_dict["nodes"]]
         return resp_dict
 
 
 @dataclass
 class Cycle:
     """Navdata cycle
 
@@ -278,15 +274,15 @@
     """
 
     id: int
     ident: str
     year: int
     release: int
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Plan:
     """A flight plan; the thing this whole API revolves around
 
@@ -347,42 +343,42 @@
     maxAltitude: Optional[float] = None
     waypoints: Optional[int] = None
     likes: Optional[int] = None
     downloads: Optional[int] = None
     popularity: Optional[int] = None
     notes: Optional[str] = None
     encodedPolyline: Optional[str] = None
-    createdAt: Optional[datetime] = None
-    updatedAt: Optional[datetime] = None
+    createdAt: Optional[Union[datetime, str]] = None
+    updatedAt: Optional[Union[datetime, str]] = None
     tags: Optional[List[str]] = None
     user: Optional[User] = None
     application: Optional[Application] = None
     route: Optional[Route] = None
     cycle: Optional[Cycle] = None
 
-    def __post_init__(self):
-        if self.createdAt and type(self.createdAt) != datetime:
+    def __post_init__(self) -> None:
+        if self.createdAt and type(self.createdAt) == str:
             self.createdAt = isoparse(self.createdAt)
 
-        if self.updatedAt and type(self.updatedAt) != datetime:
+        if self.updatedAt and type(self.updatedAt) == str:
             self.updatedAt = isoparse(self.updatedAt)
 
         if self.user and isinstance(self.user, dict):
             self.user = User(**self.user)
 
         if self.application and isinstance(self.application, dict):
             self.application = Application(**self.application)
 
         if self.route and isinstance(self.route, dict):
             self.route = Route(**self.route)
 
         if self.cycle and isinstance(self.cycle, dict):
             self.cycle = Cycle(**self.cycle)
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         plan_dict = self.__dict__
         if isinstance(plan_dict["createdAt"], datetime):
             plan_dict["createdAt"] = _datetime_to_iso(plan_dict["createdAt"])
         if isinstance(plan_dict["updatedAt"], datetime):
             plan_dict["updatedAt"] = _datetime_to_iso(plan_dict["updatedAt"])
         if isinstance(plan_dict["user"], User):
             plan_dict["user"] = plan_dict["user"].to_api_dict()
@@ -430,15 +426,15 @@
     toName: Optional[str] = None
     flightNumber: Optional[str] = None
     distanceMin: Optional[str] = None
     distanceMax: Optional[str] = None
     tags: Optional[List[str]] = None
     includeRoute: Optional[bool] = None
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         plan_query_dict = self.__dict__
         if self.tags:
             plan_query_dict["tags"] = ", ".join(self.tags)
         return plan_query_dict
 
 
 @dataclass
@@ -482,15 +478,15 @@
     cruiseAlt: Optional[float] = 35000
     cruiseSpeed: Optional[float] = 420
     ascentRate: Optional[float] = 2500
     ascentSpeed: Optional[float] = 250
     descentRate: Optional[float] = 1500
     descentSpeed: Optional[float] = 250
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Tag:
     """Flight plan tag
 
@@ -507,15 +503,15 @@
     """
 
     name: str
     description: Optional[str]
     planCount: int
     popularity: int
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Timezone:
     """Contains timezone information
 
@@ -527,15 +523,15 @@
         The number of seconds the airport timezone is currently
         offset from UTC. Positive is ahead of UTC. ``None`` if not available
     """
 
     name: Optional[str]
     offset: Optional[float]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Times:
     """Contains relevant times information
 
@@ -547,38 +543,30 @@
         Time of sunset
     dawn : datetime
         Time of dawn
     dusk : datetime
         Time of dusk
     """
 
-    sunrise: datetime
-    sunset: datetime
-    dawn: datetime
-    dusk: datetime
+    sunrise: Union[datetime, str]
+    sunset: Union[datetime, str]
+    dawn: Union[datetime, str]
+    dusk: Union[datetime, str]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.sunrise = (
-            isoparse(self.sunrise)
-            if not isinstance(self.sunrise, datetime)
-            else self.sunrise
+            isoparse(self.sunrise) if isinstance(self.sunrise, str) else self.sunrise
         )
         self.sunset = (
-            isoparse(self.sunset)
-            if not isinstance(self.sunset, datetime)
-            else self.sunset
-        )
-        self.dawn = (
-            isoparse(self.dawn) if not isinstance(self.dawn, datetime) else self.dawn
-        )
-        self.dusk = (
-            isoparse(self.dusk) if not isinstance(self.dusk, datetime) else self.dusk
+            isoparse(self.sunset) if isinstance(self.sunset, str) else self.sunset
         )
+        self.dawn = isoparse(self.dawn) if isinstance(self.dawn, str) else self.dawn
+        self.dusk = isoparse(self.dusk) if isinstance(self.dusk, str) else self.dusk
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         plan_dict = self.__dict__
         plan_dict["sunrise"] = _datetime_to_iso(plan_dict["sunrise"])
         plan_dict["sunset"] = _datetime_to_iso(plan_dict["sunset"])
         plan_dict["dawn"] = _datetime_to_iso(plan_dict["dawn"])
         plan_dict["dusk"] = _datetime_to_iso(plan_dict["dusk"])
         return plan_dict
 
@@ -597,15 +585,15 @@
         The longitude of the runway end
     """
 
     ident: str
     lat: float
     lon: float
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Navaid:
     """Describes a navigational aid
 
@@ -650,19 +638,19 @@
     bearing: Optional[float]
     name: Optional[str]
     elevation: float
     range: float
 
     validtypes = ["LOC-ILS", "LOC-LOC", "GS", "DME", "OM", "MM", "IM"]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid Navaid type")
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Runway:
     """Describes a runway at an :class:`Airport`
 
@@ -700,26 +688,29 @@
     markings: List[str]
     lighting: List[str]
     thresholdOffset: float
     overrunLength: float
     ends: List[RunwayEnds]
     navaids: List[Navaid]
 
-    def __post_init__(self):
-        if self.ends and (isinstance(self.ends[0], dict)):
-            self.ends = list(map(lambda rw: RunwayEnds(**rw), self.ends))
-        if self.navaids and (isinstance(self.navaids[0], dict)):
-            self.navaids = list(map(lambda n: Navaid(**n), self.navaids))
+    def __post_init__(self) -> None:
+        if self.ends:
+            self.ends = [
+                (RunwayEnds(**rwe) if isinstance(rwe, dict) else rwe)
+                for rwe in self.ends
+            ]
+        if self.navaids:
+            self.navaids = [
+                (Navaid(**na) if isinstance(na, dict) else na) for na in self.navaids
+            ]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
-        resp_dict["ends"] = list(map(lambda end: end.to_api_dict(), resp_dict["ends"]))
-        resp_dict["navaids"] = list(
-            map(lambda aid: aid.to_api_dict(), resp_dict["navaids"])
-        )
+        resp_dict["ends"] = [end.to_api_dict() for end in resp_dict["ends"]]
+        resp_dict["navaids"] = [aid.to_api_dict() for aid in resp_dict["navaids"]]
         return resp_dict
 
 
 @dataclass
 class Frequency:
     """Holds frequency information
 
@@ -734,15 +725,15 @@
 
     """
 
     type: str
     frequency: float
     name: Optional[str]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Weather:
     """Contains weather reports and predictions
 
@@ -753,15 +744,15 @@
     TAF : Optional[str]
         Current TAF report for the airport
     """
 
     METAR: Optional[str]
     TAF: Optional[str]
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
 
 
 @dataclass
 class Airport:
     """Describes an airport.
     An oversized dataclass with more information than you'd need in 500 years.
@@ -812,40 +803,43 @@
     timezone: Timezone
     times: Times
     runwayCount: int
     runways: List[Runway]
     frequencies: List[Frequency]
     weather: Weather
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.timezone and isinstance(self.timezone, dict):
             self.timezone = Timezone(**self.timezone)
 
         if self.times and isinstance(self.times, dict):
             self.times = Times(**self.times)
 
-        if self.runways and isinstance(self.runways[0], dict):
-            self.runways = list(map(lambda rw: Runway(**rw), self.runways))
-
-        if self.frequencies and isinstance(self.frequencies[0], dict):
-            self.frequencies = list(map(lambda rw: Frequency(**rw), self.frequencies))
+        if self.runways:
+            self.runways = [
+                (Runway(**rw) if isinstance(rw, dict) else rw) for rw in self.runways
+            ]
+
+        if self.frequencies:
+            self.frequencies = [
+                (Frequency(**fq) if isinstance(fq, dict) else fq)
+                for fq in self.frequencies
+            ]
 
         if self.weather and isinstance(self.weather, dict):
             self.weather = Weather(**self.weather)
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
         resp_dict["timezone"] = resp_dict["timezone"].to_api_dict()
         resp_dict["times"] = resp_dict["times"].to_api_dict()
-        resp_dict["runways"] = list(
-            map(lambda rwy: rwy.to_api_dict(), resp_dict["runways"])
-        )
-        resp_dict["frequencies"] = list(
-            map(lambda freq: freq.to_api_dict(), resp_dict["frequencies"])
-        )
+        resp_dict["runways"] = [rwy.to_api_dict() for rwy in resp_dict["runways"]]
+        resp_dict["frequencies"] = [
+            freq.to_api_dict() for freq in resp_dict["frequencies"]
+        ]
         resp_dict["weather"] = resp_dict["weather"].to_api_dict()
         return resp_dict
 
 
 @dataclass
 class Track:
     """Used for NATS and PACOTS tracks
@@ -863,23 +857,23 @@
     """
 
     ident: Union[str, int]
     route: Route
     validFrom: datetime
     validTo: datetime
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.route and isinstance(self.route, dict):
             self.route = Route(**self.route)
         if self.validFrom and isinstance(self.validFrom, str):
             self.validFrom = isoparse(self.validFrom)
         if self.validTo and isinstance(self.validTo, str):
             self.validTo = isoparse(self.validTo)
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         resp_dict = self.__dict__
         if isinstance(resp_dict["validFrom"], datetime):
             resp_dict["validFrom"] = _datetime_to_iso(resp_dict["validFrom"])
         if isinstance(resp_dict["validTo"], datetime):
             resp_dict["validTo"] = _datetime_to_iso(resp_dict["validTo"])
         return resp_dict
 
@@ -918,13 +912,13 @@
     elevation: float
     runwayIdent: Optional[str] = None
     airportICAO: Optional[str] = None
     name: Optional[float] = None
 
     validtypes = ["UKN", "APT", "NDB", "VOR", "FIX", "DME", "LATLON"]
 
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         if self.type not in self.validtypes:
             raise ValueError(f"{self.type} is not a valid SearchNavaid type")
 
-    def to_api_dict(self):
+    def to_api_dict(self) -> Dict[str, Any]:
         return self.__dict__
```

### Comparing `flightplandb-0.8.0/src/flightplandb/exceptions.py` & `flightplandb-0.8.1/src/flightplandb/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 "Contains all the internally defined exceptions used by the library."
+from typing import Tuple, Union
 
 
 class BaseErrorHandler(Exception):
     """Base exception. The other exceptions all inherit from
     this one, but this exception will be raised directly if
     no others match the returned HTTP status code.
 
@@ -10,109 +11,111 @@
     ----------
     status_code
         Status code of the error
     message
         Description of the error
     """
 
-    def __init__(self, status_code=None, message=None):
+    def __init__(self, status_code: int, message: str):
         self.status_code = status_code
         self.message = message
         super().__init__(self.status_code, self.message)
 
 
 class BadRequestException(BaseErrorHandler):
     """An incorrect request was made to the server.
     Raised for an HTTP status code 400.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
 class UnauthorizedException(BaseErrorHandler):
     """You are incorrectly authorised and may not make this request.
     Raised for an HTTP status code 401.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
 class ForbiddenException(BaseErrorHandler):
     """The server refuses to fulfill this request,
     for instance due to insufficient authentication.
     Raised for an HTTP status code 403.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
 class NotFoundException(BaseErrorHandler):
     """The server couldn't find a resource matching the request.
     Raised for an HTTP status code 404.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
 class TooManyRequestsException(BaseErrorHandler):
     """Your requests limit for the server has been exceeded.
     Raised for an HTTP status code 429.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
 class InternalServerException(BaseErrorHandler):
     """Something unspecified went wrong with the server.
     Raised for an HTTP status code 500.
 
     Attributes
     ----------
     status_code
-        Not used
+        Status code of the error
     message
         A verbose description of this error.
     """
 
 
-def status_handler(status_code, ignore_statuses=None):
+def status_handler(
+    status_code: int, ignore_statuses: Union[Tuple[int], Tuple[()]] = ()
+) -> None:
     "Raises correct custom exception for appropriate HTTP status code."
     if status_code not in ignore_statuses and status_code >= 400:
         if status_code == 400:
             raise BadRequestException(
                 status_code=status_code,
                 message="The request could not be understood by "
                 "the server due to malformed syntax.",
             )
-        if status_code == 401:
+        elif status_code == 401:
             raise UnauthorizedException(
                 status_code=status_code,
                 message="You are incorrectly authorised and "
                 "may not make this request.",
             )
         elif status_code == 403:
             raise ForbiddenException(
```

### Comparing `flightplandb-0.8.0/src/flightplandb/internal.py` & `flightplandb-0.8.1/src/flightplandb/internal.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,23 +42,23 @@
 
 # https://www.sphinx-doc.org/en/master/usage/extensions/autodoc.html#directive-autoclass
 # https://github.com/python/cpython/blob/main/Lib/random.py#L792
 
 url_base: str = "https://api.flightplandatabase.com"
 
 
-def _auth_str(key):
+def _auth_str(key: str) -> str:
     """Returns a API auth string."""
 
     if isinstance(key, str):
-        key = key.encode("latin1")
+        encoded_key = key.encode("latin1")
     else:
         raise ValueError("API key must be a string!")
 
-    authstr = "Basic " + (b64encode(key + b":").strip().decode())
+    authstr = "Basic " + (b64encode(encoded_key + b":").strip().decode())
 
     return authstr
 
 
 format_return_types = {
     # if a dict is requested, the JSON will later be converted to that
     "native": "application/vnd.fpd.v1+json",
@@ -112,68 +112,68 @@
 
 
 @overload
 async def request(
     method: str,
     path: str,
     return_format: native_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Tuple[CIMultiDictProxy[str], Dict]:
+) -> Tuple[CIMultiDictProxy[str], Dict[str, Any]]:
     ...
 
 
 @overload
 async def request(
     method: str,
     path: str,
     return_format: bytes_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> Tuple[CIMultiDictProxy[str], bytes]:
     ...
 
 
 @overload
 async def request(
     method: str,
     path: str,
     return_format: str_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> Tuple[CIMultiDictProxy[str], str]:
     ...
 
 
 async def request(
     method: str,
     path: str,
     return_format: all_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> Tuple[CIMultiDictProxy[str], Union[Any, bytes, str]]:
     """General HTTP requests function for non-paginated results.
 
     Parameters
     ----------
     method : str
         An HTTP request type. One of GET, POST, PATCH, or DELETE
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
         The API response format, defaults to ``"native"``
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     json_data : `Dict`, optional
         Custom JSON data to be formatted into the request body
     key : str
@@ -192,16 +192,14 @@
     ------
     ValueError
         Invalid return_format option
     HTTPError
         Invalid HTTP status in response
     """
 
-    if not ignore_statuses:
-        ignore_statuses = []
     if not params:
         params = {}
     request_headers = {}
 
     # the API only takes "true" or "false", not True or False
     # additionally, aiohttp refuses to pass in a boolean or nonetype in the params
     _null_keys = []
@@ -272,76 +270,73 @@
     return headers
 
 
 @overload
 async def get(
     path: str,
     return_format: native_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Dict:
+) -> Union[Dict[str, Any], List[Any]]:
     ...
 
 
 @overload
 async def get(
     path: str,
     return_format: bytes_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> bytes:
     ...
 
 
 @overload
 async def get(
     path: str,
     return_format: str_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> str:
     ...
 
 
 async def get(
     path: str,
     return_format: all_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Union[Dict, str, bytes]:
+) -> Union[Dict[str, Any], List[Any], str, bytes]:
     """Calls :meth:`request()` for get requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
         The API response format, defaults to ``"native"``
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
         A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
         depending on if the return format is UTF-8 or something else.
     """
 
-    # I HATE not being able to set empty lists as default arguments
-    if not ignore_statuses:
-        ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="get",
         path=path,
         return_format=return_format,
@@ -352,63 +347,63 @@
     return resp
 
 
 @overload
 async def post(
     path: str,
     return_format: native_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Dict:
+) -> Dict[str, Any]:
     ...
 
 
 @overload
 async def post(
     path: str,
     return_format: bytes_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> bytes:
     ...
 
 
 @overload
 async def post(
     path: str,
     return_format: str_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> str:
     ...
 
 
 async def post(
     path: str,
     return_format: all_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Union[Dict, str, bytes]:
+) -> Union[Dict[str, Any], str, bytes]:
     """Calls :meth:`request()` for post requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
         The API response format, defaults to ``"native"``
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     json_data : `Dict`, optional
         Custom JSON data to be formatted into the request body
     key : `str`, optional
@@ -416,16 +411,15 @@
 
     Returns
     -------
     Union[Dict, bytes]
         A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
         depending on if the return format is UTF-8 or something else.
     """
-    if not ignore_statuses:
-        ignore_statuses = []
+
     if not params:
         params = {}
 
     _, resp = await request(
         method="post",
         path=path,
         return_format=return_format,
@@ -437,63 +431,63 @@
     return resp
 
 
 @overload
 async def patch(
     path: str,
     return_format: native_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Dict:
+) -> Dict[str, Any]:
     ...
 
 
 @overload
 async def patch(
     path: str,
     return_format: bytes_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> bytes:
     ...
 
 
 @overload
 async def patch(
     path: str,
     return_format: str_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> str:
     ...
 
 
 async def patch(
     path: str,
     return_format: all_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
-    json_data: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
+    json_data: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Union[Dict, str, bytes]:
+) -> Union[Dict[str, Any], str, bytes]:
     """Calls :meth:`request()` for patch requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
         The API response format, defaults to ``"native"``
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     json_data : `Dict`, optional
         Custom JSON data to be formatted into the request body
     key : `str`, optional
@@ -502,16 +496,14 @@
     Returns
     -------
     Union[Dict, bytes]
         A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
         depending on if the return format is UTF-8 or something else.
     """
 
-    if not ignore_statuses:
-        ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="patch",
         path=path,
         return_format=return_format,
@@ -523,75 +515,73 @@
     return resp
 
 
 @overload
 async def delete(
     path: str,
     return_format: native_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Dict:
+) -> Dict[str, Any]:
     ...
 
 
 @overload
 async def delete(
     path: str,
     return_format: bytes_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> bytes:
     ...
 
 
 @overload
 async def delete(
     path: str,
     return_format: str_return_types_hints,
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
 ) -> str:
     ...
 
 
 async def delete(
     path: str,
     return_format: all_return_types_hints = "native",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> Union[Dict, str, bytes]:
+) -> Union[Dict[str, Any], str, bytes]:
     """Calls :meth:`request()` for delete requests.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     return_format : `str`, optional
         The API response format, defaults to ``"native"``
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     Union[Dict, bytes]
         A ``Dict`` if ``return_format`` is ``"native"``, otherwise ``str`` or ``bytes``
         depending on if the return format is UTF-8 or something else.
     """
 
-    if not ignore_statuses:
-        ignore_statuses = []
     if not params:
         params = {}
 
     _, resp = await request(
         method="delete",
         path=path,
         return_format=return_format,
@@ -602,45 +592,43 @@
     return resp
 
 
 async def getiter(
     path: str,
     limit: int = 100,
     sort: str = "created",
-    ignore_statuses: Optional[List] = None,
-    params: Optional[Dict] = None,
+    ignore_statuses: Union[Tuple[int], Tuple[()]] = (),
+    params: Optional[Dict[str, Any]] = None,
     key: Optional[str] = None,
-) -> AsyncIterable[Dict]:
+) -> AsyncIterable[Dict[str, Any]]:
     """Get :meth:`request()` for paginated results.
 
     Parameters
     ----------
     path : str
         The endpoint's path to which the request is being made
     limit : int, optional
         Maximum number of results to return, defaults to 100
     sort : `str`, optional
         Sort order to return results in. Valid sort orders are
         created, updated, popularity, and distance
-    ignore_statuses : `List`, optional
+    ignore_statuses : `Tuple`, optional
         Statuses (together with 200 OK) which don't
         raise an HTTPError, defaults to None
     params : `Dict`, optional
         Any other HTTP request parameters, defaults to None
     key : `str`, optional
         API token, defaults to None (which makes it unauthenticated)
 
     Returns
     -------
     AsyncIterable[Dict]
         An iterable of dicts. Return format cannot be specified.
     """
 
-    if not ignore_statuses:
-        ignore_statuses = []
     if not params:
         params = {}
     request_headers = {}
 
     valid_sort_orders = ["created", "updated", "popularity", "distance"]
     if sort not in valid_sort_orders:
         raise ValueError(f"sort argument must be one of {', '.join(valid_sort_orders)}")
```

### Comparing `flightplandb-0.8.0/src/flightplandb/nav.py` & `flightplandb-0.8.1/src/flightplandb/nav.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Commands related to navigation aids and airports."""
-from typing import AsyncIterable, List, Optional
+from typing import AsyncIterable, Dict, List, Optional
 
 from flightplandb import internal
 from flightplandb.datatypes import Airport, SearchNavaid, Track
 
 
 async def airport(icao: str, key: Optional[str] = None) -> Airport:
     """Fetches information about an airport.
@@ -23,15 +23,21 @@
     Raises
     ------
     :class:`~flightplandb.exceptions.BadRequestException`
         No airport with the specified ICAO code was found.
     """
 
     resp = await internal.get(path=f"/nav/airport/{icao}", key=key)
-    return Airport(**resp)
+    if isinstance(resp, Dict):
+        return Airport(**resp)
+    else:
+        raise ValueError(
+            "Could not convert response to a Airport datatype; "
+            "it is not a valid mapping"
+        )
 
 
 async def nats(key: Optional[str] = None) -> List[Track]:
     """Fetches current North Atlantic Tracks.
 
     Parameters
     ----------
```

### Comparing `flightplandb-0.8.0/src/flightplandb/plan.py` & `flightplandb-0.8.1/src/flightplandb/plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Flightplan-related commands."""
-from typing import AsyncIterable, Dict, Optional, Union, overload
+from typing import Any, AsyncIterable, Dict, Optional, Union, overload
 
 from flightplandb import internal
 from flightplandb.datatypes import GenerateQuery, Plan, PlanQuery, StatusResponse
 
 
 @overload
 async def fetch(
@@ -30,15 +30,15 @@
     ...
 
 
 async def fetch(
     id_: int,
     return_format: internal.all_return_types_hints = "native",
     key: Optional[str] = None,
-) -> Union[Plan, Dict, str, bytes]:
+) -> Union[Plan, Dict[str, Any], str, bytes]:
     # Underscore for id_ must be escaped as id\_ so sphinx shows the _.
     # However, this would raise W605. To fix this, a raw string is used.
     r"""
     Fetches a flight plan and its associated attributes by ID.
     Returns it in specified format.
 
     Parameters
@@ -69,16 +69,18 @@
 
     request = await internal.get(
         path=f"/plan/{id_}", return_format=return_format, key=key
     )
 
     if isinstance(request, dict) and return_format in internal.native_return_values:
         return Plan(**request)
-    else:
+    elif isinstance(request, (dict, str, bytes)):
         return request
+    else:
+        raise ValueError(f"Expected dict, str, or bytes response, got {type(request)}")
 
 
 @overload
 async def create(
     plan: Plan,
     return_format: internal.native_return_types_hints = "native",
     key: Optional[str] = None,
@@ -104,15 +106,15 @@
     ...
 
 
 async def create(
     plan: Plan,
     return_format: internal.all_return_types_hints = "native",
     key: Optional[str] = None,
-) -> Union[Plan, Dict, bytes, str]:
+) -> Union[Plan, Dict[str, Any], bytes, str]:
     """Creates a new flight plan.
 
     Requires authentication.
 
     Parameters
     ----------
     plan : Plan
@@ -181,15 +183,15 @@
     ...
 
 
 async def edit(
     plan: Plan,
     return_format: internal.all_return_types_hints = "native",
     key: Optional[str] = None,
-) -> Union[Plan, Dict, bytes, str]:
+) -> Union[Plan, Dict[str, Any], bytes, str]:
     """Edits a flight plan linked to your account.
 
     Requires authentication.
 
     Parameters
     ----------
     plan : Plan
@@ -321,17 +323,22 @@
 
     Returns
     -------
     bool
         ``True``/``False`` to indicate that the plan was liked / not liked
     """
 
-    resp = await internal.get(path=f"/plan/{id_}/like", ignore_statuses=[404], key=key)
-    status_response = StatusResponse(**resp)
-    return status_response.message != "Not Found"
+    resp = await internal.get(path=f"/plan/{id_}/like", ignore_statuses=(404,), key=key)
+    if isinstance(resp, Dict):
+        return StatusResponse(**resp).message != "Not Found"
+    else:
+        raise ValueError(
+            "Could not convert response to a StatusResponse datatype; "
+            "it is not a valid mapping"
+        )
 
 
 async def like(id_: int, key: Optional[str] = None) -> StatusResponse:
     r"""Likes a flight plan.
 
     Requires authentication.
```

### Comparing `flightplandb-0.8.0/src/flightplandb/tags.py` & `flightplandb-0.8.1/src/flightplandb/tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Contains the command for fetching flight plan tags."""
-from typing import List, Optional
+from typing import Dict, List, Optional
 
 from flightplandb import internal
 from flightplandb.datatypes import Tag
 
 
 async def fetch(key: Optional[str] = None) -> List[Tag]:
     """Fetches current popular tags from all flight plans.
@@ -16,8 +16,16 @@
 
     Returns
     ----------
     List[Tag]
         A list of the current popular tags.
     """
 
-    return list(map(lambda t: Tag(**t), await internal.get(path="/tags", key=key)))
+    tags_list = []
+    for tag in await internal.get(path="/tags", key=key):
+        if isinstance(tag, Dict):
+            tags_list.append(Tag(**tag))
+        else:
+            raise ValueError(
+                f"could not convert {tag} to a Tag datatype; it is not a valid mapping"
+            )
+    return tags_list
```

### Comparing `flightplandb-0.8.0/src/flightplandb/user.py` & `flightplandb-0.8.1/src/flightplandb/user.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Commands related to registered users."""
-from typing import AsyncIterable, Optional
+from typing import AsyncIterable, Dict, Optional
 
 from flightplandb import internal
 from flightplandb.datatypes import Plan, User, UserSmall
 
 
 async def me(key: Optional[str] = None) -> User:
     """Fetches profile information for the currently authenticated user.
@@ -23,15 +23,20 @@
     Raises
     ------
     :class:`~flightplandb.exceptions.UnauthorizedException`
         Authentication failed.
     """
 
     resp = await internal.get(path="/me", key=key)
-    return User(**resp)
+    if isinstance(resp, Dict):
+        return User(**resp)
+    else:
+        raise ValueError(
+            "could not convert response to a User datatype; it is not a valid mapping"
+        )
 
 
 async def fetch(username: str, key: Optional[str] = None) -> User:
     """Fetches profile information for any registered user
 
     Parameters
     ----------
@@ -48,15 +53,20 @@
     Raises
     -------
     :class:`~flightplandb.exceptions.NotFoundException`
         No user was found with this username.
     """
 
     resp = await internal.get(path=f"/user/{username}", key=key)
-    return User(**resp)
+    if isinstance(resp, Dict):
+        return User(**resp)
+    else:
+        raise ValueError(
+            "could not convert response to a User datatype; it is not a valid mapping"
+        )
 
 
 async def plans(
     username: str, sort: str = "created", limit: int = 100, key: Optional[str] = None
 ) -> AsyncIterable[Plan]:
     """Fetches flight plans created by a user.
 
@@ -111,15 +121,15 @@
     async for i in internal.getiter(
         path=f"/user/{username}/likes", sort=sort, limit=limit, key=key
     ):
         yield Plan(**i)
 
 
 async def search(
-    username: str, limit=100, key: Optional[str] = None
+    username: str, limit: int = 100, key: Optional[str] = None
 ) -> AsyncIterable[UserSmall]:
     """Searches for users by username. For more detailed info on a
     specific user, use :meth:`fetch`
 
     Parameters
     ----------
     username : str
```

### Comparing `flightplandb-0.8.0/src/flightplandb.egg-info/PKG-INFO` & `flightplandb-0.8.1/src/flightplandb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flightplandb
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python wrapper for the Flight Plan Database API
 Author-email: PH-KDX <smtp.python.email.sender@gmail.com>
 License: GPL v3
 Project-URL: Homepage, https://github.com/PH-KDX/flightplandb-py/
 Project-URL: Documentation, https://flightplandb-py.readthedocs.io/
 Project-URL: Issue tracker, https://github.com/PH-KDX/flightplandb-py/issues
 Project-URL: Changelog, https://github.com/PH-KDX/flightplandb-py/blob/main/CHANGELOG.rst
```

### Comparing `flightplandb-0.8.0/src/flightplandb.egg-info/SOURCES.txt` & `flightplandb-0.8.1/src/flightplandb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/tests/test_api.py` & `flightplandb-0.8.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/tests/test_nav.py` & `flightplandb-0.8.1/tests/test_nav.py`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/tests/test_plan.py` & `flightplandb-0.8.1/tests/test_plan.py`

 * *Files 0% similar despite different names*

```diff
@@ -616,15 +616,15 @@
     correct_response = True
 
     patched_internal_get.return_value = json_response
 
     response = await flightplandb.plan.has_liked(42)
     # check that TagsAPI method made correct request of FlightPlanDB
     patched_internal_get.assert_awaited_once_with(
-        path="/plan/42/like", ignore_statuses=[404], key=None
+        path="/plan/42/like", ignore_statuses=(404,), key=None
     )
     # check that TagsAPI method decoded data correctly for given response
     assert response == correct_response
 
 
 @pytest.mark.allow_hosts(["127.0.0.1", "::1"])
 @mock.patch("flightplandb.internal.post")
```

### Comparing `flightplandb-0.8.0/tests/test_tags.py` & `flightplandb-0.8.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/tests/test_user.py` & `flightplandb-0.8.1/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `flightplandb-0.8.0/tests/test_weather.py` & `flightplandb-0.8.1/tests/test_weather.py`

 * *Files identical despite different names*

