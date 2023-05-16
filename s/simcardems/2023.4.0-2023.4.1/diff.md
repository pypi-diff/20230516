# Comparing `tmp/simcardems-2023.4.0.tar.gz` & `tmp/simcardems-2023.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simcardems-2023.4.0.tar", last modified: Wed May 10 08:10:53 2023, max compression
+gzip compressed data, was "simcardems-2023.4.1.tar", last modified: Tue May 16 08:44:01 2023, max compression
```

## Comparing `simcardems-2023.4.0.tar` & `simcardems-2023.4.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.958935 simcardems-2023.4.0/
--rw-r--r--   0 root         (0) root         (0)    26526 2023-05-10 07:53:22.000000 simcardems-2023.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-10 08:10:53.958935 simcardems-2023.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3141 2023-05-10 07:53:22.000000 simcardems-2023.4.0/README.md
--rw-r--r--   0 root         (0) root         (0)     1831 2023-05-10 08:10:53.958935 simcardems-2023.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      296 2023-05-10 07:53:22.000000 simcardems-2023.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.938935 simcardems-2023.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.946935 simcardems-2023.4.0/src/simcardems/
--rw-r--r--   0 root         (0) root         (0)     3453 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/__init__.py
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/__main__.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/cli.py
--rw-r--r--   0 root         (0) root         (0)     1919 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/config.py
--rw-r--r--   0 root         (0) root         (0)    18669 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/datacollector.py
--rw-r--r--   0 root         (0) root         (0)     9907 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/ep_model.py
--rw-r--r--   0 root         (0) root         (0)    17148 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/geometry.py
--rw-r--r--   0 root         (0) root         (0)    11745 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/gui.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/lvgeometry.py
--rw-r--r--   0 root         (0) root         (0)    11482 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/mechanics_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems/models/
--rw-r--r--   0 root         (0) root         (0)      660 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6841 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      819 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60660 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    14001 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      567 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6993 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    60244 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    11882 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/
--rw-r--r--   0 root         (0) root         (0)      559 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6989 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
--rw-r--r--   0 root         (0) root         (0)    70534 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)    11880 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.954935 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/
--rw-r--r--   0 root         (0) root         (0)      419 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60536 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
--rw-r--r--   0 root         (0) root         (0)     5012 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
--rw-r--r--   0 root         (0) root         (0)     5730 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/newton_solver.py
--rw-r--r--   0 root         (0) root         (0)    21621 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/postprocess.py
--rw-r--r--   0 root         (0) root         (0)     7156 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/runner.py
--rw-r--r--   0 root         (0) root         (0)     6485 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/save_load_functions.py
--rw-r--r--   0 root         (0) root         (0)     4515 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/slabgeometry.py
--rw-r--r--   0 root         (0) root         (0)     2642 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/time_stepper.py
--rw-r--r--   0 root         (0) root         (0)     5462 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/utils.py
--rw-r--r--   0 root         (0) root         (0)     4826 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/value_extractor.py
--rw-r--r--   0 root         (0) root         (0)       25 2023-05-10 07:53:22.000000 simcardems-2023.4.0/src/simcardems/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.950935 simcardems-2023.4.0/src/simcardems.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3845 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2016 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-10 07:53:45.000000 simcardems-2023.4.0/src/simcardems.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-05-10 08:10:53.000000 simcardems-2023.4.0/src/simcardems.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-10 08:10:53.958935 simcardems-2023.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_boundary_conditions.py
--rw-r--r--   0 root         (0) root         (0)     3454 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_cli.py
--rw-r--r--   0 root         (0) root         (0)     2974 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_datacollector.py
--rw-r--r--   0 root         (0) root         (0)     2559 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_geometry.py
--rw-r--r--   0 root         (0) root         (0)     3507 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_mechanics_model.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_models.py
--rw-r--r--   0 root         (0) root         (0)     2793 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_postprocessing.py
--rw-r--r--   0 root         (0) root         (0)     1956 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_runner.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-05-10 07:53:22.000000 simcardems-2023.4.0/tests/test_save_load_functions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/
+-rw-r--r--   0 root         (0) root         (0)    26526 2023-05-16 08:34:16.000000 simcardems-2023.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-16 08:44:01.900084 simcardems-2023.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3141 2023-05-16 08:34:16.000000 simcardems-2023.4.1/README.md
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-05-16 08:44:01.900084 simcardems-2023.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      296 2023-05-16 08:34:16.000000 simcardems-2023.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.888084 simcardems-2023.4.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/
+-rw-r--r--   0 root         (0) root         (0)     3453 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/cli.py
+-rw-r--r--   0 root         (0) root         (0)     1919 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/config.py
+-rw-r--r--   0 root         (0) root         (0)    18669 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     9907 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/ep_model.py
+-rw-r--r--   0 root         (0) root         (0)    17148 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/geometry.py
+-rw-r--r--   0 root         (0) root         (0)    11745 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/gui.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/lvgeometry.py
+-rw-r--r--   0 root         (0) root         (0)    11482 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/mechanics_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/
+-rw-r--r--   0 root         (0) root         (0)      660 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6841 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60660 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    14164 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      567 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6993 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    60244 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12046 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/
+-rw-r--r--   0 root         (0) root         (0)      559 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6989 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/active_model.py
+-rw-r--r--   0 root         (0) root         (0)    70534 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)    12043 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/em_model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/
+-rw-r--r--   0 root         (0) root         (0)      419 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60536 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py
+-rw-r--r--   0 root         (0) root         (0)     5012 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/em_model.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/newton_solver.py
+-rw-r--r--   0 root         (0) root         (0)    21621 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/postprocess.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/runner.py
+-rw-r--r--   0 root         (0) root         (0)     6485 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/save_load_functions.py
+-rw-r--r--   0 root         (0) root         (0)     4515 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/slabgeometry.py
+-rw-r--r--   0 root         (0) root         (0)     2642 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/time_stepper.py
+-rw-r--r--   0 root         (0) root         (0)     5462 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4826 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/value_extractor.py
+-rw-r--r--   0 root         (0) root         (0)       25 2023-05-16 08:34:16.000000 simcardems-2023.4.1/src/simcardems/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.896084 simcardems-2023.4.1/src/simcardems.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3845 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 08:34:34.000000 simcardems-2023.4.1/src/simcardems.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-05-16 08:44:01.000000 simcardems-2023.4.1/src/simcardems.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 08:44:01.900084 simcardems-2023.4.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_boundary_conditions.py
+-rw-r--r--   0 root         (0) root         (0)     3454 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_cli.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_datacollector.py
+-rw-r--r--   0 root         (0) root         (0)     2559 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_geometry.py
+-rw-r--r--   0 root         (0) root         (0)     3507 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_mechanics_model.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     2793 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_postprocessing.py
+-rw-r--r--   0 root         (0) root         (0)     1956 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-05-16 08:34:16.000000 simcardems-2023.4.1/tests/test_save_load_functions.py
```

### Comparing `simcardems-2023.4.0/LICENSE` & `simcardems-2023.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/PKG-INFO` & `simcardems-2023.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.0/README.md` & `simcardems-2023.4.1/README.md`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/setup.cfg` & `simcardems-2023.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/__init__.py` & `simcardems-2023.4.1/src/simcardems/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/benchmark.py` & `simcardems-2023.4.1/src/simcardems/benchmark.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/boundary_conditions.py` & `simcardems-2023.4.1/src/simcardems/boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/cli.py` & `simcardems-2023.4.1/src/simcardems/cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/config.py` & `simcardems-2023.4.1/src/simcardems/config.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/datacollector.py` & `simcardems-2023.4.1/src/simcardems/datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/ep_model.py` & `simcardems-2023.4.1/src/simcardems/ep_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/geometry.py` & `simcardems-2023.4.1/src/simcardems/geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/gui.py` & `simcardems-2023.4.1/src/simcardems/gui.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/lvgeometry.py` & `simcardems-2023.4.1/src/simcardems/lvgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/mechanics_model.py` & `simcardems-2023.4.1/src/simcardems/mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/__init__.py` & `simcardems-2023.4.1/src/simcardems/models/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/em_model.py` & `simcardems-2023.4.1/src/simcardems/models/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/__init__.py` & `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/cell_model.py` & `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/explicit_ORdmm_Land/em_model.py` & `simcardems-2023.4.1/src/simcardems/models/explicit_ORdmm_Land/em_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,19 +89,24 @@
         self,
         f_mech: dolfin.Function,
         f_ep: dolfin.Function,
     ) -> dolfin.Function:
         """Interpolates function from mechanics to ep mesh"""
 
         x = dolfin.as_backend_type(f_mech.vector()).vec()
-        _, temp = self.transfer_matrix.getVecs()
+        a, temp = self.transfer_matrix.getVecs()
         self.transfer_matrix.mult(x, temp)
         f_ep.vector().vec().aypx(0.0, temp)
         f_ep.vector().apply("")
 
+        # Remember to free memory allocated by petsc: https://gitlab.com/petsc/petsc/-/issues/1309
+        x.destroy()
+        a.destroy()
+        temp.destroy()
+
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
 
         if not super().__eq__(__o):
             return False
```

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_ORdmm_Land/em_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,25 @@
         self,
         f_mech: dolfin.Function,
         f_ep: dolfin.Function,
     ) -> dolfin.Function:
         """Interpolates function from mechanics to ep mesh"""
 
         x = dolfin.as_backend_type(f_mech.vector()).vec()
-        _, temp = self.transfer_matrix.getVecs()
+        a, temp = self.transfer_matrix.getVecs()
+
         self.transfer_matrix.mult(x, temp)
         f_ep.vector().vec().aypx(0.0, temp)
         f_ep.vector().apply("")
 
+        # Remember to free memory allocated by petsc: https://gitlab.com/petsc/petsc/-/issues/1309
+        x.destroy()
+        a.destroy()
+        temp.destroy()
+
     @property
     def coupling_type(self):
         return "fully_coupled_ORdmm_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
```

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/__init__.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/__init__.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/active_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/active_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/fully_coupled_Tor_Land/em_model.py` & `simcardems-2023.4.1/src/simcardems/models/fully_coupled_Tor_Land/em_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,19 +56,24 @@
         self,
         f_mech: dolfin.Function,
         f_ep: dolfin.Function,
     ) -> dolfin.Function:
         """Interpolates function from mechanics to ep mesh"""
 
         x = dolfin.as_backend_type(f_mech.vector()).vec()
-        _, temp = self.transfer_matrix.getVecs()
+        a, temp = self.transfer_matrix.getVecs()
         self.transfer_matrix.mult(x, temp)
         f_ep.vector().vec().aypx(0.0, temp)
         f_ep.vector().apply("")
 
+        # Remember to free memory allocated by petsc: https://gitlab.com/petsc/petsc/-/issues/1309
+        x.destroy()
+        a.destroy()
+        temp.destroy()
+
     @property
     def coupling_type(self):
         return "fully_coupled_Tor_Land"
 
     def __eq__(self, __o: object) -> bool:
         if not isinstance(__o, type(self)):
             return NotImplemented
```

### Comparing `simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py` & `simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/cell_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/models/pureEP_ORdmm_Land/em_model.py` & `simcardems-2023.4.1/src/simcardems/models/pureEP_ORdmm_Land/em_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/newton_solver.py` & `simcardems-2023.4.1/src/simcardems/newton_solver.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/postprocess.py` & `simcardems-2023.4.1/src/simcardems/postprocess.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/runner.py` & `simcardems-2023.4.1/src/simcardems/runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/save_load_functions.py` & `simcardems-2023.4.1/src/simcardems/save_load_functions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/slabgeometry.py` & `simcardems-2023.4.1/src/simcardems/slabgeometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/time_stepper.py` & `simcardems-2023.4.1/src/simcardems/time_stepper.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/utils.py` & `simcardems-2023.4.1/src/simcardems/utils.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems/value_extractor.py` & `simcardems-2023.4.1/src/simcardems/value_extractor.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/src/simcardems.egg-info/PKG-INFO` & `simcardems-2023.4.1/src/simcardems.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simcardems
-Version: 2023.4.0
+Version: 2023.4.1
 Summary: Simula Cardiac electromechanics solver
 Home-page: https://github.com/ComputationalPhysiology/simcardems
 Author: Henrik Finsberg, Ilsbeth van Herck, Cécile Daversin-Catty
 Author-email: henriknf@simula.no
 License: LGPL-2.1
 Keywords: action potential,cardiac mechanics,electrophysiology,electromechanics
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
```

### Comparing `simcardems-2023.4.0/src/simcardems.egg-info/SOURCES.txt` & `simcardems-2023.4.1/src/simcardems.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_boundary_conditions.py` & `simcardems-2023.4.1/tests/test_boundary_conditions.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_cli.py` & `simcardems-2023.4.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_datacollector.py` & `simcardems-2023.4.1/tests/test_datacollector.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_geometry.py` & `simcardems-2023.4.1/tests/test_geometry.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_mechanics_model.py` & `simcardems-2023.4.1/tests/test_mechanics_model.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_models.py` & `simcardems-2023.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_postprocessing.py` & `simcardems-2023.4.1/tests/test_postprocessing.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_runner.py` & `simcardems-2023.4.1/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `simcardems-2023.4.0/tests/test_save_load_functions.py` & `simcardems-2023.4.1/tests/test_save_load_functions.py`

 * *Files identical despite different names*

