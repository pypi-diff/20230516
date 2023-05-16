# Comparing `tmp/vivarium-core-1.5.5.tar.gz` & `tmp/vivarium-core-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-core-1.5.5.tar", last modified: Wed Feb  8 15:37:49 2023, max compression
+gzip compressed data, was "vivarium-core-1.5.6.tar", last modified: Tue May 16 13:45:18 2023, max compression
```

## Comparing `vivarium-core-1.5.5.tar` & `vivarium-core-1.5.6.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.392541 vivarium-core-1.5.5/
--rw-r--r--   0 eranagmon   (502) staff       (20)      733 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/AUTHORS.md
--rw-r--r--   0 eranagmon   (502) staff       (20)    11357 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/LICENSE.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-02-08 15:37:49.392390 vivarium-core-1.5.5/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)     4124 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/README.md
--rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-02-08 15:37:49.392597 vivarium-core-1.5.5/setup.cfg
--rw-r--r--   0 eranagmon   (502) staff       (20)     2836 2023-02-08 15:36:57.000000 vivarium-core-1.5.5/setup.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.377409 vivarium-core-1.5.5/vivarium/
--rw-r--r--   0 eranagmon   (502) staff       (20)     4085 2022-11-09 18:29:14.000000 vivarium-core-1.5.5/vivarium/__init__.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.378002 vivarium-core-1.5.5/vivarium/composites/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/composites/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1369 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/composites/injected_glc_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26070 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/composites/toys.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.381732 vivarium-core-1.5.5/vivarium/core/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    18947 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/composer.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    12095 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/composition.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     9131 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/control.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      394 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/directories.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26791 2022-11-09 18:29:14.000000 vivarium-core-1.5.5/vivarium/core/emitter.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    44691 2023-02-08 15:36:57.000000 vivarium-core-1.5.5/vivarium/core/engine.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    32987 2022-11-09 18:29:14.000000 vivarium-core-1.5.5/vivarium/core/process.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    13882 2022-11-09 21:33:51.000000 vivarium-core-1.5.5/vivarium/core/registry.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    10221 2022-11-09 22:22:40.000000 vivarium-core-1.5.5/vivarium/core/serialize.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     7123 2022-11-09 18:29:14.000000 vivarium-core-1.5.5/vivarium/core/serialize_test.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    72477 2023-02-08 15:36:57.000000 vivarium-core-1.5.5/vivarium/core/store.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1588 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/core/types.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.384001 vivarium-core-1.5.5/vivarium/experiments/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2823 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/bigraph_view.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1005 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/composite_merge.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    36860 2022-11-09 18:29:14.000000 vivarium-core-1.5.5/vivarium/experiments/engine_tests.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2663 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3446 2023-02-08 15:36:57.000000 vivarium-core-1.5.5/vivarium/experiments/hierarchy_composite_division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3055 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/large_experiment.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2955 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/profile_image.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    20995 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/profile_runtime.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     8444 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/store_api.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/experiments/test_profiler.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.386062 vivarium-core-1.5.5/vivarium/library/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1897 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/datum.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11391 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/dict_utils.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3255 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/filepath.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5183 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/make_network.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      145 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/path.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1803 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/pretty.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1789 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/schema.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11820 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/timeseries.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11352 2023-02-06 17:30:02.000000 vivarium-core-1.5.5/vivarium/library/topology.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2948 2022-11-09 22:22:40.000000 vivarium-core-1.5.5/vivarium/library/units.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2209 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/library/wrappers.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.386772 vivarium-core-1.5.5/vivarium/plots/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/plots/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11417 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/plots/agents_multigen.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    11493 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/plots/simulation_output.py
--rw-r--r--   0 eranagmon   (502) staff       (20)    26041 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/plots/topology.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.391369 vivarium-core-1.5.5/vivarium/processes/
--rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/__init__.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6105 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/alternator.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5018 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/burst.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      538 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/clock.py
--rw-r--r--   0 eranagmon   (502) staff       (20)      949 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/divide_condition.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2413 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5685 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/ecoli_shape_deriver.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5077 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/engulf.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3480 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3080 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/growth_rate.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3235 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/injector.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6894 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/mass_adaptor.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     6681 2023-02-08 15:36:57.000000 vivarium-core-1.5.5/vivarium/processes/meta_division.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3423 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/molarity_deriver.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     2432 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/nonspatial_environment.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3244 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/remove.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     1403 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/strip_units.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     5558 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/swap_processes.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3745 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/template_process.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     3260 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/timeline.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     7701 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/toy_gillespie.py
--rw-r--r--   0 eranagmon   (502) staff       (20)     4600 2022-09-07 22:46:45.000000 vivarium-core-1.5.5/vivarium/processes/tree_mass.py
-drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-02-08 15:37:49.392172 vivarium-core-1.5.5/vivarium_core.egg-info/
--rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (502) staff       (20)     2408 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)       20 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/entry_points.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)      115 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-02-08 15:37:49.000000 vivarium-core-1.5.5/vivarium_core.egg-info/top_level.txt
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.130659 vivarium-core-1.5.6/
+-rw-r--r--   0 eranagmon   (502) staff       (20)      733 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/AUTHORS.md
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11357 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/LICENSE.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-05-16 13:45:18.130518 vivarium-core-1.5.6/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4124 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/README.md
+-rw-r--r--   0 eranagmon   (502) staff       (20)       38 2023-05-16 13:45:18.130711 vivarium-core-1.5.6/setup.cfg
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2836 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/setup.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.117496 vivarium-core-1.5.6/vivarium/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4085 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/__init__.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.118086 vivarium-core-1.5.6/vivarium/composites/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/composites/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1369 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/composites/injected_glc_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    26070 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/composites/toys.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.121284 vivarium-core-1.5.6/vivarium/core/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    18947 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/composer.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    12095 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/composition.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     9131 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/control.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      394 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/core/directories.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    26791 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/emitter.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    44691 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/engine.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    32987 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/process.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    13882 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/registry.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    10214 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/vivarium/core/serialize.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     7123 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/core/serialize_test.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    72491 2023-05-16 13:45:05.000000 vivarium-core-1.5.6/vivarium/core/store.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1588 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/core/types.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.123400 vivarium-core-1.5.6/vivarium/experiments/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2823 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/bigraph_view.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1005 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/composite_merge.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    36860 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/engine_tests.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2663 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3446 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/hierarchy_composite_division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3055 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/large_experiment.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2955 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/experiments/profile_image.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    20995 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/profile_runtime.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     8444 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/store_api.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1429 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/experiments/test_profiler.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.125476 vivarium-core-1.5.6/vivarium/library/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1897 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/datum.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11391 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/library/dict_utils.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3255 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/filepath.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5183 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/make_network.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      145 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/path.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1803 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/pretty.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1789 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/schema.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11820 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/timeseries.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11352 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/library/topology.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2948 2023-05-02 22:25:02.000000 vivarium-core-1.5.6/vivarium/library/units.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2209 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/library/wrappers.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.126020 vivarium-core-1.5.6/vivarium/plots/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11417 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/agents_multigen.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    11493 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/simulation_output.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)    26041 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/plots/topology.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.129551 vivarium-core-1.5.6/vivarium/processes/
+-rw-r--r--   0 eranagmon   (502) staff       (20)        0 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/__init__.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6105 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/alternator.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5018 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/burst.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      538 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/clock.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)      949 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/divide_condition.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2413 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5685 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/ecoli_shape_deriver.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5077 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/engulf.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3480 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3080 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/growth_rate.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3235 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/injector.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6894 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/mass_adaptor.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6681 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/meta_division.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3423 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/molarity_deriver.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2432 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/nonspatial_environment.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3244 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/remove.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     1403 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/strip_units.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     5558 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/swap_processes.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3745 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/template_process.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     3260 2022-09-07 22:46:45.000000 vivarium-core-1.5.6/vivarium/processes/timeline.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     7701 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/toy_gillespie.py
+-rw-r--r--   0 eranagmon   (502) staff       (20)     4600 2023-05-16 13:18:03.000000 vivarium-core-1.5.6/vivarium/processes/tree_mass.py
+drwxr-xr-x   0 eranagmon   (502) staff       (20)        0 2023-05-16 13:45:18.130318 vivarium-core-1.5.6/vivarium_core.egg-info/
+-rw-r--r--   0 eranagmon   (502) staff       (20)     6265 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/PKG-INFO
+-rw-r--r--   0 eranagmon   (502) staff       (20)     2408 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/SOURCES.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        1 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/dependency_links.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)       20 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/entry_points.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)      115 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/requires.txt
+-rw-r--r--   0 eranagmon   (502) staff       (20)        9 2023-05-16 13:45:18.000000 vivarium-core-1.5.6/vivarium_core.egg-info/top_level.txt
```

### Comparing `vivarium-core-1.5.5/AUTHORS.md` & `vivarium-core-1.5.6/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/LICENSE.txt` & `vivarium-core-1.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/PKG-INFO` & `vivarium-core-1.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.5.5
+Version: 1.5.6
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
```

### Comparing `vivarium-core-1.5.5/README.md` & `vivarium-core-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/setup.py` & `vivarium-core-1.5.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup
 
 
-VERSION = '1.5.5'
+VERSION = '1.5.6'
 
 
 if __name__ == '__main__':
     with open("README.md", 'r') as readme:
         description = readme.read()
         # Patch the relative links to absolute URLs that will work on PyPI.
         description2 = re.sub(
```

### Comparing `vivarium-core-1.5.5/vivarium/__init__.py` & `vivarium-core-1.5.6/vivarium/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/composites/injected_glc_phosphorylation.py` & `vivarium-core-1.5.6/vivarium/composites/injected_glc_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/composites/toys.py` & `vivarium-core-1.5.6/vivarium/composites/toys.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/composer.py` & `vivarium-core-1.5.6/vivarium/core/composer.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/composition.py` & `vivarium-core-1.5.6/vivarium/core/composition.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/control.py` & `vivarium-core-1.5.6/vivarium/core/control.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/emitter.py` & `vivarium-core-1.5.6/vivarium/core/emitter.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/engine.py` & `vivarium-core-1.5.6/vivarium/core/engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/process.py` & `vivarium-core-1.5.6/vivarium/core/process.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/registry.py` & `vivarium-core-1.5.6/vivarium/core/registry.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/serialize.py` & `vivarium-core-1.5.6/vivarium/core/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 import math
 import warnings
 from typing import Any, List, Union
 from collections.abc import Callable
 
 import orjson
 import numpy as np
-from pint import Unit
-try:
-    from pint.quantity import Quantity
-except ImportError:
-    from pint import Quantity
+# from pint import Unit
+# try:
+#     from pint.quantity import Quantity
+# except ImportError:
+#     from pint import Quantity
 from vivarium.core.process import Process
 from vivarium.library.units import units
 from vivarium.core.registry import serializer_registry, Serializer
 
 
 def find_numpy_and_non_strings(
     d: dict,
@@ -165,16 +165,15 @@
     def can_deserialize(self, data: Any) -> bool:
         if not isinstance(data, str):
             return False
         return bool(self.regex_for_serialized.fullmatch(data))
 
     # Here the differing argument is `unit`, which is optional, so we
     # can ignore the pylint warning.
-    def deserialize(  # pylint: disable=arguments-differ
-            self, data: str, unit: Unit = None) -> Quantity:
+    def deserialize(self, data: str, unit=None):  # type: ignore  # pylint: disable=arguments-differ
         """Deserialize data with units from a human-readable string.
 
         Args:
             data: The data to deserialize. Providing a list here is
                 deprecated. You should use ``deserialize_value``
                 instead, which uses a separate list deserializer.
             unit: The units to convert ``data`` to after deserializing.
```

### Comparing `vivarium-core-1.5.5/vivarium/core/serialize_test.py` & `vivarium-core-1.5.6/vivarium/core/serialize_test.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/core/store.py` & `vivarium-core-1.5.6/vivarium/core/store.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import uuid
 import warnings
 
 import numpy as np
 from pint import Unit, Quantity
 from typing import Optional
 
-from vivarium import divider_registry, serializer_registry, updater_registry
+from vivarium.core.registry import divider_registry, serializer_registry, updater_registry
 from vivarium.core.process import ParallelProcess, Process
 from vivarium.library.dict_utils import deep_merge, deep_merge_check, MULTI_UPDATE_KEY
 from vivarium.library.topology import dict_to_paths
 from vivarium.core.types import Processes, Topology, State, Steps, Flow
 from vivarium.core.serialize import QuantitySerializer
 
 _EMPTY_UPDATES = None, None, None, None, None, None
```

### Comparing `vivarium-core-1.5.5/vivarium/core/types.py` & `vivarium-core-1.5.6/vivarium/core/types.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/bigraph_view.py` & `vivarium-core-1.5.6/vivarium/experiments/bigraph_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/composite_merge.py` & `vivarium-core-1.5.6/vivarium/experiments/composite_merge.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/engine_tests.py` & `vivarium-core-1.5.6/vivarium/experiments/engine_tests.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/glucose_phosphorylation.py` & `vivarium-core-1.5.6/vivarium/experiments/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/hierarchy_composite_division.py` & `vivarium-core-1.5.6/vivarium/experiments/hierarchy_composite_division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/large_experiment.py` & `vivarium-core-1.5.6/vivarium/experiments/large_experiment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/profile_image.py` & `vivarium-core-1.5.6/vivarium/experiments/profile_image.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/profile_runtime.py` & `vivarium-core-1.5.6/vivarium/experiments/profile_runtime.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/store_api.py` & `vivarium-core-1.5.6/vivarium/experiments/store_api.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/experiments/test_profiler.py` & `vivarium-core-1.5.6/vivarium/experiments/test_profiler.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/datum.py` & `vivarium-core-1.5.6/vivarium/library/datum.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/dict_utils.py` & `vivarium-core-1.5.6/vivarium/library/dict_utils.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/filepath.py` & `vivarium-core-1.5.6/vivarium/library/filepath.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/make_network.py` & `vivarium-core-1.5.6/vivarium/library/make_network.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/pretty.py` & `vivarium-core-1.5.6/vivarium/library/pretty.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/schema.py` & `vivarium-core-1.5.6/vivarium/library/schema.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/timeseries.py` & `vivarium-core-1.5.6/vivarium/library/timeseries.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/topology.py` & `vivarium-core-1.5.6/vivarium/library/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/units.py` & `vivarium-core-1.5.6/vivarium/library/units.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/library/wrappers.py` & `vivarium-core-1.5.6/vivarium/library/wrappers.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/plots/agents_multigen.py` & `vivarium-core-1.5.6/vivarium/plots/agents_multigen.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/plots/simulation_output.py` & `vivarium-core-1.5.6/vivarium/plots/simulation_output.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/plots/topology.py` & `vivarium-core-1.5.6/vivarium/plots/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/alternator.py` & `vivarium-core-1.5.6/vivarium/processes/alternator.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/burst.py` & `vivarium-core-1.5.6/vivarium/processes/burst.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/clock.py` & `vivarium-core-1.5.6/vivarium/processes/clock.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/divide_condition.py` & `vivarium-core-1.5.6/vivarium/processes/divide_condition.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/division.py` & `vivarium-core-1.5.6/vivarium/processes/division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/ecoli_shape_deriver.py` & `vivarium-core-1.5.6/vivarium/processes/ecoli_shape_deriver.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/engulf.py` & `vivarium-core-1.5.6/vivarium/processes/engulf.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/glucose_phosphorylation.py` & `vivarium-core-1.5.6/vivarium/processes/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/growth_rate.py` & `vivarium-core-1.5.6/vivarium/processes/growth_rate.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/injector.py` & `vivarium-core-1.5.6/vivarium/processes/injector.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/mass_adaptor.py` & `vivarium-core-1.5.6/vivarium/processes/mass_adaptor.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/meta_division.py` & `vivarium-core-1.5.6/vivarium/processes/meta_division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/molarity_deriver.py` & `vivarium-core-1.5.6/vivarium/processes/molarity_deriver.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/nonspatial_environment.py` & `vivarium-core-1.5.6/vivarium/processes/nonspatial_environment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/remove.py` & `vivarium-core-1.5.6/vivarium/processes/remove.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/strip_units.py` & `vivarium-core-1.5.6/vivarium/processes/strip_units.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/swap_processes.py` & `vivarium-core-1.5.6/vivarium/processes/swap_processes.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/template_process.py` & `vivarium-core-1.5.6/vivarium/processes/template_process.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/timeline.py` & `vivarium-core-1.5.6/vivarium/processes/timeline.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/toy_gillespie.py` & `vivarium-core-1.5.6/vivarium/processes/toy_gillespie.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium/processes/tree_mass.py` & `vivarium-core-1.5.6/vivarium/processes/tree_mass.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.5.5/vivarium_core.egg-info/PKG-INFO` & `vivarium-core-1.5.6/vivarium_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.5.5
+Version: 1.5.6
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
```

### Comparing `vivarium-core-1.5.5/vivarium_core.egg-info/SOURCES.txt` & `vivarium-core-1.5.6/vivarium_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

