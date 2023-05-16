# Comparing `tmp/FLORIS-3.3.tar.gz` & `tmp/FLORIS-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLORIS-3.3.tar", last modified: Tue Mar  7 22:45:57 2023, max compression
+gzip compressed data, was "FLORIS-3.4.tar", last modified: Tue May 16 17:48:20 2023, max compression
```

## Comparing `FLORIS-3.3.tar` & `FLORIS-3.4.tar`

### file list

```diff
@@ -1,115 +1,119 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/FLORIS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-07 22:45:57.000000 FLORIS-3.3/FLORIS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-03-07 22:45:57.000000 FLORIS-3.3/FLORIS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 22:45:57.000000 FLORIS-3.3/FLORIS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-07 22:45:57.000000 FLORIS-3.3/FLORIS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 22:45:57.000000 FLORIS-3.3/FLORIS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-07 22:45:47.000000 FLORIS-3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-03-07 22:45:57.707672 FLORIS-3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-03-07 22:45:47.000000 FLORIS-3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/floris/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/logging_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/floris/simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11406 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/farm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/floris.py
--rw-r--r--   0 runner    (1001) docker     (123)     9786 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/flow_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    20291 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    40143 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18484 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/turbine.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/floris/simulation/wake_combination/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_combination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_combination/fls.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_combination/max.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_combination/sosfs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/floris/simulation/wake_deflection/
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_deflection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19672 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_deflection/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_deflection/jimenez.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_deflection/none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.691672 FLORIS-3.3/floris/simulation/wake_turbulence/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_turbulence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_turbulence/crespo_hernandez.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_turbulence/none.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.695672 FLORIS-3.3/floris/simulation/wake_velocity/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/cumulative_gauss_curl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/gauss.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/jensen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/none.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/turbopark.py
--rw-r--r--   0 runner    (1001) docker     (123)  9163212 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/simulation/wake_velocity/turbopark_lookup_table.mat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.703673 FLORIS-3.3/floris/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/cc_blade_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/cut_plane.py
--rw-r--r--   0 runner    (1001) docker     (123)    40330 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/floris_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/floris_interface_legacy_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/flow_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/interface_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/layout_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.703673 FLORIS-3.3/floris/tools/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.703673 FLORIS-3.3/floris/tools/optimization/layout_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.703673 FLORIS-3.3/floris/tools/optimization/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/yaw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/floris/tools/optimization/legacy/scipy/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/base_COE.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/cluster_turbines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
--rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/layout_height.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/optimization.py
--rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/power_density.py
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/power_density_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw.py
--rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)    46052 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
--rw-r--r--   0 runner    (1001) docker     (123)    21991 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
--rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/floris/tools/optimization/other/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/other/boundary_grid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/floris/tools/optimization/yaw_optimization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/yaw_optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12495 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
--rw-r--r--   0 runner    (1001) docker     (123)    21070 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/parallel_computing_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/power_rose.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/rews.py
--rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/sowfa_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    30577 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/uncertainty_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    17736 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)    61531 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/tools/wind_rose.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 22:45:57.707672 FLORIS-3.3/floris/turbine_library/
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/turbine_library/iea_10MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/turbine_library/iea_15MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/turbine_library/nrel_5MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/turbine_library/x_20MW.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/type_dec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-07 22:45:47.000000 FLORIS-3.3/floris/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-03-07 22:45:47.000000 FLORIS-3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 22:45:57.707672 FLORIS-3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-03-07 22:45:47.000000 FLORIS-3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/FLORIS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 17:48:20.000000 FLORIS-3.4/FLORIS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-16 17:48:08.000000 FLORIS-3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-16 17:48:20.151147 FLORIS-3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-05-16 17:48:08.000000 FLORIS-3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/floris/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/logging_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.131147 FLORIS-3.4/floris/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/farm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14075 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/floris.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13379 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/flow_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39069 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58882 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30621 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/turbine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_combination/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/fls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/max.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_combination/sosfs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_deflection/
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19670 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/jimenez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_deflection/none.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_turbulence/
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/crespo_hernandez.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_turbulence/wake_induced_mixing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.135147 FLORIS-3.4/floris/simulation/wake_velocity/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/cumulative_gauss_curl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10723 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/empirical_gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8862 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/gauss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/jensen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/none.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/turbopark.py
+-rw-r--r--   0 runner    (1001) docker     (123)  9163212 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/simulation/wake_velocity/turbopark_lookup_table.mat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/cc_blade_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14537 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/cut_plane.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40510 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/floris_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9305 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/floris_interface_legacy_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5617 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/flow_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9245 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/interface_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13087 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/layout_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/layout_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24334 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7968 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/yaw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/legacy/scipy/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/base_COE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/cluster_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16134 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11986 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout_height.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/optimization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18216 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30497 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14439 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46052 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21991 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26817 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.147147 FLORIS-3.4/floris/tools/optimization/other/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13489 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/other/boundary_grid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/floris/tools/optimization/yaw_optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33490 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13212 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20989 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/parallel_computing_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18526 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/power_rose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/rews.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21079 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/sowfa_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30200 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/uncertainty_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23948 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61639 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/tools/wind_rose.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:48:20.151147 FLORIS-3.4/floris/turbine_library/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/iea_10MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/iea_15MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/nrel_5MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    33041 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/turbine_previewer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/turbine_library/x_20MW.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6539 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/type_dec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11878 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-16 17:48:08.000000 FLORIS-3.4/floris/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-16 17:48:08.000000 FLORIS-3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:48:20.151147 FLORIS-3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-05-16 17:48:08.000000 FLORIS-3.4/setup.py
```

### Comparing `FLORIS-3.3/FLORIS.egg-info/PKG-INFO` & `FLORIS-3.4/FLORIS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.3
+Version: 3.4
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `FLORIS-3.3/FLORIS.egg-info/SOURCES.txt` & `FLORIS-3.4/FLORIS.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -22,37 +22,39 @@
 floris/simulation/turbine.py
 floris/simulation/wake.py
 floris/simulation/wake_combination/__init__.py
 floris/simulation/wake_combination/fls.py
 floris/simulation/wake_combination/max.py
 floris/simulation/wake_combination/sosfs.py
 floris/simulation/wake_deflection/__init__.py
+floris/simulation/wake_deflection/empirical_gauss.py
 floris/simulation/wake_deflection/gauss.py
 floris/simulation/wake_deflection/jimenez.py
 floris/simulation/wake_deflection/none.py
 floris/simulation/wake_turbulence/__init__.py
 floris/simulation/wake_turbulence/crespo_hernandez.py
 floris/simulation/wake_turbulence/none.py
+floris/simulation/wake_turbulence/wake_induced_mixing.py
 floris/simulation/wake_velocity/__init__.py
 floris/simulation/wake_velocity/cumulative_gauss_curl.py
+floris/simulation/wake_velocity/empirical_gauss.py
 floris/simulation/wake_velocity/gauss.py
 floris/simulation/wake_velocity/jensen.py
 floris/simulation/wake_velocity/none.py
 floris/simulation/wake_velocity/turbopark.py
 floris/simulation/wake_velocity/turbopark_lookup_table.mat
 floris/tools/__init__.py
 floris/tools/cc_blade_utilities.py
 floris/tools/cut_plane.py
 floris/tools/floris_interface.py
 floris/tools/floris_interface_legacy_reader.py
 floris/tools/flow_data.py
 floris/tools/interface_utilities.py
 floris/tools/layout_functions.py
 floris/tools/parallel_computing_interface.py
-floris/tools/plotting.py
 floris/tools/power_rose.py
 floris/tools/rews.py
 floris/tools/sowfa_utilities.py
 floris/tools/uncertainty_interface.py
 floris/tools/visualization.py
 floris/tools/wind_rose.py
 floris/tools/optimization/__init__.py
@@ -86,11 +88,13 @@
 floris/tools/optimization/other/__init__.py
 floris/tools/optimization/other/boundary_grid.py
 floris/tools/optimization/yaw_optimization/__init__.py
 floris/tools/optimization/yaw_optimization/yaw_optimization_base.py
 floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py
 floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py
 floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py
+floris/turbine_library/__init__.py
 floris/turbine_library/iea_10MW.yaml
 floris/turbine_library/iea_15MW.yaml
 floris/turbine_library/nrel_5MW.yaml
+floris/turbine_library/turbine_previewer.py
 floris/turbine_library/x_20MW.yaml
```

### Comparing `FLORIS-3.3/LICENSE.txt` & `FLORIS-3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/PKG-INFO` & `FLORIS-3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLORIS
-Version: 3.3
+Version: 3.4
 Summary: A controls-oriented engineering wake model.
 Home-page: https://github.com/NREL/FLORIS
 Author: NREL National Wind Technology Center
 Author-email: rafael.mudafort@nrel.gov
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
```

### Comparing `FLORIS-3.3/README.md` & `FLORIS-3.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FLORIS Wake Modeling and Wind Farm Controls Software
 
 FLORIS is a controls-focused wind farm simulation software incorporating
 steady-state engineering wake models into a performance-focused Python
 framework. It has been in active development at NREL since 2013 and the latest
-release is [FLORIS v3.3](https://github.com/NREL/floris/releases/latest).
+release is [FLORIS v3.4](https://github.com/NREL/floris/releases/latest).
 Online documentation is available at https://nrel.github.io/floris.
 
 The software is in active development and engagement with the development team
 is highly encouraged. If you are interested in using FLORIS to conduct studies
 of a wind farm or extending FLORIS to include your own wake model, please join
 the conversation in [GitHub Discussions](https://github.com/NREL/floris/discussions/)!
 
@@ -61,20 +61,21 @@
     NAME
         floris - # Copyright 2021 NREL
 
     PACKAGE CONTENTS
         logging_manager
         simulation (package)
         tools (package)
+        turbine_library (package)
         type_dec
         utilities
         version
 
     VERSION
-        3.3
+        3.4
 
     FILE
         ~/floris/floris/__init__.py
 ```
 
 It is important to regularly check for new updates and releases as new
 features, improvements, and bug fixes will be issued on an ongoing basis.
```

### Comparing `FLORIS-3.3/floris/__init__.py` & `FLORIS-3.4/floris/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/logging_manager.py` & `FLORIS-3.4/floris/logging_manager.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/__init__.py` & `FLORIS-3.4/floris/simulation/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,22 +33,31 @@
 # that should be included in the simulation package.
 # Since some of these depend on each other, the order
 # that they are listed here does matter.
 
 import floris.logging_manager
 
 from .base import BaseClass, BaseModel, State
-from .turbine import average_velocity, axial_induction, Ct, power, Turbine
+from .turbine import average_velocity, axial_induction, Ct, power, rotor_effective_velocity, Turbine
 from .farm import Farm
-from .grid import FlowFieldGrid, FlowFieldPlanarGrid, Grid, TurbineGrid
+from .grid import (
+    FlowFieldGrid,
+    FlowFieldPlanarGrid,
+    Grid,
+    PointsGrid,
+    TurbineGrid,
+    TurbineCubatureGrid
+)
 from .flow_field import FlowField
 from .wake import WakeModelManager
 from .solver import (
     cc_solver,
+    empirical_gauss_solver,
     full_flow_cc_solver,
+    full_flow_empirical_gauss_solver,
     full_flow_sequential_solver,
     full_flow_turbopark_solver,
     sequential_solver,
     turbopark_solver,
 )
 from .floris import Floris
```

### Comparing `FLORIS-3.3/floris/simulation/base.py` & `FLORIS-3.4/floris/simulation/base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/farm.py` & `FLORIS-3.4/floris/simulation/farm.py`

 * *Files 26% similar despite different names*

```diff
@@ -14,197 +14,244 @@
 
 import copy
 from pathlib import Path
 from typing import Any, List
 
 import attrs
 import numpy as np
-import yaml
 from attrs import define, field
 
 from floris.simulation import (
     BaseClass,
     State,
     Turbine,
 )
+from floris.simulation.turbine import compute_tilt_angles_for_floating_turbines
 from floris.type_dec import (
     convert_to_path,
     floris_array_converter,
+    iter_validator,
     NDArrayFloat,
     NDArrayObject,
 )
 from floris.utilities import load_yaml, Vec3
 
 
 default_turbine_library_path = Path(__file__).parents[1] / "turbine_library"
 
 
 @define
 class Farm(BaseClass):
     """Farm is where wind power plants should be instantiated from a YAML configuration
-    file. The Farm will create a heterogenous set of turbines that compose a windfarm,
+    file. The Farm will create a heterogenous set of turbines that compose a wind farm,
     validate the inputs, and then create a vectorized representation of the the turbine
     data.
 
     Farm is the container class of the FLORIS package. It brings
     together all of the component objects after input (i.e., Turbine,
     Wake, FlowField) and packages everything into the appropriate data
     type. Farm should also be used as an entry point to probe objects
     for generating output.
     """
 
     layout_x: NDArrayFloat = field(converter=floris_array_converter)
     layout_y: NDArrayFloat = field(converter=floris_array_converter)
-    turbine_type: List = field()
+    # TODO: turbine_type should be immutable
+    turbine_type: List = field(validator=iter_validator(list, (dict, str)))
     turbine_library_path: Path = field(
         default=default_turbine_library_path, converter=convert_to_path
     )
 
-    turbine_definitions: dict = field(init=False)
+    turbine_definitions: list = field(init=False, validator=iter_validator(list, dict))
     yaw_angles: NDArrayFloat = field(init=False)
     yaw_angles_sorted: NDArrayFloat = field(init=False)
+    tilt_angles: NDArrayFloat = field(init=False)
+    tilt_angles_sorted: NDArrayFloat = field(init=False)
     coordinates: List[Vec3] = field(init=False)
     hub_heights: NDArrayFloat = field(init=False)
     hub_heights_sorted: NDArrayFloat = field(init=False, default=[])
     turbine_fCts: tuple = field(init=False, default=[])
     turbine_type_map_sorted: NDArrayObject = field(init=False, default=[])
     rotor_diameters_sorted: NDArrayFloat = field(init=False, default=[])
     TSRs_sorted: NDArrayFloat = field(init=False, default=[])
+    pPs: NDArrayFloat = field(init=False, default=[])
     pPs_sorted: NDArrayFloat = field(init=False, default=[])
+    pTs: NDArrayFloat = field(init=False, default=[])
+    pTs_sorted: NDArrayFloat = field(init=False, default=[])
+    ref_tilt_cp_cts: NDArrayFloat = field(init=False, default=[])
+    ref_tilt_cp_cts_sorted: NDArrayFloat = field(init=False, default=[])
+    correct_cp_ct_for_tilt: NDArrayFloat = field(init=False, default=[])
+    correct_cp_ct_for_tilt_sorted: NDArrayFloat = field(init=False, default=[])
+    turbine_fTilts: list = field(init=False, default=[])
 
     def __attrs_post_init__(self) -> None:
-        self.check_turbine_type()
+        # Turbine definitions can be supplied in three ways:
+        # - A string selecting a turbine in the floris turbine library
+        # - A Python dict representation of a turbine definition
+        #   - There's an option to use the yaml keyword "!include" which results in the yaml
+        #     library preprocessing the inputs and loading the specified file directly into
+        #     the main input file. The result is that floris sees the turbine definition as a dict.
+        # - A string selecting an turbine that exists in an external turbine library
+        #   specified in `turbine_library_path`
+
+        # Load all the turbine types into a cache to be mapped to specific turbine indices later.
+        # This allows to read the yaml input files once rather than every time they're given.
+        # In other words, if the turbine type is already in the cache, skip that iteration of
+        # the for-loop.
+        turbine_definition_cache = {}
+        for t in self.turbine_type:
+            # If a turbine type is a dict, then it was either preprocessed by the yaml
+            # library to resolve the "!include" or it was set in a script as a dict. In either case,
+            # add an entry to the cache
+            if isinstance(t, dict):
+                if t["turbine_type"] in turbine_definition_cache:
+                    continue
+                turbine_definition_cache[t["turbine_type"]] = t
+
+            # If a turbine type is a string, then it is expected in the internal or external
+            # turbine library
+            if isinstance(t, str):
+                if t in turbine_definition_cache:
+                    continue
+
+                # Check if the file exists in the internal and/or external library
+                internal_fn = (default_turbine_library_path / t).with_suffix(".yaml")
+                external_fn = (self.turbine_library_path / t).with_suffix(".yaml")
+                in_internal = internal_fn.exists()
+                in_external = external_fn.exists()
+
+                # If an external library is used and there's a duplicate of an internal
+                # definition, then raise an error
+                is_unique_path = self.turbine_library_path != default_turbine_library_path
+                if is_unique_path and in_external and in_internal:
+                    raise ValueError(
+                        f"The turbine type: {t} exists in both the internal and external"
+                        " turbine library."
+                    )
+
+                if in_internal:
+                    full_path = internal_fn
+                elif in_external:
+                    full_path = external_fn
+                else:
+                    raise FileNotFoundError(
+                        f"The turbine type: {t} does not exist in either the internal or"
+                        " external turbine library."
+                    )
+                turbine_definition_cache[t] = load_yaml(full_path)
+
+        # Convert any dict entries in the turbine_type list to the type string. Since the
+        # definition is saved above, we can make the whole list consistent now to use it
+        # for mapping turbines later.
+        # We use a private variable here instead of self.turbine_type because self.turbine_type
+        # should always retain the input data. When this class is exported as_dict, the input
+        # types must be used. If we modify that directly and change its shape, recreating this
+        # class with a different layout but not a new self.turbine_type could cause the data
+        # to be out of sync.
+        _turbine_types = [
+            copy.deepcopy(t["turbine_type"]) if isinstance(t, dict) else t
+            for t in self.turbine_type
+        ]
+
+        # If 1 turbine definition is given, expand to N turbines; this covers a 1-turbine
+        # farm and 1 definition for multiple turbines
+        if len(_turbine_types) == 1:
+            _turbine_types *= self.n_turbines
+
+        # Map each turbine definition to its index in this list
+        self.turbine_definitions = [
+            copy.deepcopy(turbine_definition_cache[t]) for t in _turbine_types
+        ]
 
     @layout_x.validator
     def check_x(self, attribute: attrs.Attribute, value: Any) -> None:
         if len(value) != len(self.layout_y):
             raise ValueError("layout_x and layout_y must have the same number of entries.")
 
     @layout_y.validator
     def check_y(self, attribute: attrs.Attribute, value: Any) -> None:
         if len(value) != len(self.layout_x):
             raise ValueError("layout_x and layout_y must have the same number of entries.")
 
+    @turbine_type.validator
+    def check_turbine_type(self, attribute: attrs.Attribute, value: Any) -> None:
+        # Check that the list of turbines is either of length 1 or N turbines
+        if len(value) != 1 and len(value) != self.n_turbines:
+            raise ValueError(
+                "turbine_type must have the same number of entries as layout_x/layout_y or have "
+                "a single turbine_type value."
+            )
+
     @turbine_library_path.validator
     def check_library_path(self, attribute: attrs.Attribute, value: Path) -> None:
         """Ensures that the input to `library_path` exists and is a directory."""
         if not value.is_dir():
             raise FileExistsError(f"The input file path: {str(value)} is not a valid directory.")
 
-    def check_turbine_type(self) -> None:
-        if len(self.turbine_type) != len(self.layout_x):
-            if len(self.turbine_type) == 1:
-                self.turbine_type *= len(self.layout_x)
-            elif np.unique(self.turbine_type).size == 1:
-                self.turbine_type = [self.turbine_type[0]] * len(self.layout_x)
-            else:
-                raise ValueError(
-                    "turbine_type must have the same number of entries as layout_x/layout_y or have"
-                    " a single turbine_type value."
-                )
-
-        # If the user specified the default location, do not check against duplicated definitions
-        turbine_map = {}
-        unique_turbines = [
-            yaml.safe_load(el_j)
-            for el_j in {yaml.dump(el_i, default_flow_style=False)
-            for el_i in self.turbine_type}
-        ]
-        for turbine in unique_turbines:
-
-            # If the passed data are already turbine dictionaries, skip the file loading
-            if isinstance(turbine, str):
-                # Check if the file exists in the internal and/or external libary
-                internal_fn = (default_turbine_library_path / turbine).with_suffix(".yaml")
-                external_fn = (self.turbine_library_path / turbine).with_suffix(".yaml")
-                in_internal = internal_fn.exists()
-                in_external = external_fn.exists()
-
-                # If an external library is used, and the file is a duplicate with what already
-                # exists, then raise an error
-                is_separate_path = self.turbine_library_path != default_turbine_library_path
-                if is_separate_path and in_external and in_internal:
-                    raise ValueError(
-                        f"The turbine type: {turbine} exists in both the internal and external"
-                        " turbine library."
-                    )
-                if in_internal:
-                    full_path = internal_fn
-                elif in_external:
-                    full_path = external_fn
-                else:
-                    raise ValueError(
-                        f"The turbine type: {turbine} exists in both the internal and external"
-                        " turbine library."
-                    )
-                turbine_map[turbine] = turbine = load_yaml(full_path)
-            elif isinstance(turbine, dict):
-                turbine_map[turbine["turbine_type"]] = turbine
-                full_path = turbine["turbine_type"]
-
-            # Log a warning if the reference air density doesn't exist
-            if "ref_density_cp_ct" not in turbine:
-                self.logger.warning(
-                    f"The value ref_density_cp_ct is not defined in the file {full_path}."
-                    "This value is not the simulated air density but is the density "
-                    "at which the cp/ct curves are defined. In previous versions, this "
-                    "was assumed to be 1.225. Future versions of FLORIS will give an error "
-                    "if this value is not explicitly defined. Currently, this value is "
-                    "being set to the prior default value of 1.225."
-                )
-                turbine['ref_density_cp_ct'] = 1.225
-                turbine_map[turbine["turbine_type"]] = turbine
-
-        self.turbine_definitions = [
-            copy.deepcopy(turbine_map[el]) if isinstance(el, str)
-            else copy.deepcopy(turbine_map[el["turbine_type"]])
-            for el in self.turbine_type
-        ]
-
     def initialize(self, sorted_indices):
         # Sort yaw angles from most upstream to most downstream wind turbine
         self.yaw_angles_sorted = np.take_along_axis(
             self.yaw_angles,
             sorted_indices[:, :, :, 0, 0],
             axis=2,
         )
+        self.tilt_angles_sorted = np.take_along_axis(
+            self.tilt_angles,
+            sorted_indices[:, :, :, 0, 0],
+            axis=2,
+        )
         self.state = State.INITIALIZED
 
     def construct_hub_heights(self):
         self.hub_heights = np.array([turb['hub_height'] for turb in self.turbine_definitions])
 
     def construct_rotor_diameters(self):
         self.rotor_diameters = np.array([
             turb['rotor_diameter'] for turb in self.turbine_definitions
         ])
 
     def construct_turbine_TSRs(self):
         self.TSRs = np.array([turb['TSR'] for turb in self.turbine_definitions])
 
-    def construc_turbine_pPs(self):
+    def construct_turbine_pPs(self):
         self.pPs = np.array([turb['pP'] for turb in self.turbine_definitions])
 
-    def construc_turbine_ref_density_cp_cts(self):
+    def construct_turbine_pTs(self):
+        self.pTs = np.array([turb['pT'] for turb in self.turbine_definitions])
+
+    def construct_turbine_ref_density_cp_cts(self):
         self.ref_density_cp_cts = np.array([
             turb['ref_density_cp_ct'] for turb in self.turbine_definitions
         ])
 
+    def construct_turbine_ref_tilt_cp_cts(self):
+        self.ref_tilt_cp_cts = np.array(
+            [turb['ref_tilt_cp_ct'] for turb in self.turbine_definitions]
+        )
+
+    def construct_turbine_correct_cp_ct_for_tilt(self):
+        self.correct_cp_ct_for_tilt = np.array(
+            [turb.correct_cp_ct_for_tilt for turb in self.turbine_map]
+        )
+
     def construct_turbine_map(self):
         self.turbine_map = [Turbine.from_dict(turb) for turb in self.turbine_definitions]
 
     def construct_turbine_fCts(self):
-        self.turbine_fCts = [(turb.turbine_type, turb.fCt_interp) for turb in self.turbine_map]
+        self.turbine_fCts = {
+            turb.turbine_type: turb.fCt_interp for turb in self.turbine_map
+        }
 
-    def construct_turbine_fCps(self):
-        self.turbine_fCps = [(turb.turbine_type, turb.fCp_interp) for turb in self.turbine_map]
+    def construct_turbine_fTilts(self):
+        self.turbine_fTilts = [(turb.turbine_type, turb.fTilt_interp) for turb in self.turbine_map]
 
     def construct_turbine_power_interps(self):
-        self.turbine_power_interps = [
-            (turb.turbine_type, turb.power_interp) for turb in self.turbine_map
-        ]
+        self.turbine_power_interps = {
+            turb.turbine_type: turb.power_interp for turb in self.turbine_map
+        }
 
     def construct_coordinates(self):
         self.coordinates = np.array([
             Vec3([x, y, z]) for x, y, z in zip(self.layout_x, self.layout_y, self.hub_heights)
         ])
 
     def expand_farm_properties(
@@ -225,19 +272,44 @@
             axis=2
         )
         self.TSRs_sorted = np.take_along_axis(
             self.TSRs * template_shape,
             sorted_coord_indices,
             axis=2
         )
+        self.ref_density_cp_cts_sorted = np.take_along_axis(
+            self.ref_density_cp_cts * template_shape,
+            sorted_coord_indices,
+            axis=2
+        )
+        self.ref_tilt_cp_cts_sorted = np.take_along_axis(
+            self.ref_tilt_cp_cts * template_shape,
+            sorted_coord_indices,
+            axis=2
+        )
+        self.correct_cp_ct_for_tilt_sorted = np.take_along_axis(
+            self.correct_cp_ct_for_tilt * template_shape,
+            sorted_coord_indices,
+            axis=2
+        )
         self.pPs_sorted = np.take_along_axis(
             self.pPs * template_shape,
             sorted_coord_indices,
             axis=2
         )
+        self.pTs_sorted = np.take_along_axis(
+            self.pTs * template_shape,
+            sorted_coord_indices,
+            axis=2
+        )
+        self.tilt_angles_sorted = np.take_along_axis(
+            self.tilt_angles * template_shape,
+            sorted_coord_indices,
+            axis=2
+        )
         self.turbine_type_names_sorted = [turb["turbine_type"] for turb in self.turbine_definitions]
         self.turbine_type_map_sorted = np.take_along_axis(
             np.reshape(
                 self.turbine_type_names_sorted * n_wind_directions,
                 np.shape(sorted_coord_indices)
             ),
             sorted_coord_indices,
@@ -245,20 +317,44 @@
         )
 
     def set_yaw_angles(self, n_wind_directions: int, n_wind_speeds: int):
         # TODO Is this just for initializing yaw angles to zero?
         self.yaw_angles = np.zeros((n_wind_directions, n_wind_speeds, self.n_turbines))
         self.yaw_angles_sorted = np.zeros((n_wind_directions, n_wind_speeds, self.n_turbines))
 
+    def set_tilt_to_ref_tilt(self, n_wind_directions: int, n_wind_speeds: int):
+        self.tilt_angles = (
+            np.ones((n_wind_directions, n_wind_speeds, self.n_turbines))
+            * self.ref_tilt_cp_cts
+        )
+        self.tilt_angles_sorted = (
+            np.ones((n_wind_directions, n_wind_speeds, self.n_turbines))
+            * self.ref_tilt_cp_cts
+        )
+
+    def calculate_tilt_for_eff_velocities(self, rotor_effective_velocities):
+        tilt_angles = compute_tilt_angles_for_floating_turbines(
+            self.turbine_type_map_sorted,
+            self.tilt_angles_sorted,
+            self.turbine_fTilts,
+            rotor_effective_velocities,
+        )
+        return tilt_angles
+
     def finalize(self, unsorted_indices):
         self.yaw_angles = np.take_along_axis(
             self.yaw_angles_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
+        self.tilt_angles = np.take_along_axis(
+            self.tilt_angles_sorted,
+            unsorted_indices[:,:,:,0,0],
+            axis=2
+        )
         self.hub_heights = np.take_along_axis(
             self.hub_heights_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
         self.rotor_diameters = np.take_along_axis(
             self.rotor_diameters_sorted,
@@ -271,14 +367,19 @@
             axis=2
         )
         self.pPs = np.take_along_axis(
             self.pPs_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
+        self.pTs = np.take_along_axis(
+            self.pTs_sorted,
+            unsorted_indices[:,:,:,0,0],
+            axis=2
+        )
         self.turbine_type_map = np.take_along_axis(
             self.turbine_type_map_sorted,
             unsorted_indices[:,:,:,0,0],
             axis=2
         )
         self.state.USED
```

### Comparing `FLORIS-3.3/floris/simulation/floris.py` & `FLORIS-3.4/floris/simulation/floris.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,34 +10,37 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
-import json
 from pathlib import Path
 
 import yaml
 from attrs import define, field
 
-import floris.logging_manager as logging_manager
+from floris import logging_manager
 from floris.simulation import (
     BaseClass,
     cc_solver,
+    empirical_gauss_solver,
     Farm,
     FlowField,
     FlowFieldGrid,
     FlowFieldPlanarGrid,
     full_flow_cc_solver,
+    full_flow_empirical_gauss_solver,
     full_flow_sequential_solver,
     full_flow_turbopark_solver,
     Grid,
+    PointsGrid,
     sequential_solver,
     State,
+    TurbineCubatureGrid,
     TurbineGrid,
     turbopark_solver,
     WakeModelManager,
 )
 from floris.utilities import load_yaml
 
 
@@ -61,36 +64,54 @@
     description: str = field(converter=str)
     floris_version: str = field(converter=str)
 
     grid: Grid = field(init=False)
 
     def __attrs_post_init__(self) -> None:
 
+        self.check_deprecated_inputs()
+
         # Initialize farm quanitities that depend on other objects
         self.farm.construct_turbine_map()
         self.farm.construct_turbine_fCts()
-        self.farm.construct_turbine_fCps()
         self.farm.construct_turbine_power_interps()
         self.farm.construct_hub_heights()
         self.farm.construct_rotor_diameters()
         self.farm.construct_turbine_TSRs()
-        self.farm.construc_turbine_pPs()
-        self.farm.construc_turbine_ref_density_cp_cts()
+        self.farm.construct_turbine_pPs()
+        self.farm.construct_turbine_pTs()
+        self.farm.construct_turbine_ref_density_cp_cts()
+        self.farm.construct_turbine_ref_tilt_cp_cts()
+        self.farm.construct_turbine_fTilts()
+        self.farm.construct_turbine_correct_cp_ct_for_tilt()
         self.farm.construct_coordinates()
         self.farm.set_yaw_angles(self.flow_field.n_wind_directions, self.flow_field.n_wind_speeds)
+        self.farm.set_tilt_to_ref_tilt(
+            self.flow_field.n_wind_directions,
+            self.flow_field.n_wind_speeds,
+        )
 
         if self.solver["type"] == "turbine_grid":
             self.grid = TurbineGrid(
                 turbine_coordinates=self.farm.coordinates,
                 reference_turbine_diameter=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["turbine_grid_points"],
                 time_series=self.flow_field.time_series,
             )
+        elif self.solver["type"] == "turbine_cubature_grid":
+            self.grid = TurbineCubatureGrid(
+                turbine_coordinates=self.farm.coordinates,
+                reference_turbine_diameter=self.farm.rotor_diameters,
+                wind_directions=self.flow_field.wind_directions,
+                wind_speeds=self.flow_field.wind_speeds,
+                time_series=self.flow_field.time_series,
+                grid_resolution=self.solver["turbine_grid_points"],
+            )
         elif self.solver["type"] == "flow_field_grid":
             self.grid = FlowFieldGrid(
                 turbine_coordinates=self.farm.coordinates,
                 reference_turbine_diameter=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 grid_resolution=self.solver["flow_field_grid_points"],
@@ -101,25 +122,26 @@
                 turbine_coordinates=self.farm.coordinates,
                 reference_turbine_diameter=self.farm.rotor_diameters,
                 wind_directions=self.flow_field.wind_directions,
                 wind_speeds=self.flow_field.wind_speeds,
                 normal_vector=self.solver["normal_vector"],
                 planar_coordinate=self.solver["planar_coordinate"],
                 grid_resolution=self.solver["flow_field_grid_points"],
+                time_series=self.flow_field.time_series,
                 x1_bounds=self.solver["flow_field_bounds"][0],
                 x2_bounds=self.solver["flow_field_bounds"][1],
-                time_series=self.flow_field.time_series,
             )
         else:
             raise ValueError(
-                f"Supported solver types are [turbine_grid, flow_field_grid],"
-                f" but type given was {self.solver['type']}"
+                "Supported solver types are "
+                "[turbine_grid, turbine_cubature_grid, flow_field_grid, flow_field_planar_grid], "
+                f"but type given was {self.solver['type']}"
             )
 
-        if type(self.grid) == TurbineGrid:
+        if isinstance(self.grid, (TurbineGrid, TurbineCubatureGrid)):
             self.farm.expand_farm_properties(
                 self.flow_field.n_wind_directions,
                 self.flow_field.n_wind_speeds,
                 self.grid.sorted_coord_indices
             )
 
         # Configure logging
@@ -128,14 +150,51 @@
             self.logging["console"]["level"],
         )
         logging_manager.configure_file_log(
             self.logging["file"]["enable"],
             self.logging["file"]["level"],
         )
 
+    def check_deprecated_inputs(self):
+        """
+        This function should used when the FLORIS input file changes in order to provide
+        an informative error and suggest a fix.
+        """
+
+        error_messages = []
+        # Check for missing values add in version 3.2 and 3.4
+        for turbine in self.farm.turbine_definitions:
+
+            if "ref_density_cp_ct" not in turbine.keys():
+                error_messages.append(
+                    "From FLORIS v3.2, the turbine definition must include 'ref_density_cp_ct'. "
+                    "This value represents the air density at which the provided Cp and Ct "
+                    "curves are defined. Previously, this was assumed to be 1.225 kg/m^3, "
+                    "and other air density values applied were assumed to be a deviation "
+                    "from the defined level. FLORIS now requires the user to explicitly "
+                    "define the reference density. Add 'ref_density_cp_ct' to your "
+                    "turbine definition and try again. For a description of the turbine inputs, "
+                    "see https://nrel.github.io/floris/input_reference_turbine.html."
+                )
+
+            if "ref_tilt_cp_ct" not in turbine.keys():
+                error_messages.append(
+                    "From FLORIS v3.4, the turbine definition must include 'ref_tilt_cp_ct'. "
+                    "This value represents the tilt angle at which the provided Cp and Ct "
+                    "curves are defined. Add 'ref_tilt_cp_ct' to your turbine definition and "
+                    "try again. For a description of the turbine inputs, "
+                    "see https://nrel.github.io/floris/input_reference_turbine.html."
+                )
+
+            if len(error_messages) > 0:
+                raise ValueError(
+                    f"{turbine['turbine_type']} turbine model\n" +
+                    "\n\n".join(error_messages)
+                )
+
     # @profile
     def initialize_domain(self):
         """Initialize solution space prior to wake calculations"""
 
         # Initialize field quanitities; doing this immediately prior to doing
         # the calculation step allows for manipulating inputs in a script
         # without changing the data structures
@@ -151,40 +210,55 @@
         initialize_domain() is required to be called before this function."""
 
         vel_model = self.wake.model_strings["velocity_model"]
 
         # <<interface>>
         # start = time.time()
 
+        if vel_model in ["gauss", "cc", "turbopark", "jensen"] and \
+            self.farm.correct_cp_ct_for_tilt.any():
+            self.logger.warn(
+                "The current model does not account for vertical wake deflection due to " +
+                "tilt. Corrections to Cp and Ct can be included, but no vertical wake " +
+                "deflection will occur."
+            )
+
         if vel_model=="cc":
-            elapsed_time = cc_solver(
+            cc_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
         elif vel_model=="turbopark":
-            elapsed_time = turbopark_solver(
+            turbopark_solver(
+                self.farm,
+                self.flow_field,
+                self.grid,
+                self.wake
+            )
+        elif vel_model=="empirical_gauss":
+            empirical_gauss_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
         else:
-            elapsed_time = sequential_solver(
+            sequential_solver(
                 self.farm,
                 self.flow_field,
                 self.grid,
                 self.wake
             )
         # end = time.time()
         # elapsed_time = end - start
 
         self.finalize()
-        return elapsed_time
+        # return elapsed_time
 
     def solve_for_viz(self):
         # Do the calculation with the TurbineGrid for a single wind speed
         # and wind direction and 1 point on the grid. Then, use the result
         # to construct the full flow field grid.
         # This function call should be for a single wind direction and wind speed
         # since the memory consumption is very large.
@@ -193,65 +267,86 @@
 
         vel_model = self.wake.model_strings["velocity_model"]
 
         if vel_model=="cc":
             full_flow_cc_solver(self.farm, self.flow_field, self.grid, self.wake)
         elif vel_model=="turbopark":
             full_flow_turbopark_solver(self.farm, self.flow_field, self.grid, self.wake)
+        elif vel_model=="empirical_gauss":
+            full_flow_empirical_gauss_solver(self.farm, self.flow_field, self.grid, self.wake)
         else:
             full_flow_sequential_solver(self.farm, self.flow_field, self.grid, self.wake)
 
+    def solve_for_points(self, x, y, z):
+        # Do the calculation with the TurbineGrid for a single wind speed
+        # and wind direction and a 3x3 rotor grid. Then, use the result
+        # to construct the full flow field grid.
+        # This function call should be for a single wind direction and wind speed
+        # since the memory consumption is very large.
+
+        # Instantiate the flow_grid
+        field_grid = PointsGrid(
+            points_x=x,
+            points_y=y,
+            points_z=z,
+            turbine_coordinates=self.farm.coordinates,
+            reference_turbine_diameter=self.farm.rotor_diameters,
+            wind_directions=self.flow_field.wind_directions,
+            wind_speeds=self.flow_field.wind_speeds,
+            grid_resolution=1,
+            time_series=self.flow_field.time_series,
+            x_center_of_rotation=self.grid.x_center_of_rotation,
+            y_center_of_rotation=self.grid.y_center_of_rotation
+        )
+
+        self.flow_field.initialize_velocity_field(field_grid)
+
+        vel_model = self.wake.model_strings["velocity_model"]
+
+        if vel_model == "cc" or vel_model == "turbopark":
+            raise NotImplementedError(
+                "solve_for_points is currently only available with the "+\
+                "gauss, jensen, and empirical_guass models."
+            )
+        elif vel_model == "empirical_gauss":
+            full_flow_empirical_gauss_solver(self.farm, self.flow_field, field_grid, self.wake)
+        else:
+            full_flow_sequential_solver(self.farm, self.flow_field, field_grid, self.wake)
+
+        return self.flow_field.u_sorted[:,:,:,0,0] # Remove turbine grid dimensions
+
     def finalize(self):
         # Once the wake calculation is finished, unsort the values to match
         # the user-supplied order of things.
         self.flow_field.finalize(self.grid.unsorted_indices)
         self.farm.finalize(self.grid.unsorted_indices)
         self.state = State.USED
 
     ## I/O
 
     @classmethod
-    def from_file(cls, input_file_path: str | Path, filetype: str = None) -> Floris:
-        """Creates a `Floris` instance from an input file. Must be filetype
-        JSON or YAML.
+    def from_file(cls, input_file_path: str | Path) -> Floris:
+        """Creates a `Floris` instance from an input file. Must be filetype YAML.
 
         Args:
             input_file_path (str): The relative or absolute file path and name to the
                 input file.
-            filetype (str): The type to export: [YAML | JSON]
 
         Returns:
             Floris: The class object instance.
         """
-        input_file_path = Path(input_file_path).resolve()
-        if filetype is None:
-            filetype = input_file_path.suffix.strip(".")
-
-        with open(input_file_path) as input_file:
-            if filetype.lower() in ("yml", "yaml"):
-                input_dict = load_yaml(input_file_path)
-            elif filetype.lower() == "json":
-                input_dict = json.load(input_file)
-
-                # TODO: This is a temporary hack to put the turbine definition into the farm.
-                # Long term, we need a strategy for handling this. The YAML file format supports
-                # pointers to other data, for example.
-                # input_dict["farm"]["turbine"] = input_dict["turbine"]
-                # input_dict.pop("turbine")
-            else:
-                raise ValueError("Supported import filetypes are JSON and YAML")
+        input_dict = load_yaml(Path(input_file_path).resolve())
         return Floris.from_dict(input_dict)
 
-    def to_file(self, output_file_path: str, filetype: str="YAML") -> None:
-        """Converts the `Floris` object to an input-ready JSON or YAML file at `output_file_path`.
+    def to_file(self, output_file_path: str) -> None:
+        """Converts the `Floris` object to an input-ready YAML file at `output_file_path`.
 
         Args:
             output_file_path (str): The full path and filename for where to save the file.
-            filetype (str): The type to export: [YAML | JSON]
         """
         with open(output_file_path, "w+") as f:
-            if filetype.lower() == "yaml":
-                yaml.dump(self.as_dict(), f, default_flow_style=False)
-            elif filetype.lower() == "json":
-                json.dump(self.as_dict(), f, indent=2, sort_keys=False)
-            else:
-                raise ValueError("Supported export filetypes are JSON and YAML")
+            yaml.dump(
+                self.as_dict(),
+                f,
+                sort_keys=False,
+                default_flow_style=False
+            )
```

### Comparing `FLORIS-3.3/floris/simulation/grid.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,462 +8,495 @@
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
-
-from __future__ import annotations
-
-from abc import ABC, abstractmethod
-from typing import Iterable
-
-import attrs
+import matplotlib.pyplot as plt
 import numpy as np
-from attrs import define, field
+from scipy.optimize import minimize
 
-from floris.type_dec import (
-    floris_array_converter,
-    floris_float_type,
-    NDArrayFloat,
-    NDArrayInt,
-)
-from floris.utilities import rotate_coordinates_rel_west, Vec3
+from .layout import LayoutOptimization
 
 
-@define
-class Grid(ABC):
+class PowerDensityOptimization(LayoutOptimization):
     """
-    Grid should establish domain bounds based on given criteria,
-    and develop three arrays to contain components of the grid
-    locations in space.
-
-    This could be generalized to any number of dimensions to be
-    used by perhaps a turbulence field.
-
-    The grid will have to be reestablished for each wind direction since the planform
-    area of the farm will be different.
-
-    x are the locations in space in the primary direction (typically the direction of the wind)
-    y are the locations in space in the lateral direction
-    z are the locations in space in the vertical direction
-    u are the velocity components at each point in space
-    v are the velocity components at each point in space
-    w are the velocity components at each point in space
-    all of these arrays are the same size
-
-    Args:
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int` | :py:obj:`Iterable(int,)`): Grid resolution specific
-            to each grid type.
-        wind_directions (:py:obj:`NDArrayFloat`): Wind directions supplied by the user.
-        wind_speeds (:py:obj:`NDArrayFloat`): Wind speeds supplied by the user.
-        time_series (:py:obj:`bool`): True/false flag to indicate whether the supplied wind
-            data is a time series.
+    PowerDensityOptimization is a subclass of the
+    :py:class:`~.tools.optimization.scipy.layout.LayoutOptimization` class
+    that performs power density optimization.
     """
-    turbine_coordinates: list[Vec3] = field()
-    reference_turbine_diameter: float
-    grid_resolution: int | Iterable = field()
-    wind_directions: NDArrayFloat = field(converter=floris_array_converter)
-    wind_speeds: NDArrayFloat = field(converter=floris_array_converter)
-    time_series: bool = field()
-
-    n_turbines: int = field(init=False)
-    n_wind_speeds: int = field(init=False)
-    n_wind_directions: int = field(init=False)
-    turbine_coordinates_array: NDArrayFloat = field(init=False)
-    x: NDArrayFloat = field(init=False, default=[])
-    y: NDArrayFloat = field(init=False, default=[])
-    z: NDArrayFloat = field(init=False, default=[])
-    x_sorted: NDArrayFloat = field(init=False)
-    y_sorted: NDArrayFloat = field(init=False)
-    z_sorted: NDArrayFloat = field(init=False)
-
-    def __attrs_post_init__(self) -> None:
-        self.turbine_coordinates_array = np.array([c.elements for c in self.turbine_coordinates])
-
-    @turbine_coordinates.validator
-    def check_coordinates(self, instance: attrs.Attribute, value: list[Vec3]) -> None:
-        """
-        Ensures all elements are `Vec3` objects and keeps the `n_turbines`
-        attribute up to date.
-        """
-        types = np.unique([isinstance(c, Vec3) for c in value])
-        if not all(types):
-            raise TypeError("'turbine_coordinates' must be `Vec3` objects.")
-
-        self.n_turbines = len(value)
-
-    @wind_speeds.validator
-    def wind_speeds_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_speeds` attribute up to date."""
-        if self.time_series:
-            self.n_wind_speeds = 1
-        else:
-            self.n_wind_speeds = value.size
 
-    @wind_directions.validator
-    def wind_directions_validator(self, instance: attrs.Attribute, value: NDArrayFloat) -> None:
-        """Using the validator method to keep the `n_wind_directions` attribute up to date."""
-        self.n_wind_directions = value.size
-
-    @grid_resolution.validator
-    def grid_resolution_validator(self, instance: attrs.Attribute, value: int | Iterable) -> None:
-        # TODO move this to the grid types and off of the base class
-        """Check that grid resolution is given as int or Vec3 with int components."""
-        if isinstance(value, int) and type(self) is TurbineGrid:
-            return
-        elif isinstance(value, Iterable) and type(self) is FlowFieldPlanarGrid:
-            assert type(value[0]) is int
-            assert type(value[1]) is int
-        elif isinstance(value, Iterable) and type(self) is FlowFieldGrid:
-            assert type(value[0]) is int
-            assert type(value[1]) is int
-            assert type(value[2]) is int
-        else:
-            raise TypeError("`grid_resolution` must be of type int or Iterable(int,)")
+    def __init__(
+        self,
+        fi,
+        boundaries,
+        wd,
+        ws,
+        freq,
+        AEP_initial,
+        yawbnds=None,
+        x0=None,
+        bnds=None,
+        min_dist=None,
+        opt_method="SLSQP",
+        opt_options=None,
+    ):
+        """
+        Instantiate PowerDensityOptimization object with a FlorisInterface
+        object and assigns parameter values.
 
-    @abstractmethod
-    def set_grid(self) -> None:
-        raise NotImplementedError("Grid.set_grid")
-
-@define
-class TurbineGrid(Grid):
-    """See `Grid` for more details.
-
-    Args:
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        wind_directions (`list[float]`): The input wind directions
-        wind_speeds (`list[float]`): The input wind speeds
-        grid_resolution (:py:obj:`int`): The number of points on each turbine
-    """
-    # TODO: describe these and the differences between `sorted_indices` and `sorted_coord_indices`
-    sorted_indices: NDArrayInt = field(init=False)
-    sorted_coord_indices: NDArrayInt = field(init=False)
-    unsorted_indices: NDArrayInt = field(init=False)
-
-    def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
-        self.set_grid()
-
-    def set_grid(self) -> None:
-        """
-        Create grid points at each turbine for each wind direction and wind speed in the simulation.
-        This creates the underlying data structure for the calculation.
-
-        arrays have shape
-        (n wind directions, n wind speeds, n turbines, m grid spanwise, m grid vertically)
-        - dimension 1: each wind direction
-        - dimension 2: each wind speed
-        - dimension 3: each turbine
-        - dimension 4: number of points in the spanwise direction (ngrid)
-        - dimension 5: number of points in the vertical dimension (ngrid)
-
-        For example
-        - x is [
-            n wind direction,
-            n wind speeds,
-            n turbines,
-            x-component of the points in the spanwise direction,
-            x-component of the points in the vertical direction
-        ]
-        - y is [
-            n wind direction,
-            n wind speeds,
-            n turbines,
-            y-component of the points in the spanwise direction,
-            y-component of the points in the vertical direction
-        ]
-
-        The x,y,z arrays contain the actual locations in that direction.
-
-        # -   **self.grid_resolution** (*int*, optional): The square root of the number
-        #             of points to use on the turbine grid. This number will be
-        #             squared so that the points can be evenly distributed.
-        #             Defaults to 5.
-
-        If the grid conforms to the sequential solver interface,
-        it must be sorted from upstream to downstream
-
-        In a y-z plane on the rotor swept area, the -2 dimension is a column of
-        points and the -1 dimension is the row number.
-        So the following line prints the 0'th column of the the 0'th turbine's grid:
-        print(grid.y_sorted[0,0,0,0,:])
-        print(grid.z_sorted[0,0,0,0,:])
-        And this line prints a single point
-        print(grid.y_sorted[0,0,0,0,0])
-        print(grid.z_sorted[0,0,0,0,0])
-        Note that the x coordinates are all the same for the rotor plane.
-
-        """
-        # TODO: Where should we locate the coordinate system? Currently, its at
-        # the foot of the turbine where the tower meets the ground.
-
-        # These are the rotated coordinates of the wind turbines based on the wind direction
-        x, y, z = rotate_coordinates_rel_west(self.wind_directions, self.turbine_coordinates_array)
-
-        # -   **rloc** (*float, optional): A value, from 0 to 1, that determines
-        #         the width/height of the grid of points on the rotor as a ratio of
-        #         the rotor radius.
-        #         Defaults to 0.5.
-
-        # Create the data for the turbine grids
-        radius_ratio = 0.5
-        disc_area_radius = radius_ratio * self.reference_turbine_diameter / 2
-        template_grid = np.ones(
-            (
-                self.n_wind_directions,
-                self.n_wind_speeds,
-                self.n_turbines,
-                self.grid_resolution,
-                self.grid_resolution,
+        Args:
+            fi (:py:class:`floris.tools.floris_interface.FlorisInterface`):
+                Interface used to interact with the Floris object.
+            boundaries (iterable(float, float)): Pairs of x- and y-coordinates
+                that represent the boundary's vertices (m).
+            wd (np.array): An array of wind directions (deg).
+            ws (np.array): An array of wind speeds (m/s).
+            freq (np.array): An array of the frequencies of occurance
+                correponding to each pair of wind direction and wind speed
+                values.
+            AEP_initial (float): The initial Annual Energy
+                Production used for normalization in the optimization (Wh)
+                (TODO: Is Watt-hours the correct unit?).
+            yawbnds: TODO: This parameter isn't used. Remove it?
+            x0 (iterable, optional): The initial turbine locations,
+                ordered by x-coordinate and then y-coordiante
+                (ie. [x1, x2, ..., xn, y1, y2, ..., yn]) (m). If none are
+                provided, x0 initializes to the current turbine locations.
+                Defaults to None.
+            bnds (iterable, optional): Bounds for the optimization
+                variables (pairs of min/max values for each variable (m)). If
+                none are specified, they are set to (0, 1) for each turbine.
+                Defaults to None. TODO: Explain significance of (0, 1).
+            min_dist (float, optional): The minimum distance to be
+                maintained between turbines during the optimization (m). If not
+                specified, initializes to 4 rotor diameters. Defaults to None.
+            opt_method (str, optional): The optimization method used by
+                scipy.optimize.minize. Defaults to 'SLSQP'.
+            opt_options (dict, optional): Optimization options used by
+                scipy.optimize.minize. If none are specified, they are set t
+                {'maxiter': 100, 'disp': True, 'iprint': 2, 'ftol': 1e-9}.
+                Defaults to None.
+        """
+        super().__init__(
+            fi,
+            boundaries,
+            wd,
+            ws,
+            freq,
+            AEP_initial,
+            x0=x0,
+            bnds=bnds,
+            min_dist=min_dist,
+            opt_method=opt_method,
+            opt_options=opt_options,
+        )
+        self.epsilon = np.finfo(float).eps
+        self.counter = 0
+
+        if opt_options is None:
+            self.opt_options = {"maxiter": 100, "disp": True, "iprint": 2, "ftol": 1e-9}
+
+    def _generate_constraints(self):
+        # grad_constraint1 = grad(self._space_constraint)
+        # grad_constraint2 = grad(self._distance_from_boundaries)
+
+        tmp1 = {
+            "type": "ineq",
+            "fun": lambda x, *args: self._space_constraint(x, self.min_dist),
+            "args": (self.min_dist,),
+        }
+        tmp2 = {
+            "type": "ineq",
+            "fun": lambda x, *args: self._distance_from_boundaries(
+                x, self.boundaries_norm
             ),
-            dtype=floris_float_type
+            "args": (self.boundaries_norm,),
+        }
+        tmp3 = {"type": "ineq", "fun": lambda x, *args: self._AEP_constraint(x)}
+
+        self.cons = [tmp1, tmp2, tmp3]
+
+    def _set_opt_bounds(self):
+        self.bnds = [
+            (0.0, 1.0) for _ in range(2 * self.nturbs + self.nturbs * len(self.wd))
+        ]
+
+    def _change_coordinates(self, locsx, locsy):
+        # Parse the layout coordinates
+        layout_array = [locsx, locsy]
+
+        # Update the turbine map in floris
+        self.fi.reinitialize_flow_field(layout_array=layout_array)
+
+    def _powDens_opt(self, optVars):
+        locsx = optVars[0 : self.nturbs]
+        locsy = optVars[self.nturbs : 2 * self.nturbs]
+
+        locsx_unnorm = [
+            self._unnorm(valx, self.bndx_min, self.bndx_max) for valx in locsx
+        ]
+        locsy_unnorm = [
+            self._unnorm(valy, self.bndy_min, self.bndy_max) for valy in locsy
+        ]
+
+        turb_controls = [
+            optVars[
+                2 * self.nturbs + i * self.nturbs : 3 * self.nturbs + i * self.nturbs
+            ]
+            for i in range(len(self.wd))
+        ]
+
+        turb_controls_unnorm = [
+            self._unnorm(yaw, self.yaw_min, self.yaw_max) for yaw in turb_controls
+        ]
+
+        self._change_coordinates(locsx_unnorm, locsy_unnorm)
+        opt_area = self.find_layout_area(locsx_unnorm + locsy_unnorm)
+
+        AEP_sum = 0.0
+
+        for i in range(len(self.wd)):
+            for j, turbine in enumerate(self.fi.floris.farm.turbine_map.turbines):
+                turbine.yaw_angle = turb_controls_unnorm[i][j]
+
+            AEP_sum = AEP_sum + self._AEP_single_wd(
+                self.wd[i], self.ws[i], self.freq[i]
+            )
+
+        # print('AEP ratio: ', AEP_sum/self.AEP_initial)
+
+        return -1 * AEP_sum / self.AEP_initial * self.initial_area / opt_area
+
+    def _AEP_constraint(self, optVars):
+        locsx = optVars[0 : self.nturbs]
+        locsy = optVars[self.nturbs : 2 * self.nturbs]
+
+        locsx_unnorm = [
+            self._unnorm(valx, self.bndx_min, self.bndx_max) for valx in locsx
+        ]
+        locsy_unnorm = [
+            self._unnorm(valy, self.bndy_min, self.bndy_max) for valy in locsy
+        ]
+
+        turb_controls = [
+            optVars[
+                2 * self.nturbs + i * self.nturbs : 3 * self.nturbs + i * self.nturbs
+            ]
+            for i in range(len(self.wd))
+        ]
+
+        turb_controls_unnorm = [
+            self._unnorm(yaw, self.yaw_min, self.yaw_max) for yaw in turb_controls
+        ]
+
+        self._change_coordinates(locsx_unnorm, locsy_unnorm)
+
+        AEP_sum = 0.0
+
+        for i in range(len(self.wd)):
+            for j, turbine in enumerate(self.fi.floris.farm.turbine_map.turbines):
+                turbine.yaw_angle = turb_controls_unnorm[i][j]
+
+            AEP_sum = AEP_sum + self._AEP_single_wd(
+                self.wd[i], self.ws[i], self.freq[i]
+            )
+
+        return AEP_sum / self.AEP_initial - 1.0
+
+    def _optimize(self):
+        self.residual_plant = minimize(
+            self._powDens_opt,
+            self.x0,
+            method=self.opt_method,
+            bounds=self.bnds,
+            constraints=self.cons,
+            options=self.opt_options,
         )
-        # Calculate the radial distance from the center of the turbine rotor.
-        # If a grid resolution of 1 is selected, create a disc_grid of zeros, as
-        # np.linspace would just return the starting value of -1 * disc_area_radius
-        # which would place the point below the center of the rotor.
-        if self.grid_resolution == 1:
-            disc_grid = np.zeros((np.shape(disc_area_radius)[0], 1 ))
+
+        opt_results = self.residual_plant.x
+
+        return opt_results
+
+    def optimize(self):
+        """
+        This method finds the optimized layout of wind turbines for power
+        production given the provided frequencies of occurance of wind
+        conditions (wind speed, direction).
+
+        TODO: update the doc
+
+        Returns:
+            iterable: A list of the optimized x, y locations of each
+            turbine (m).
+        """
+        print("=====================================================")
+        print("Optimizing turbine layout...")
+        print("Number of parameters to optimize = ", len(self.x0))
+        print("=====================================================")
+
+        opt_locs_norm = self._optimize()
+
+        print("Optimization complete.")
+
+        opt_locs = [
+            [
+                self._unnorm(valx, self.bndx_min, self.bndx_max)
+                for valx in opt_locs_norm[0 : self.nturbs]
+            ],
+            [
+                self._unnorm(valy, self.bndy_min, self.bndy_max)
+                for valy in opt_locs_norm[self.nturbs : 2 * self.nturbs]
+            ],
+        ]
+
+        return opt_locs
+
+    def reinitialize_opt(
+        self,
+        boundaries=None,
+        yawbnds=None,
+        wd=None,
+        ws=None,
+        freq=None,
+        AEP_initial=None,
+        x0=None,
+        bnds=None,
+        min_dist=None,
+        opt_method=None,
+        opt_options=None,
+    ):
+        """
+        This method reinitializes any optimization parameters that are
+        specified. Otherwise, the current parameter values are kept.
+
+        Args:
+            boundaries (iterable(float, float)): Pairs of x- and y-coordinates
+                that represent the boundary's vertices (m).
+            yawbnds (iterable): A list of the min. and max. yaw offset that is
+                allowed during the optimization (deg). If none are specified,
+                initialized to (0, 25.0). Defaults to None.
+            wd (np.array): An array of wind directions (deg). Defaults to None.
+            ws (np.array): An array of wind speeds (m/s). Defaults to None.
+            freq (np.array): An array of the frequencies of occurance
+                correponding to each pair of wind direction and wind speed
+                values. Defaults to None.
+            AEP_initial (float): The initial Annual Energy
+                Production used for normalization in the optimization (Wh)
+                (TODO: Is Watt-hours the correct unit?). If not specified,
+                initializes to the AEP of the current Floris object. Defaults
+                to None.
+            x0 (iterable, optional): The initial turbine locations,
+                ordered by x-coordinate and then y-coordiante
+                (ie. [x1, x2, ..., xn, y1, y2, ..., yn]) (m). If none are
+                provided, x0 initializes to the current turbine locations.
+                Defaults to None.
+            bnds (iterable, optional): Bounds for the optimization
+                variables (pairs of min/max values for each variable (m)). If
+                none are specified, they are set to (0, 1) for each turbine.
+                Defaults to None.
+            min_dist (float, optional): The minimum distance to be
+                maintained between turbines during the optimization (m). If not
+                specified, initializes to 4 rotor diameters. Defaults to None.
+            opt_method (str, optional): The optimization method used by
+                scipy.optimize.minize. Defaults to None.
+            opt_options (dict, optional): Optimization options used by
+                scipy.optimize.minize. Defaults to None.
+        """
+        if boundaries is not None:
+            self.boundaries = boundaries
+            self.bndx_min = np.min([val[0] for val in boundaries])
+            self.bndy_min = np.min([val[1] for val in boundaries])
+            self.bndx_max = np.max([val[0] for val in boundaries])
+            self.bndy_max = np.max([val[1] for val in boundaries])
+            self.boundaries_norm = [
+                [
+                    self._norm(val[0], self.bndx_min, self.bndx_max),
+                    self._norm(val[1], self.bndy_min, self.bndy_max),
+                ]
+                for val in self.boundaries
+            ]
+        if yawbnds is not None:
+            self.yaw_min = yawbnds[0]
+            self.yaw_max = yawbnds[1]
+        else:
+            self.yaw_min = 0.0
+            self.yaw_max = 25.0
+        if wd is not None:
+            self.wd = wd
+        if ws is not None:
+            self.ws = ws
+        if freq is not None:
+            self.freq = freq
+        if AEP_initial is not None:
+            self.AEP_initial = AEP_initial
         else:
-            disc_grid = np.linspace(
-                -1 * disc_area_radius,
-                disc_area_radius,
-                self.grid_resolution,
-                dtype=floris_float_type,
-                axis=1
+            self.AEP_initial = self.fi.get_farm_AEP(self.wd, self.ws, self.freq)
+        if x0 is not None:
+            self.x0 = x0
+        else:
+            self.x0 = (
+                [
+                    self._norm(coord.x1, self.bndx_min, self.bndx_max)
+                    for coord in self.fi.floris.farm.turbine_map.coords
+                ]
+                + [
+                    self._norm(coord.x2, self.bndy_min, self.bndy_max)
+                    for coord in self.fi.floris.farm.turbine_map.coords
+                ]
+                + [self._norm(5.0, self.yaw_min, self.yaw_max)]
+                * len(self.wd)
+                * self.nturbs
             )
-        # Construct the turbine grids
-        # Here, they are already rotated to the correct orientation for each wind direction
-        _x = x[:, :, :, None, None] * template_grid
-
-        ones_grid = np.ones(
-            (self.n_turbines, self.grid_resolution, self.grid_resolution),
-            dtype=floris_float_type
+        if bnds is not None:
+            self.bnds = bnds
+        else:
+            self._set_opt_bounds()
+        if min_dist is not None:
+            self.min_dist = min_dist
+        else:
+            self.min_dist = 4 * self.fi.floris.farm.turbines[0].rotor_diameter
+        if opt_method is not None:
+            self.opt_method = opt_method
+        if opt_options is not None:
+            self.opt_options = opt_options
+
+        self.layout_x_orig = [
+            coord.x1 for coord in self.fi.floris.farm.turbine_map.coords
+        ]
+        self.layout_y_orig = [
+            coord.x2 for coord in self.fi.floris.farm.turbine_map.coords
+        ]
+
+        self._generate_constraints()
+
+        self.initial_area = self.find_layout_area(
+            self.layout_x_orig + self.layout_y_orig
         )
-        _y = y[:, :, :, None, None] + template_grid * ( disc_grid[None, None, :, :, None])
-        _z = z[:, :, :, None, None] + template_grid * ( disc_grid[:, None, :] * ones_grid )
 
-        # Sort the turbines at each wind direction
+    def find_layout_area(self, locs):
+        """
+        This method returns the area occupied by the wind farm.
 
-        # Get the sorted indices for the x coordinates. These are the indices
-        # to sort the turbines from upstream to downstream for all wind directions.
-        # Also, store the indices to sort them back for when the calculation finishes.
-        self.sorted_indices = _x.argsort(axis=2)
-        self.sorted_coord_indices = x.argsort(axis=2)
-        self.unsorted_indices = self.sorted_indices.argsort(axis=2)
-
-        # Put the turbines into the final arrays in their sorted order
-        self.x_sorted = np.take_along_axis(_x, self.sorted_indices, axis=2)
-        self.y_sorted = np.take_along_axis(_y, self.sorted_indices, axis=2)
-        self.z_sorted = np.take_along_axis(_z, self.sorted_indices, axis=2)
-
-        self.x = np.take_along_axis(self.x_sorted, self.unsorted_indices, axis=2)
-        self.y = np.take_along_axis(self.y_sorted, self.unsorted_indices, axis=2)
-        self.z = np.take_along_axis(self.z_sorted, self.unsorted_indices, axis=2)
+        Args:
+            locs (iterable): A list of the turbine coordinates, organized as
+                [x1, x2, ..., xn, y1, y2, ..., yn] (m).
 
-@define
-class FlowFieldGrid(Grid):
-    """
-    Args:
-        grid_resolution (`Vec3`): The number of grid points to be created in each direction.
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int`): The number of points on each turbine
-    """
+        Returns:
+            float: The area occupied by the wind farm (m^2).
+        """
+        locsx = locs[0 : self.nturbs]
+        locsy = locs[self.nturbs :]
+
+        points = zip(locsx, locsy)
+        points = np.array(list(points))
+
+        hull = self.convex_hull(points)
 
-    def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
-        self.set_grid()
-
-    def set_grid(self) -> None:
-        """
-        Create a structured grid for the entire flow field domain.
-        resolution: Vec3
-
-        Calculates the domain bounds for the current wake model. The bounds
-        are calculated based on preset extents from the
-        given layout. The bounds consist of the minimum and maximum values
-        in the x-, y-, and z-directions.
-
-        If the Curl model is used, the predefined bounds are always set.
-
-        First, sort the turbines so that we know the bounds in the correct orientation.
-        Then, create the grid based on this wind-from-left orientation
-        """
-
-        # These are the rotated coordinates of the wind turbines based on the wind direction
-        x, y, z = rotate_coordinates_rel_west(self.wind_directions, self.turbine_coordinates_array)
-
-        # Construct the arrays storing the grid points
-        eps = 0.01
-        xmin = min(x[0,0]) - 2 * self.reference_turbine_diameter
-        xmax = max(x[0,0]) + 10 * self.reference_turbine_diameter
-        ymin = min(y[0,0]) - 2 * self.reference_turbine_diameter
-        ymax = max(y[0,0]) + 2 * self.reference_turbine_diameter
-        zmin = 0 + eps
-        zmax = 6 * max(z[0,0])
-
-        x_points, y_points, z_points = np.meshgrid(
-            np.linspace(xmin, xmax, int(self.grid_resolution[0])),
-            np.linspace(ymin, ymax, int(self.grid_resolution[1])),
-            np.linspace(zmin, zmax, int(self.grid_resolution[2])),
-            indexing="ij"
+        area = self.polygon_area(
+            np.array([val[0] for val in hull]), np.array([val[1] for val in hull])
         )
 
-        self.x_sorted = x_points[None, None, :, :, :]
-        self.y_sorted = y_points[None, None, :, :, :]
-        self.z_sorted = z_points[None, None, :, :, :]
+        return area
 
-@define
-class FlowFieldPlanarGrid(Grid):
-    """
-    Args:
-        grid_resolution (`Vec3`): The number of grid points to be created in each direction.
-        turbine_coordinates (`list[Vec3]`): The collection of turbine coordinate (`Vec3`) objects.
-        reference_turbine_diameter (:py:obj:`float`): The reference turbine's rotor diameter.
-        grid_resolution (:py:obj:`int`): The number of points on each turbine
-    """
-    normal_vector: str = field()
-    planar_coordinate: float = field()
-    x1_bounds: tuple = field(default=None)
-    x2_bounds: tuple = field(default=None)
-
-    sorted_indices: NDArrayInt = field(init=False)
-    unsorted_indices: NDArrayInt = field(init=False)
-
-    def __attrs_post_init__(self) -> None:
-        super().__attrs_post_init__()
-        self.set_grid()
-
-    def set_grid(self) -> None:
-        """
-        Create a structured grid for the entire flow field domain.
-        resolution: Vec3
-
-        Calculates the domain bounds for the current wake model. The bounds
-        are calculated based on preset extents from the
-        given layout. The bounds consist of the minimum and maximum values
-        in the x-, y-, and z-directions.
-
-        If the Curl model is used, the predefined bounds are always set.
-
-        First, sort the turbines so that we know the bounds in the correct orientation.
-        Then, create the grid based on this wind-from-left orientation
-        """
-        # These are the rotated coordinates of the wind turbines based on the wind direction
-        x, y, z = rotate_coordinates_rel_west(self.wind_directions, self.turbine_coordinates_array)
-
-        max_diameter = np.max(self.reference_turbine_diameter)
-
-        if self.normal_vector == "z":  # Rules of thumb for horizontal plane
-            if self.x1_bounds is None:
-                self.x1_bounds = (np.min(x) - 2 * max_diameter, np.max(x) + 10 * max_diameter)
-
-            if self.x2_bounds is None:
-                self.x2_bounds = (np.min(y) - 2 * max_diameter, np.max(y) + 2 * max_diameter)
-
-            # TODO figure out proper z spacing for GCH, currently set to +/- 10.0
-            x_points, y_points, z_points = np.meshgrid(
-                np.linspace(self.x1_bounds[0], self.x1_bounds[1], int(self.grid_resolution[0])),
-                np.linspace(self.x2_bounds[0], self.x2_bounds[1], int(self.grid_resolution[1])),
-                np.array([
-                    float(self.planar_coordinate) - 10.0,
-                    float(self.planar_coordinate),
-                    float(self.planar_coordinate) + 10.0
-                ]),
-                indexing="ij"
-            )
+    def convex_hull(self, points):
+        """
+        Finds the vertices that describe the convex hull shape given the input
+        coordinates.
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
-
-        elif self.normal_vector == "x":  # Rules of thumb for cross plane
-            if self.x1_bounds is None:
-                self.x1_bounds = (np.min(y) - 2 * max_diameter, np.max(y) + 2 * max_diameter)
-
-            if self.x2_bounds is None:
-                self.x2_bounds = (0.001, 6 * np.max(z))
-
-            x_points, y_points, z_points = np.meshgrid(
-                np.array([float(self.planar_coordinate)]),
-                np.linspace(self.x1_bounds[0], self.x1_bounds[1], int(self.grid_resolution[0])),
-                np.linspace(self.x2_bounds[0], self.x2_bounds[1], int(self.grid_resolution[1])),
-                indexing="ij"
-            )
+        Args:
+            points (iterable((float, float))): Coordinates of interest.
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
-
-        elif self.normal_vector == "y":  # Rules of thumb for y plane
-            if self.x1_bounds is None:
-                self.x1_bounds = (np.min(x) - 2 * max_diameter, np.max(x) + 10 * max_diameter)
-
-            if self.x2_bounds is None:
-                self.x2_bounds = (0.001, 6 * np.max(z))
-
-            x_points, y_points, z_points = np.meshgrid(
-                np.linspace(self.x1_bounds[0], self.x1_bounds[1], int(self.grid_resolution[0])),
-                np.array([float(self.planar_coordinate)]),
-                np.linspace(self.x2_bounds[0], self.x2_bounds[1], int(self.grid_resolution[1])),
-                indexing="ij"
-            )
+        Returns:
+            list: Vertices describing convex hull shape.
+        """
+        # find two hull points, U, V, and split to left and right search
+        u = min(points, key=lambda p: p[0])
+        v = max(points, key=lambda p: p[0])
+        left, right = self.split(u, v, points), self.split(v, u, points)
+
+        # find convex hull on each side
+        return [v] + self.extend(u, v, left) + [u] + self.extend(v, u, right) + [v]
+
+    def polygon_area(self, x, y):
+        """
+        Calculates the area of a polygon defined by its (x, y) vertices.
+
+        Args:
+            x (iterable(float)): X-coordinates of polygon vertices.
+            y (iterable(float)): Y-coordinates of polygon vertices.
+
+        Returns:
+            float: Area of polygon.
+        """
+        # coordinate shift
+        x_ = x - x.mean()
+        y_ = y - y.mean()
+
+        correction = x_[-1] * y_[0] - y_[-1] * x_[0]
+        main_area = np.dot(x_[:-1], y_[1:]) - np.dot(y_[:-1], x_[1:])
+        return 0.5 * np.abs(main_area + correction)
+
+    def split(self, u, v, points):
+        # TODO: Provide description of this method.
+        # return points on left side of UV
+        return [p for p in points if np.cross(p - u, v - u) < 0]
+
+    def extend(self, u, v, points):
+        # TODO: Provide description of this method.
+        if not points:
+            return []
+
+        # find furthest point W, and split search to WV, UW
+        w = min(points, key=lambda p: np.cross(p - u, v - u))
+        p1, p2 = self.split(w, v, points), self.split(u, w, points)
+        return self.extend(w, v, p1) + [w] + self.extend(u, w, p2)
+
+    def plot_opt_results(self):
+        """
+        This method plots the original and new locations of the turbines in a
+        wind farm after layout optimization.
+        """
+        locsx_old = [
+            self._unnorm(valx, self.bndx_min, self.bndx_max)
+            for valx in self.x0[0 : self.nturbs]
+        ]
+        locsy_old = [
+            self._unnorm(valy, self.bndy_min, self.bndy_max)
+            for valy in self.x0[self.nturbs : 2 * self.nturbs]
+        ]
+        locsx = [
+            self._unnorm(valx, self.bndx_min, self.bndx_max)
+            for valx in self.residual_plant.x[0 : self.nturbs]
+        ]
+        locsy = [
+            self._unnorm(valy, self.bndy_min, self.bndy_max)
+            for valy in self.residual_plant.x[self.nturbs : 2 * self.nturbs]
+        ]
+
+        plt.figure(figsize=(9, 6))
+        fontsize = 16
+        plt.plot(locsx_old, locsy_old, "ob")
+        plt.plot(locsx, locsy, "or")
+        # plt.title('Layout Optimization Results', fontsize=fontsize)
+        plt.xlabel("x (m)", fontsize=fontsize)
+        plt.ylabel("y (m)", fontsize=fontsize)
+        plt.axis("equal")
+        plt.grid()
+        plt.tick_params(which="both", labelsize=fontsize)
+        plt.legend(
+            ["Old locations", "New locations"],
+            loc="lower center",
+            bbox_to_anchor=(0.5, 1.01),
+            ncol=2,
+            fontsize=fontsize,
+        )
 
-            self.x_sorted = x_points[None, None, :, :, :]
-            self.y_sorted = y_points[None, None, :, :, :]
-            self.z_sorted = z_points[None, None, :, :, :]
-
-        # self.sorted_indices = self.x.argsort(axis=2)
-        # self.unsorted_indices = self.sorted_indices.argsort(axis=2)
-
-        # Put the turbines into the final arrays in their sorted order
-        # self.x = np.take_along_axis(self.x, self.sorted_indices, axis=2)
-        # self.y = np.take_along_axis(self.y, self.sorted_indices, axis=2)
-        # self.z = np.take_along_axis(self.z, self.sorted_indices, axis=2)
-
-    # def finalize(self):
-        # sorted_indices = self.x.argsort(axis=2)
-        # unsorted_indices = sorted_indices.argsort(axis=2)
-
-        # # print(self.x)
-
-        # x_coordinates, y_coordinates, _ = self.turbine_coordinates_array.T
-
-        # x_center_of_rotation = (np.min(x_coordinates) + np.max(x_coordinates)) / 2
-        # y_center_of_rotation = (np.min(y_coordinates) + np.max(y_coordinates)) / 2
-        # # print(x_center_of_rotation)
-        # # print(y_center_of_rotation)
-        # # lkj
-
-        # self.x = np.take_along_axis(self.x, self.unsorted_indices, axis=2)
-        # self.y = np.take_along_axis(self.y, self.unsorted_indices, axis=2)
-        # self.z = np.take_along_axis(self.z, self.unsorted_indices, axis=2)
-        # # print(self.x)
-
-        # self.x, self.y, self.z = self._rotated_grid(
-        #     -1 * self.wind_directions,
-        #     (x_center_of_rotation, y_center_of_rotation)
-        # )
-        # TODO figure out how to un-rotate grid for plotting after it has been solved
-        # pass
-
-    # def _rotated_grid(self, angle, center_of_rotation):
-    #     """
-    #     Rotate the discrete flow field grid.
-    #     """
-    #     angle = ((angle - 270) % 360 + 360) % 360
-    #     # angle = np.reshape(angle, (len(angle), 1, 1))
-    #     xoffset = self.x - center_of_rotation[0]
-    #     yoffset = self.y - center_of_rotation[1]
-    #     rotated_x = (
-    #         xoffset * cosd(angle) - yoffset * sind(angle) + center_of_rotation[0]
-    #     )
-    #     rotated_y = (
-    #         xoffset * sind(angle) + yoffset * cosd(angle) + center_of_rotation[1]
-    #     )
-    #     return rotated_x, rotated_y, self.z
+        verts = self.boundaries
+        for i in range(len(verts)):
+            if i == len(verts) - 1:
+                plt.plot([verts[i][0], verts[0][0]], [verts[i][1], verts[0][1]], "b")
+            else:
+                plt.plot(
+                    [verts[i][0], verts[i + 1][0]], [verts[i][1], verts[i + 1][1]], "b"
+                )
```

### Comparing `FLORIS-3.3/floris/simulation/solver.py` & `FLORIS-3.4/floris/simulation/solver.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,35 +6,40 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
+from __future__ import annotations
+
 import copy
-import sys
-import time
 
 import numpy as np
 
 from floris.simulation import (
     axial_induction,
     Ct,
     Farm,
     FlowField,
     FlowFieldGrid,
+    FlowFieldPlanarGrid,
+    PointsGrid,
     TurbineGrid,
 )
 from floris.simulation.turbine import average_velocity
 from floris.simulation.wake import WakeModelManager
+from floris.simulation.wake_deflection.empirical_gauss import yaw_added_wake_mixing
 from floris.simulation.wake_deflection.gauss import (
     calculate_transverse_velocity,
     wake_added_yaw,
     yaw_added_turbulence_mixing,
 )
+from floris.type_dec import NDArrayFloat
+from floris.utilities import cosd
 
 
 def calculate_area_overlap(wake_velocities, freestream_velocities, y_ngrid, z_ngrid):
     """
     compute wake overlap based on the number of points that are not freestream
     velocity, i.e. affected by the wake
     """
@@ -90,27 +95,39 @@
 
         u_i = flow_field.u_sorted[:, :, i:i+1]
         v_i = flow_field.v_sorted[:, :, i:i+1]
 
         ct_i = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
         # get the first index here (0:1)
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
         axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
         turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
         yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
         hub_height_i = farm.hub_heights_sorted[: ,:, i:i+1, None, None]
@@ -236,33 +253,36 @@
         axis=(3,4)
     )[:, :, :, None, None]
 
 
 def full_flow_sequential_solver(
     farm: Farm,
     flow_field: FlowField,
-    flow_field_grid: FlowFieldGrid,
+    flow_field_grid: FlowFieldGrid | FlowFieldPlanarGrid | PointsGrid,
     model_manager: WakeModelManager
 ) -> None:
 
     # Get the flow quantities and turbine performance
     turbine_grid_farm = copy.deepcopy(farm)
     turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     turbine_grid_farm.construct_turbine_map()
     turbine_grid_farm.construct_turbine_fCts()
-    turbine_grid_farm.construct_turbine_fCps()
     turbine_grid_farm.construct_turbine_power_interps()
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
-    turbine_grid_farm.construc_turbine_pPs()
-    turbine_grid_farm.construc_turbine_ref_density_cp_cts()
+    turbine_grid_farm.construct_turbine_pPs()
+    turbine_grid_farm.construct_turbine_pTs()
+    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
     turbine_grid_farm.construct_coordinates()
-
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
         reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
         wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
@@ -306,25 +326,33 @@
 
         u_i = turbine_grid_flow_field.u_sorted[:, :, i:i+1]
         v_i = turbine_grid_flow_field.v_sorted[:, :, i:i+1]
 
         ct_i = Ct(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the Ct function,
         # get the first index here (0:1)
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
         axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
         turbulence_intensity_i = \
@@ -441,71 +469,78 @@
         x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
         x_i = x_i[:, :, :, None, None]
         y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
         y_i = y_i[:, :, :, None, None]
         z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
         z_i = z_i[:, :, :, None, None]
 
+        rotor_diameter_i = farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
+
         mask2 = (
             np.array(grid.x_sorted < x_i + 0.01)
             * np.array(grid.x_sorted > x_i - 0.01)
-            * np.array(grid.y_sorted < y_i + 0.51*126.0)
-            * np.array(grid.y_sorted > y_i - 0.51*126.0)
+            * np.array(grid.y_sorted < y_i + 0.51 * rotor_diameter_i)
+            * np.array(grid.y_sorted > y_i - 0.51 * rotor_diameter_i)
         )
-        # mask2 = (
-        #     np.logical_and(
-        #         np.logical_and(
-        #             np.logical_and(
-        #                 grid.x_sorted < x_i + 0.01,
-        #                 grid.x_sorted > x_i - 0.01
-        #             ),
-        #             grid.y_sorted < y_i + 0.51*126.0
-        #         ),
-        #         grid.y_sorted > y_i - 0.51*126.0
-        #     )
-        # )
         turb_inflow_field = (
             turb_inflow_field * ~mask2
             + (flow_field.u_initial_sorted - turb_u_wake) * mask2
         )
 
         turb_avg_vels = average_velocity(turb_inflow_field)
         turb_Cts = Ct(
             turb_avg_vels,
             farm.yaw_angles_sorted,
+            farm.tilt_angles_sorted,
+            farm.ref_tilt_cp_cts_sorted,
             farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         turb_Cts = turb_Cts[:, :, :, None, None]
         turb_aIs = axial_induction(
             turb_avg_vels,
             farm.yaw_angles_sorted,
+            farm.tilt_angles_sorted,
+            farm.ref_tilt_cp_cts_sorted,
             farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         turb_aIs = turb_aIs[:, :, :, None, None]
 
         u_i = turb_inflow_field[:, :, i:i+1]
         v_i = flow_field.v_sorted[:, :, i:i+1]
 
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
 
         axial_induction_i = axial_induction_i[:, :, :, None, None]
 
         turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
         yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
         hub_height_i = farm.hub_heights_sorted[: ,:, i:i+1, None, None]
-        rotor_diameter_i = farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
         TSR_i = farm.TSRs_sorted[: ,:, i:i+1, None, None]
 
         effective_yaw_i = np.zeros_like(yaw_angle_i)
         effective_yaw_i += yaw_angle_i
 
         if model_manager.enable_secondary_steering:
             added_yaw = wake_added_yaw(
@@ -629,22 +664,26 @@
 ) -> None:
     # Get the flow quantities and turbine performance
     turbine_grid_farm = copy.deepcopy(farm)
     turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     turbine_grid_farm.construct_turbine_map()
     turbine_grid_farm.construct_turbine_fCts()
-    turbine_grid_farm.construct_turbine_fCps()
     turbine_grid_farm.construct_turbine_power_interps()
     turbine_grid_farm.construct_hub_heights()
     turbine_grid_farm.construct_rotor_diameters()
     turbine_grid_farm.construct_turbine_TSRs()
-    turbine_grid_farm.construc_turbine_pPs()
-    turbine_grid_farm.construc_turbine_ref_density_cp_cts()
+    turbine_grid_farm.construct_turbine_pPs()
+    turbine_grid_farm.construct_turbine_pTs()
+    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
     turbine_grid_farm.construct_coordinates()
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
 
     turbine_grid = TurbineGrid(
         turbine_coordinates=turbine_grid_farm.coordinates,
         reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
         wind_directions=turbine_grid_flow_field.wind_directions,
         wind_speeds=turbine_grid_flow_field.wind_speeds,
         grid_resolution=3,
@@ -692,25 +731,37 @@
         u_i = turbine_grid_flow_field.u_sorted[:, :, i:i+1]
         v_i = turbine_grid_flow_field.v_sorted[:, :, i:i+1]
 
         turb_avg_vels = average_velocity(turbine_grid_flow_field.u_sorted)
         turb_Cts = Ct(
             velocities=turb_avg_vels,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights
         )
         turb_Cts = turb_Cts[:, :, :, None, None]
 
         axial_induction_i = axial_induction(
             velocities=turbine_grid_flow_field.u_sorted,
             yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
             fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights
         )
         axial_induction_i = axial_induction_i[:, :, :, None, None]
 
         turbulence_intensity_i = \
             turbine_grid_flow_field.turbulence_intensity_field_sorted_avg[:, :, i:i+1]
         yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, :, i:i+1, None, None]
         hub_height_i = turbine_grid_farm.hub_heights_sorted[: ,:, i:i+1, None, None]
@@ -782,14 +833,15 @@
             **deficit_model_args
         )
 
         flow_field.v_sorted += v_wake
         flow_field.w_sorted += w_wake
     flow_field.u_sorted = flow_field.u_initial_sorted - turb_u_wake
 
+
 def turbopark_solver(
     farm: Farm,
     flow_field: FlowField,
     grid: TurbineGrid,
     model_manager: WakeModelManager
 ) -> None:
     # Algorithm
@@ -828,34 +880,52 @@
 
         u_i = flow_field.u_sorted[:, :, i:i+1]
         v_i = flow_field.v_sorted[:, :, i:i+1]
 
         Cts = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
 
         ct_i = Ct(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the Ct function,
         # get the first index here (0:1)
         ct_i = ct_i[:, :, 0:1, None, None]
         axial_induction_i = axial_induction(
             velocities=flow_field.u_sorted,
             yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
             fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
             turbine_type_map=farm.turbine_type_map_sorted,
             ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
         )
         # Since we are filtering for the i'th turbine in the axial induction function,
         # get the first index here (0:1)
         axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
         turbulence_intensity_i = turbine_turbulence_intensity[:, :, i:i+1]
         yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
         hub_height_i = farm.hub_heights_sorted[: ,:, i:i+1, None, None]
@@ -895,17 +965,23 @@
                 y_ii = y_ii[:, :, :, None, None]
 
                 yaw_ii = farm.yaw_angles_sorted[:, :, ii:ii+1, None, None]
                 turbulence_intensity_ii = turbine_turbulence_intensity[:, :, ii:ii+1]
                 ct_ii = Ct(
                     velocities=flow_field.u_sorted,
                     yaw_angle=farm.yaw_angles_sorted,
+                    tilt_angle=farm.tilt_angles_sorted,
+                    ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
                     fCt=farm.turbine_fCts,
+                    tilt_interp=farm.turbine_fTilts,
+                    correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
                     turbine_type_map=farm.turbine_type_map_sorted,
-                    ix_filter=[ii]
+                    ix_filter=[ii],
+                    average_method=grid.average_method,
+                    cubature_weights=grid.cubature_weights
                 )
                 ct_ii = ct_ii[:, :, 0:1, None, None]
                 rotor_diameter_ii = farm.rotor_diameters_sorted[: ,:, ii:ii+1, None, None]
 
                 deflection_field_ii = model_manager.deflection_model.function(
                     x_ii,
                     y_ii,
@@ -1024,15 +1100,14 @@
 
     # # Get the flow quantities and turbine performance
     # turbine_grid_farm = copy.deepcopy(farm)
     # turbine_grid_flow_field = copy.deepcopy(flow_field)
 
     # turbine_grid_farm.construct_turbine_map()
     # turbine_grid_farm.construct_turbine_fCts()
-    # turbine_grid_farm.construct_turbine_fCps()
     # turbine_grid_farm.construct_turbine_power_interps()
     # turbine_grid_farm.construct_hub_heights()
     # turbine_grid_farm.construct_rotor_diameters()
     # turbine_grid_farm.construct_turbine_TSRs()
     # turbine_grid_farm.construc_turbine_pPs()
     # turbine_grid_farm.construct_coordinates()
 
@@ -1058,7 +1133,364 @@
     # flow_field.u = copy.deepcopy(turbine_grid_flow_field.u)
     # flow_field.v = copy.deepcopy(turbine_grid_flow_field.v)
     # flow_field.w = copy.deepcopy(turbine_grid_flow_field.w)
 
     # flow_field_grid.x = copy.deepcopy(turbine_grid.x)
     # flow_field_grid.y = copy.deepcopy(turbine_grid.y)
     # flow_field_grid.z = copy.deepcopy(turbine_grid.z)
+
+
+def empirical_gauss_solver(
+    farm: Farm,
+    flow_field: FlowField,
+    grid: TurbineGrid,
+    model_manager: WakeModelManager
+) -> NDArrayFloat:
+    """
+    Algorithm:
+    For each turbine, calculate its effect on every downstream turbine.
+    For the current turbine, we are calculating the deficit that it adds to downstream turbines.
+    Integrate this into the main data structure.
+    Move on to the next turbine.
+
+    Args:
+        farm (Farm)
+        flow_field (FlowField)
+        grid (TurbineGrid)
+        model_manager (WakeModelManager)
+
+    Raises:
+        NotImplementedError: Raised if secondary steering is enabled with the EmGauss model.
+        NotImplementedError: Raised if transverse velocities is enabled with the EmGauss model.
+
+    Returns:
+        NDArrayFloat: wake induced mixing field primarily for use in the full-flow EmGauss solver
+    """
+
+
+    # <<interface>>
+    deflection_model_args = model_manager.deflection_model.prepare_function(grid, flow_field)
+    deficit_model_args = model_manager.velocity_model.prepare_function(grid, flow_field)
+
+    # This is u_wake
+    wake_field = np.zeros_like(flow_field.u_initial_sorted)
+    v_wake = np.zeros_like(flow_field.v_initial_sorted)
+    w_wake = np.zeros_like(flow_field.w_initial_sorted)
+
+    x_locs = np.mean(grid.x_sorted, axis=(3, 4))[:,:,:,None]
+    downstream_distance_D = x_locs - np.transpose(x_locs, axes=(0,1,3,2))
+    downstream_distance_D = downstream_distance_D / \
+        np.repeat(farm.rotor_diameters_sorted[:,:,:,None], grid.n_turbines, axis=-1)
+    downstream_distance_D = np.maximum(downstream_distance_D, 0.1) # For ease
+    mixing_factor = np.zeros_like(downstream_distance_D)
+    mixing_factor[:,:,:,:] = model_manager.turbulence_model.atmospheric_ti_gain*\
+        flow_field.turbulence_intensity*np.eye(grid.n_turbines)
+
+    # Calculate the velocity deficit sequentially from upstream to downstream turbines
+    for i in range(grid.n_turbines):
+
+        # Get the current turbine quantities
+        x_i = np.mean(grid.x_sorted[:, :, i:i+1], axis=(3, 4))
+        x_i = x_i[:, :, :, None, None]
+        y_i = np.mean(grid.y_sorted[:, :, i:i+1], axis=(3, 4))
+        y_i = y_i[:, :, :, None, None]
+        z_i = np.mean(grid.z_sorted[:, :, i:i+1], axis=(3, 4))
+        z_i = z_i[:, :, :, None, None]
+
+        flow_field.u_sorted[:, :, i:i+1]
+        flow_field.v_sorted[:, :, i:i+1]
+
+        ct_i = Ct(
+            velocities=flow_field.u_sorted,
+            yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
+            fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
+            turbine_type_map=farm.turbine_type_map_sorted,
+            ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
+        )
+        # Since we are filtering for the i'th turbine in the Ct function,
+        # get the first index here (0:1)
+        ct_i = ct_i[:, :, 0:1, None, None]
+        axial_induction_i = axial_induction(
+            velocities=flow_field.u_sorted,
+            yaw_angle=farm.yaw_angles_sorted,
+            tilt_angle=farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=farm.ref_tilt_cp_cts_sorted,
+            fCt=farm.turbine_fCts,
+            tilt_interp=farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=farm.correct_cp_ct_for_tilt_sorted,
+            turbine_type_map=farm.turbine_type_map_sorted,
+            ix_filter=[i],
+            average_method=grid.average_method,
+            cubature_weights=grid.cubature_weights
+        )
+        # Since we are filtering for the i'th turbine in the axial induction function,
+        # get the first index here (0:1)
+        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
+        yaw_angle_i = farm.yaw_angles_sorted[:, :, i:i+1, None, None]
+        hub_height_i = farm.hub_heights_sorted[: ,:, i:i+1, None, None]
+        rotor_diameter_i = farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
+
+        effective_yaw_i = np.zeros_like(yaw_angle_i)
+        effective_yaw_i += yaw_angle_i
+
+        average_velocities = average_velocity(
+            flow_field.u_sorted,
+            method=grid.average_method,
+            cubature_weights=grid.cubature_weights
+        )
+        tilt_angle_i = farm.calculate_tilt_for_eff_velocities(average_velocities)
+        tilt_angle_i = tilt_angle_i[:, :, i:i+1, None, None]
+
+        if model_manager.enable_secondary_steering:
+            raise NotImplementedError(
+                "Secondary steering not available for this model.")
+
+        if model_manager.enable_transverse_velocities:
+            raise NotImplementedError(
+                "Transverse velocities not used in this model.")
+
+        if model_manager.enable_yaw_added_recovery:
+            # Influence of yawing on turbine's own wake
+            mixing_factor[:, :, i:i+1, i] += \
+                yaw_added_wake_mixing(
+                    axial_induction_i,
+                    yaw_angle_i,
+                    1,
+                    model_manager.deflection_model.yaw_added_mixing_gain
+                )
+
+        # Extract total wake induced mixing for turbine i
+        mixing_i = np.linalg.norm(
+            mixing_factor[:, :, i:i+1, :, None],
+            ord=2, axis=3, keepdims=True
+        )
+
+        # Model calculations
+        # NOTE: exponential
+        deflection_field_y, deflection_field_z = model_manager.deflection_model.function(
+            x_i,
+            y_i,
+            effective_yaw_i,
+            tilt_angle_i,
+            mixing_i,
+            ct_i,
+            rotor_diameter_i,
+            **deflection_model_args
+        )
+
+        # NOTE: exponential
+        velocity_deficit = model_manager.velocity_model.function(
+            x_i,
+            y_i,
+            z_i,
+            axial_induction_i,
+            deflection_field_y,
+            deflection_field_z,
+            yaw_angle_i,
+            tilt_angle_i,
+            mixing_i,
+            ct_i,
+            hub_height_i,
+            rotor_diameter_i,
+            **deficit_model_args
+        )
+
+        wake_field = model_manager.combination_model.function(
+            wake_field,
+            velocity_deficit * flow_field.u_initial_sorted
+        )
+
+        # Calculate wake overlap for wake-added turbulence (WAT)
+        area_overlap = np.sum(velocity_deficit * flow_field.u_initial_sorted > 0.05, axis=(3, 4))\
+            / (grid.grid_resolution * grid.grid_resolution)
+
+        # Compute wake induced mixing factor
+        mixing_factor[:,:,:,i] += \
+            area_overlap * model_manager.turbulence_model.function(
+                axial_induction_i, downstream_distance_D[:,:,:,i]
+            )
+        if model_manager.enable_yaw_added_recovery:
+            mixing_factor[:,:,:,i] += \
+                area_overlap * yaw_added_wake_mixing(
+                axial_induction_i,
+                yaw_angle_i,
+                downstream_distance_D[:,:,:,i],
+                model_manager.deflection_model.yaw_added_mixing_gain
+            )
+
+        flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
+        flow_field.v_sorted += v_wake
+        flow_field.w_sorted += w_wake
+
+    return mixing_factor
+
+
+def full_flow_empirical_gauss_solver(
+    farm: Farm,
+    flow_field: FlowField,
+    flow_field_grid: FlowFieldGrid,
+    model_manager: WakeModelManager
+) -> None:
+
+    # Get the flow quantities and turbine performance
+    turbine_grid_farm = copy.deepcopy(farm)
+    turbine_grid_flow_field = copy.deepcopy(flow_field)
+
+    turbine_grid_farm.construct_turbine_map()
+    turbine_grid_farm.construct_turbine_fCts()
+    turbine_grid_farm.construct_turbine_power_interps()
+    turbine_grid_farm.construct_hub_heights()
+    turbine_grid_farm.construct_rotor_diameters()
+    turbine_grid_farm.construct_turbine_TSRs()
+    turbine_grid_farm.construct_turbine_pPs()
+    turbine_grid_farm.construct_turbine_pTs()
+    turbine_grid_farm.construct_turbine_ref_density_cp_cts()
+    turbine_grid_farm.construct_turbine_ref_tilt_cp_cts()
+    turbine_grid_farm.construct_turbine_fTilts()
+    turbine_grid_farm.construct_turbine_correct_cp_ct_for_tilt()
+    turbine_grid_farm.construct_coordinates()
+    turbine_grid_farm.set_tilt_to_ref_tilt(flow_field.n_wind_directions, flow_field.n_wind_speeds)
+
+    turbine_grid = TurbineGrid(
+        turbine_coordinates=turbine_grid_farm.coordinates,
+        reference_turbine_diameter=turbine_grid_farm.rotor_diameters,
+        wind_directions=turbine_grid_flow_field.wind_directions,
+        wind_speeds=turbine_grid_flow_field.wind_speeds,
+        grid_resolution=3,
+        time_series=turbine_grid_flow_field.time_series,
+    )
+    turbine_grid_farm.expand_farm_properties(
+        turbine_grid_flow_field.n_wind_directions,
+        turbine_grid_flow_field.n_wind_speeds,
+        turbine_grid.sorted_coord_indices
+    )
+    turbine_grid_flow_field.initialize_velocity_field(turbine_grid)
+    turbine_grid_farm.initialize(turbine_grid.sorted_indices)
+    wim_field = empirical_gauss_solver(
+        turbine_grid_farm,
+        turbine_grid_flow_field,
+        turbine_grid,
+        model_manager
+    )
+
+    ### Referring to the quantities from above, calculate the wake in the full grid
+
+    # Use full flow_field here to use the full grid in the wake models
+    deflection_model_args = model_manager.deflection_model.prepare_function(
+        flow_field_grid, flow_field
+    )
+    deficit_model_args = model_manager.velocity_model.prepare_function(flow_field_grid, flow_field)
+
+    wake_field = np.zeros_like(flow_field.u_initial_sorted)
+    v_wake = np.zeros_like(flow_field.v_initial_sorted)
+    w_wake = np.zeros_like(flow_field.w_initial_sorted)
+
+    # Calculate the velocity deficit sequentially from upstream to downstream turbines
+    for i in range(flow_field_grid.n_turbines):
+
+        # Get the current turbine quantities
+        x_i = np.mean(turbine_grid.x_sorted[:, :, i:i+1], axis=(3, 4))
+        x_i = x_i[:, :, :, None, None]
+        y_i = np.mean(turbine_grid.y_sorted[:, :, i:i+1], axis=(3, 4))
+        y_i = y_i[:, :, :, None, None]
+        z_i = np.mean(turbine_grid.z_sorted[:, :, i:i+1], axis=(3, 4))
+        z_i = z_i[:, :, :, None, None]
+
+        turbine_grid_flow_field.u_sorted[:, :, i:i+1]
+        turbine_grid_flow_field.v_sorted[:, :, i:i+1]
+
+        ct_i = Ct(
+            velocities=turbine_grid_flow_field.u_sorted,
+            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
+            fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
+            turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            ix_filter=[i],
+        )
+        # Since we are filtering for the i'th turbine in the Ct function,
+        # get the first index here (0:1)
+        ct_i = ct_i[:, :, 0:1, None, None]
+        axial_induction_i = axial_induction(
+            velocities=turbine_grid_flow_field.u_sorted,
+            yaw_angle=turbine_grid_farm.yaw_angles_sorted,
+            tilt_angle=turbine_grid_farm.tilt_angles_sorted,
+            ref_tilt_cp_ct=turbine_grid_farm.ref_tilt_cp_cts_sorted,
+            fCt=turbine_grid_farm.turbine_fCts,
+            tilt_interp=turbine_grid_farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=turbine_grid_farm.correct_cp_ct_for_tilt_sorted,
+            turbine_type_map=turbine_grid_farm.turbine_type_map_sorted,
+            ix_filter=[i],
+        )
+        # Since we are filtering for the i'th turbine in the axial induction function,
+        # get the first index here (0:1)
+        axial_induction_i = axial_induction_i[:, :, 0:1, None, None]
+        yaw_angle_i = turbine_grid_farm.yaw_angles_sorted[:, :, i:i+1, None, None]
+        hub_height_i = turbine_grid_farm.hub_heights_sorted[: ,:, i:i+1, None, None]
+        rotor_diameter_i = turbine_grid_farm.rotor_diameters_sorted[: ,:, i:i+1, None, None]
+        wake_induced_mixing_i = wim_field[:, :, i:i+1, :, None].sum(axis=3, keepdims=1)
+
+        effective_yaw_i = np.zeros_like(yaw_angle_i)
+        effective_yaw_i += yaw_angle_i
+
+        average_velocities = average_velocity(
+            turbine_grid_flow_field.u_sorted,
+            method=turbine_grid.average_method,
+            cubature_weights=turbine_grid.cubature_weights
+        )
+        tilt_angle_i = turbine_grid_farm.calculate_tilt_for_eff_velocities(average_velocities)
+        tilt_angle_i = tilt_angle_i[:, :, i:i+1, None, None]
+
+        if model_manager.enable_secondary_steering:
+            raise NotImplementedError(
+                "Secondary steering not available for this model.")
+
+        if model_manager.enable_transverse_velocities:
+            raise NotImplementedError(
+                "Transverse velocities not used in this model.")
+
+        # Model calculations
+        # NOTE: exponential
+        deflection_field_y, deflection_field_z = model_manager.deflection_model.function(
+            x_i,
+            y_i,
+            effective_yaw_i,
+            tilt_angle_i,
+            wake_induced_mixing_i,
+            ct_i,
+            rotor_diameter_i,
+            **deflection_model_args
+        )
+
+        # NOTE: exponential
+        velocity_deficit = model_manager.velocity_model.function(
+            x_i,
+            y_i,
+            z_i,
+            axial_induction_i,
+            deflection_field_y,
+            deflection_field_z,
+            yaw_angle_i,
+            tilt_angle_i,
+            wake_induced_mixing_i,
+            ct_i,
+            hub_height_i,
+            rotor_diameter_i,
+            **deficit_model_args
+        )
+
+        wake_field = model_manager.combination_model.function(
+            wake_field,
+            velocity_deficit * flow_field.u_initial_sorted
+        )
+
+        flow_field.u_sorted = flow_field.u_initial_sorted - wake_field
+        flow_field.v_sorted += v_wake
+        flow_field.w_sorted += w_wake
```

### Comparing `FLORIS-3.3/floris/simulation/wake.py` & `FLORIS-3.4/floris/simulation/wake.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,27 @@
 from floris.simulation import BaseClass, BaseModel
 from floris.simulation.wake_combination import (
     FLS,
     MAX,
     SOSFS,
 )
 from floris.simulation.wake_deflection import (
+    EmpiricalGaussVelocityDeflection,
     GaussVelocityDeflection,
     JimenezVelocityDeflection,
     NoneVelocityDeflection,
 )
-from floris.simulation.wake_turbulence import CrespoHernandez, NoneWakeTurbulence
+from floris.simulation.wake_turbulence import (
+    CrespoHernandez,
+    NoneWakeTurbulence,
+    WakeInducedMixing,
+)
 from floris.simulation.wake_velocity import (
     CumulativeGaussCurlVelocityDeficit,
+    EmpiricalGaussVelocityDeficit,
     GaussVelocityDeficit,
     JensenVelocityDeficit,
     NoneVelocityDeficit,
     TurbOParkVelocityDeficit,
 )
 
 
@@ -41,26 +47,29 @@
         "fls": FLS,
         "max": MAX,
         "sosfs": SOSFS
     },
     "deflection_model": {
         "jimenez": JimenezVelocityDeflection,
         "gauss": GaussVelocityDeflection,
-        "none": NoneVelocityDeflection
+        "none": NoneVelocityDeflection,
+        "empirical_gauss": EmpiricalGaussVelocityDeflection
     },
     "turbulence_model": {
         "none": NoneWakeTurbulence,
-        "crespo_hernandez": CrespoHernandez
+        "crespo_hernandez": CrespoHernandez,
+        "wake_induced_mixing": WakeInducedMixing
     },
     "velocity_model": {
         "none": NoneVelocityDeficit,
         "cc": CumulativeGaussCurlVelocityDeficit,
         "gauss": GaussVelocityDeficit,
         "jensen": JensenVelocityDeficit,
-        "turbopark": TurbOParkVelocityDeficit
+        "turbopark": TurbOParkVelocityDeficit,
+        "empirical_gauss": EmpiricalGaussVelocityDeficit
     },
 }
 
 
 @define
 class WakeModelManager(BaseClass):
     """
```

### Comparing `FLORIS-3.3/floris/simulation/wake_combination/__init__.py` & `FLORIS-3.4/floris/simulation/wake_combination/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_combination/fls.py` & `FLORIS-3.4/floris/simulation/wake_combination/fls.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_combination/max.py` & `FLORIS-3.4/floris/simulation/wake_combination/max.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_combination/sosfs.py` & `FLORIS-3.4/floris/simulation/wake_combination/sosfs.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_deflection/__init__.py` & `FLORIS-3.4/floris/simulation/wake_deflection/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 # WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 
+from floris.simulation.wake_deflection.empirical_gauss import EmpiricalGaussVelocityDeflection
 from floris.simulation.wake_deflection.gauss import GaussVelocityDeflection
 from floris.simulation.wake_deflection.jimenez import JimenezVelocityDeflection
 from floris.simulation.wake_deflection.none import NoneVelocityDeflection
```

### Comparing `FLORIS-3.3/floris/simulation/wake_deflection/gauss.py` & `FLORIS-3.4/floris/simulation/wake_deflection/gauss.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,14 @@
         )
 
         delta_far_wake = delta_far_wake * np.array(x > x0)
         deflection = delta_near_wake + delta_far_wake
 
         return deflection
 
-
 ## GCH components
 
 def gamma(
     D,
     velocity,
     Uinf,
     Ct,
@@ -510,15 +509,14 @@
     I_total = np.sqrt( (2 / 3) * k_total ) / average_u_i
 
     # Remove ambient from total TI leaving only the TI due to mixing
     I_mixing = I_total - I_i
 
     return I_mixing[:,:,None,None,None]
 
-
 # def yaw_added_recovery_correction(
 #     self, U_local, U, W, x_locations, y_locations, turbine, turbine_coord
 # ):
 #         """
 #         This method corrects the U-component velocities when yaw added recovery
 #         is enabled. For more details on how the velocities are changed, see [1].
 #         # TODO add reference to 1
```

### Comparing `FLORIS-3.3/floris/simulation/wake_deflection/jimenez.py` & `FLORIS-3.4/floris/simulation/wake_deflection/jimenez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_deflection/none.py` & `FLORIS-3.4/floris/simulation/wake_deflection/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_turbulence/__init__.py` & `FLORIS-3.4/floris/simulation/wake_turbulence/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,7 +11,8 @@
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 
 from floris.simulation.wake_turbulence.crespo_hernandez import CrespoHernandez
 from floris.simulation.wake_turbulence.none import NoneWakeTurbulence
+from floris.simulation.wake_turbulence.wake_induced_mixing import WakeInducedMixing
```

### Comparing `FLORIS-3.3/floris/simulation/wake_turbulence/crespo_hernandez.py` & `FLORIS-3.4/floris/simulation/wake_turbulence/crespo_hernandez.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_turbulence/none.py` & `FLORIS-3.4/floris/simulation/wake_turbulence/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/__init__.py` & `FLORIS-3.4/floris/simulation/wake_velocity/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,11 +10,12 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 
 from floris.simulation.wake_velocity.cumulative_gauss_curl import CumulativeGaussCurlVelocityDeficit
+from floris.simulation.wake_velocity.empirical_gauss import EmpiricalGaussVelocityDeficit
 from floris.simulation.wake_velocity.gauss import GaussVelocityDeficit
 from floris.simulation.wake_velocity.jensen import JensenVelocityDeficit
 from floris.simulation.wake_velocity.none import NoneVelocityDeficit
 from floris.simulation.wake_velocity.turbopark import TurbOParkVelocityDeficit
```

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/cumulative_gauss_curl.py` & `FLORIS-3.4/floris/simulation/wake_velocity/cumulative_gauss_curl.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/gauss.py` & `FLORIS-3.4/floris/simulation/wake_velocity/gauss.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/jensen.py` & `FLORIS-3.4/floris/simulation/wake_velocity/jensen.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/none.py` & `FLORIS-3.4/floris/simulation/wake_velocity/none.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/turbopark.py` & `FLORIS-3.4/floris/simulation/wake_velocity/turbopark.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/simulation/wake_velocity/turbopark_lookup_table.mat` & `FLORIS-3.4/floris/simulation/wake_velocity/turbopark_lookup_table.mat`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/__init__.py` & `FLORIS-3.4/floris/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/cc_blade_utilities.py` & `FLORIS-3.4/floris/tools/cc_blade_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/cut_plane.py` & `FLORIS-3.4/floris/tools/cut_plane.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/floris_interface.py` & `FLORIS-3.4/floris/tools/floris_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,54 +23,49 @@
 from floris.logging_manager import LoggerBase
 from floris.simulation import Floris, State
 from floris.simulation.turbine import (
     average_velocity,
     axial_induction,
     Ct,
     power,
+    rotor_effective_velocity,
 )
 from floris.tools.cut_plane import CutPlane
 from floris.type_dec import NDArrayFloat
 
 
 class FlorisInterface(LoggerBase):
     """
     FlorisInterface provides a high-level user interface to many of the
     underlying methods within the FLORIS framework. It is meant to act as a
     single entry-point for the majority of users, simplifying the calls to
     methods on objects within FLORIS.
 
     Args:
-        configuration (:py:obj:`dict`): The Floris configuration dictarionary, JSON file,
-            or YAML file. The configuration should have the following inputs specified.
+        configuration (:py:obj:`dict`): The Floris configuration dictarionary or YAML file.
+            The configuration should have the following inputs specified.
                 - **flow_field**: See `floris.simulation.flow_field.FlowField` for more details.
                 - **farm**: See `floris.simulation.farm.Farm` for more details.
                 - **turbine**: See `floris.simulation.turbine.Turbine` for more details.
                 - **wake**: See `floris.simulation.wake.WakeManager` for more details.
                 - **logging**: See `floris.simulation.floris.Floris` for more details.
     """
 
-    def __init__(self, configuration: dict | str | Path, het_map=None):
+    def __init__(self, configuration: dict | str | Path):
         self.configuration = configuration
 
         if isinstance(self.configuration, (str, Path)):
             self.floris = Floris.from_file(self.configuration)
 
         elif isinstance(self.configuration, dict):
             self.floris = Floris.from_dict(self.configuration)
 
         else:
             raise TypeError("The Floris `configuration` must be of type 'dict', 'str', or 'Path'.")
 
-        # Store the heterogeneous map for use after reinitailization
-        self.het_map = het_map
-        # Assign the heterogeneous map to the flow field
-        # Needed for a direct call to fi.calculate_wake without fi.reinitialize
-        self.floris.flow_field.het_map = het_map
-
         # If ref height is -1, assign the hub height
         if np.abs(self.floris.flow_field.reference_wind_height + 1.0) < 1.0e-6:
             self.assign_hub_height_to_ref_height()
 
         # Make a check on reference height and provide a helpful warning
         unique_heights = np.unique(np.round(self.floris.farm.hub_heights, decimals=6))
         if ((
@@ -106,46 +101,49 @@
                 f"Current length is {unique_heights}."
             )
 
         self.floris.flow_field.reference_wind_height = unique_heights[0]
 
     def copy(self):
         """Create an independent copy of the current FlorisInterface object"""
-        return FlorisInterface(self.floris.as_dict(), het_map=self.het_map)
+        return FlorisInterface(self.floris.as_dict())
 
     def calculate_wake(
         self,
         yaw_angles: NDArrayFloat | list[float] | None = None,
-        # points: NDArrayFloat | list[float] | None = None,
-        # track_n_upstream_wakes: bool = False,
+        # tilt_angles: NDArrayFloat | list[float] | None = None,
     ) -> None:
         """
         Wrapper to the :py:meth:`~.Farm.set_yaw_angles` and
         :py:meth:`~.FlowField.calculate_wake` methods.
 
         Args:
             yaw_angles (NDArrayFloat | list[float] | None, optional): Turbine yaw angles.
                 Defaults to None.
-            points: (NDArrayFloat | list[float] | None, optional): The x, y, and z
-                coordinates at which the flow field velocity is to be recorded. Defaults
-                to None.
-            track_n_upstream_wakes (bool, optional): When *True*, will keep track of the
-                number of upstream wakes a turbine is experiencing. Defaults to *False*.
         """
 
         if yaw_angles is None:
             yaw_angles = np.zeros(
                 (
                     self.floris.flow_field.n_wind_directions,
                     self.floris.flow_field.n_wind_speeds,
                     self.floris.farm.n_turbines
                 )
             )
         self.floris.farm.yaw_angles = yaw_angles
 
+        # # TODO is this required?
+        # if tilt_angles is not None:
+        #     self.floris.farm.tilt_angles = tilt_angles
+        # else:
+        #     self.floris.farm.set_tilt_to_ref_tilt(
+        #         self.floris.flow_field.n_wind_directions,
+        #         self.floris.flow_field.n_wind_speeds
+        #     )
+
         # Initialize solution space
         self.floris.initialize_domain()
 
         # Perform the wake calculations
         self.floris.steady_state_atmospheric_condition()
 
     def calculate_no_wake(
@@ -180,33 +178,28 @@
         # Finalize values to user-supplied order
         self.floris.finalize()
 
     def reinitialize(
         self,
         wind_speeds: list[float] | NDArrayFloat | None = None,
         wind_directions: list[float] | NDArrayFloat | None = None,
-        # wind_layout: list[float] | NDArrayFloat | None = None,
         wind_shear: float | None = None,
         wind_veer: float | None = None,
         reference_wind_height: float | None = None,
         turbulence_intensity: float | None = None,
         # turbulence_kinetic_energy=None,
         air_density: float | None = None,
         # wake: WakeModelManager = None,
         layout_x: list[float] | NDArrayFloat | None = None,
         layout_y: list[float] | NDArrayFloat | None = None,
         turbine_type: list | None = None,
         turbine_library_path: str | Path | None = None,
-        # turbine_id: list[str] | None = None,
-        # wtg_id: list[str] | None = None,
-        # with_resolution: float | None = None,
         solver_settings: dict | None = None,
-        time_series: bool | None = False,
-        layout: tuple[list[float], list[float]] | tuple[NDArrayFloat, NDArrayFloat] | None = None,
-        het_map=None,
+        time_series: bool = False,
+        heterogenous_inflow_config=None,
     ):
         # Export the floris object recursively as a dictionary
         floris_dict = self.floris.as_dict()
         flow_field_dict = floris_dict["flow_field"]
         farm_dict = floris_dict["farm"]
 
         # Make the given changes
@@ -222,81 +215,72 @@
             flow_field_dict["wind_veer"] = wind_veer
         if reference_wind_height is not None:
             flow_field_dict["reference_wind_height"] = reference_wind_height
         if turbulence_intensity is not None:
             flow_field_dict["turbulence_intensity"] = turbulence_intensity
         if air_density is not None:
             flow_field_dict["air_density"] = air_density
-        if het_map is not None:
-            self.het_map = het_map
+        if heterogenous_inflow_config is not None:
+            flow_field_dict["heterogenous_inflow_config"] = heterogenous_inflow_config
 
         ## Farm
-        if layout is not None:
-            self.logger.warning(
-                "Use the `layout_x` and `layout_y` parameters in place of `layout` "
-                "because the `layout` parameter will be deprecated in 3.3."
-            )
-            layout_x = layout[0]
-            layout_y = layout[1]
         if layout_x is not None:
             farm_dict["layout_x"] = layout_x
         if layout_y is not None:
             farm_dict["layout_y"] = layout_y
         if turbine_type is not None:
             farm_dict["turbine_type"] = turbine_type
         if turbine_library_path is not None:
             farm_dict["turbine_library_path"] = turbine_library_path
 
-        if time_series:
-            flow_field_dict["time_series"] = True
-        else:
-            flow_field_dict["time_series"] = False
+        flow_field_dict["time_series"] = time_series
 
         ## Wake
         # if wake is not None:
         #     self.floris.wake = wake
-        # if turbulence_intensity is not None:
-        #     pass  # TODO: this should be in the code, but maybe got skipped?
         # if turbulence_kinetic_energy is not None:
         #     pass  # TODO: not needed until GCH
+
         if solver_settings is not None:
             floris_dict["solver"] = solver_settings
 
         floris_dict["flow_field"] = flow_field_dict
         floris_dict["farm"] = farm_dict
 
         # Create a new instance of floris and attach to self
         self.floris = Floris.from_dict(floris_dict)
-        # Re-assign the hetergeneous inflow map to flow field
-        self.floris.flow_field.het_map = self.het_map
 
     def get_plane_of_points(
         self,
         normal_vector="z",
         planar_coordinate=None,
     ):
         """
         Calculates velocity values through the
-        :py:meth:`~.FlowField.calculate_wake` method at points in plane
+        :py:meth:`FlorisInterface.calculate_wake` method at points in plane
         specified by inputs.
 
         Args:
             normal_vector (string, optional): Vector normal to plane.
                 Defaults to z.
             planar_coordinate (float, optional): Value of normal vector
                 to slice through. Defaults to None.
 
-
         Returns:
-            :py:class:`pandas.DataFrame`: containing values of x1, x2, u, v, w
+            :py:class:`pandas.DataFrame`: containing values of x1, x2, x3, u, v, w
         """
         # Get results vectors
-        x_flat = self.floris.grid.x_sorted[0, 0].flatten()
-        y_flat = self.floris.grid.y_sorted[0, 0].flatten()
-        z_flat = self.floris.grid.z_sorted[0, 0].flatten()
+        if (normal_vector == "z"):
+            x_flat = self.floris.grid.x_sorted_inertial_frame[0, 0].flatten()
+            y_flat = self.floris.grid.y_sorted_inertial_frame[0, 0].flatten()
+            z_flat = self.floris.grid.z_sorted_inertial_frame[0, 0].flatten()
+        else:
+            x_flat = self.floris.grid.x_sorted[0, 0].flatten()
+            y_flat = self.floris.grid.y_sorted[0, 0].flatten()
+            z_flat = self.floris.grid.z_sorted[0, 0].flatten()
         u_flat = self.floris.flow_field.u_sorted[0, 0].flatten()
         v_flat = self.floris.flow_field.v_sorted[0, 0].flatten()
         w_flat = self.floris.flow_field.w_sorted[0, 0].flatten()
 
         # Create a df of these
         if normal_vector == "z":
             df = pd.DataFrame(
@@ -419,15 +403,14 @@
             self.floris.grid.grid_resolution[0],
             self.floris.grid.grid_resolution[1],
             "z"
         )
 
         # Reset the fi object back to the turbine grid configuration
         self.floris = Floris.from_dict(floris_dict)
-        self.floris.flow_field.het_map = self.het_map
 
         # Run the simulation again for futher postprocessing (i.e. now we can get farm power)
         self.calculate_wake(yaw_angles=current_yaw_angles)
 
         return horizontal_plane
 
     def calculate_cross_plane(
@@ -498,15 +481,14 @@
         )
 
         # Compute the cutplane
         cross_plane = CutPlane(df, y_resolution, z_resolution, "x")
 
         # Reset the fi object back to the turbine grid configuration
         self.floris = Floris.from_dict(floris_dict)
-        self.floris.flow_field.het_map = self.het_map
 
         # Run the simulation again for futher postprocessing (i.e. now we can get farm power)
         self.calculate_wake(yaw_angles=current_yaw_angles)
 
         return cross_plane
 
     def calculate_y_plane(
@@ -577,15 +559,14 @@
         )
 
         # Compute the cutplane
         y_plane = CutPlane(df, x_resolution, z_resolution, "y")
 
         # Reset the fi object back to the turbine grid configuration
         self.floris = Floris.from_dict(floris_dict)
-        self.floris.flow_field.het_map = self.het_map
 
         # Run the simulation again for futher postprocessing (i.e. now we can get farm power)
         self.calculate_wake(yaw_angles=current_yaw_angles)
 
         return y_plane
 
     def check_wind_condition_for_viz(self, wd=None, ws=None):
@@ -612,45 +593,77 @@
         if self.floris.state is not State.USED:
             raise RuntimeError(
                 "Can't run function `FlorisInterface.get_turbine_powers` without "
                 "first running `FlorisInterface.calculate_wake`."
             )
 
         turbine_powers = power(
-            air_density=self.floris.flow_field.air_density,
             ref_density_cp_ct=self.floris.farm.ref_density_cp_cts,
-            velocities=self.floris.flow_field.u,
-            yaw_angle=self.floris.farm.yaw_angles,
-            pP=self.floris.farm.pPs,
+            rotor_effective_velocities=self.turbine_effective_velocities,
             power_interp=self.floris.farm.turbine_power_interps,
             turbine_type_map=self.floris.farm.turbine_type_map,
         )
         return turbine_powers
 
     def get_turbine_Cts(self) -> NDArrayFloat:
         turbine_Cts = Ct(
             velocities=self.floris.flow_field.u,
             yaw_angle=self.floris.farm.yaw_angles,
+            tilt_angle=self.floris.farm.tilt_angles,
+            ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
             fCt=self.floris.farm.turbine_fCts,
+            tilt_interp=self.floris.farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
             turbine_type_map=self.floris.farm.turbine_type_map,
+            average_method=self.floris.grid.average_method,
+            cubature_weights=self.floris.grid.cubature_weights,
         )
         return turbine_Cts
 
     def get_turbine_ais(self) -> NDArrayFloat:
         turbine_ais = axial_induction(
             velocities=self.floris.flow_field.u,
             yaw_angle=self.floris.farm.yaw_angles,
+            tilt_angle=self.floris.farm.tilt_angles,
+            ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
             fCt=self.floris.farm.turbine_fCts,
+            tilt_interp=self.floris.farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
             turbine_type_map=self.floris.farm.turbine_type_map,
+            average_method=self.floris.grid.average_method,
+            cubature_weights=self.floris.grid.cubature_weights,
         )
         return turbine_ais
 
     @property
     def turbine_average_velocities(self) -> NDArrayFloat:
-        return average_velocity(velocities=self.floris.flow_field.u)
+        return average_velocity(
+            velocities=self.floris.flow_field.u,
+            method=self.floris.grid.average_method,
+            cubature_weights=self.floris.grid.cubature_weights
+        )
+
+    @property
+    def turbine_effective_velocities(self) -> NDArrayFloat:
+        rotor_effective_velocities = rotor_effective_velocity(
+            air_density=self.floris.flow_field.air_density,
+            ref_density_cp_ct=self.floris.farm.ref_density_cp_cts,
+            velocities=self.floris.flow_field.u,
+            yaw_angle=self.floris.farm.yaw_angles,
+            tilt_angle=self.floris.farm.tilt_angles,
+            ref_tilt_cp_ct=self.floris.farm.ref_tilt_cp_cts,
+            pP=self.floris.farm.pPs,
+            pT=self.floris.farm.pTs,
+            tilt_interp=self.floris.farm.turbine_fTilts,
+            correct_cp_ct_for_tilt=self.floris.farm.correct_cp_ct_for_tilt,
+            turbine_type_map=self.floris.farm.turbine_type_map,
+            average_method=self.floris.grid.average_method,
+            cubature_weights=self.floris.grid.cubature_weights
+        )
+        return rotor_effective_velocities
 
     def get_turbine_TIs(self) -> NDArrayFloat:
         return self.floris.flow_field.turbulence_intensity_field
 
     def get_farm_power(
         self,
         turbine_weights=None,
@@ -911,18 +924,35 @@
 
         # Reset the FLORIS object to the original wind speed and directions
         self.reinitialize(
             wind_speeds=wind_speeds,
             wind_directions=wind_directions
         )
 
-
         return aep
 
+    def sample_flow_at_points(self, x: NDArrayFloat, y: NDArrayFloat, z: NDArrayFloat):
+        """
+        Extract the wind speed at points in the flow.
+
+        Args:
+            x (1DArrayFloat | list): x-locations of points where flow is desired.
+            y (1DArrayFloat | list): y-locations of points where flow is desired.
+            z (1DArrayFloat | list): z-locations of points where flow is desired.
+
+        Returns:
+            3DArrayFloat containing wind speed with dimensions
+            (# of wind directions, # of wind speeds, # of sample points)
+        """
+
+        # Check that x, y, z are all the same length
+        if not len(x) == len(y) == len(z):
+            raise ValueError("x, y, and z must be the same size")
 
+        return self.floris.solve_for_points(x, y, z)
 
     @property
     def layout_x(self):
         """
         Wind turbine coordinate information.
 
         Returns:
@@ -955,42 +985,14 @@
         xcoords, ycoords, zcoords = np.array([c.elements for c in self.floris.farm.coordinates]).T
         if z:
             return xcoords, ycoords, zcoords
         else:
             return xcoords, ycoords
 
 
-def generate_heterogeneous_wind_map(speed_ups, x, y, z=None):
-    if z is not None:
-        # Compute the 3-dimensional interpolants for each wind diretion
-        # Linear interpolation is used for points within the user-defined area of values,
-        # while a nearest-neighbor interpolant is used for points outside that region
-        in_region = [
-            LinearNDInterpolator(list(zip(x, y, z)), speed_up, fill_value=np.nan)
-            for speed_up in speed_ups
-        ]
-        out_region = [
-            NearestNDInterpolator(list(zip(x, y, z)), speed_up)
-            for speed_up in speed_ups
-        ]
-    else:
-        # Compute the 2-dimensional interpolants for each wind diretion
-        # Linear interpolation is used for points within the user-defined area of values,
-        # while a nearest-neighbor interpolant is used for points outside that region
-        in_region = [
-            LinearNDInterpolator(list(zip(x, y)), speed_up, fill_value=np.nan)
-            for speed_up in speed_ups
-        ]
-        out_region = [
-            NearestNDInterpolator(list(zip(x, y)), speed_up)
-            for speed_up in speed_ups
-        ]
-
-    return [in_region, out_region]
-
 ## Functionality removed in v3
 
 def set_rotor_diameter(self, rotor_diameter):
     """
     This function has been replaced and no longer works correctly, assigning an error
     """
     raise Exception(
```

### Comparing `FLORIS-3.3/floris/tools/floris_interface_legacy_reader.py` & `FLORIS-3.4/floris/tools/floris_interface_legacy_reader.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/flow_data.py` & `FLORIS-3.4/floris/tools/flow_data.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/interface_utilities.py` & `FLORIS-3.4/floris/tools/interface_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/layout_functions.py` & `FLORIS-3.4/floris/tools/layout_functions.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_base.py` & `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py` & `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py` & `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py` & `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_pyoptsparse_spread.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py` & `FLORIS-3.4/floris/tools/optimization/layout_optimization/layout_optimization_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/layout.py` & `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/optimization.py` & `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/optimization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/power_density.py` & `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/power_density.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/pyoptsparse/yaw.py` & `FLORIS-3.4/floris/tools/optimization/legacy/pyoptsparse/yaw.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/base_COE.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/base_COE.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/cluster_turbines.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/cluster_turbines.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,18 +111,15 @@
             return y
 
         def determine_if_in_wake(xt, yt):
             return (yt < wake_profile_ub_turbii(xt)) & (yt > wake_profile_lb_turbii(xt))
 
         # Get most downstream turbine
         is_downstream[ii] = not any(
-            [
-                determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii])
-                for iii in range(n_turbs)
-            ]
+            determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii]) for iii in range(n_turbs)
         )
         # Determine which turbines are affected by this turbine ('ii')
         affecting_following_turbs = [
                 determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii])
                 for iii in range(n_turbs)
         ]
 
@@ -161,15 +158,15 @@
     # Iteratively merge clusters if any overlap between turbines
     ci = 0
     while ci < len(clusters):
         # Compare current row to the ones to the right of it
         cj = ci + 1
         merged_column = False
         while cj < len(clusters):
-            if any([y in clusters[ci] for y in clusters[cj]]):
+            if any(y in clusters[ci] for y in clusters[cj]):
                 # Merge
                 clusters[ci] = np.hstack([clusters[ci], clusters[cj]])
                 clusters[ci] = np.array(np.unique(clusters[ci]), dtype=int)
                 clusters.pop(cj)
                 merged_column = True
             else:
                 cj = cj + 1
```

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/derive_downstream_turbines.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,18 +103,15 @@
                 y[x < x0 + 0.01] = -np.Inf
             return y
 
         def determine_if_in_wake(xt, yt):
             return (yt < wake_profile_ub_turbii(xt)) & (yt > wake_profile_lb_turbii(xt))
 
         is_downstream[ii] = not any(
-            [
-                determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii])
-                for iii in range(n_turbs)
-            ]
+            determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii]) for iii in range(n_turbs)
         )
 
         if plot_lines:
             x1 = np.max(x_rot_srt) + 500.0
             ax.fill_between(
                 [x0, x1, x1, x0],
                 [
```

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/layout.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/layout_height.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/layout_height.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/optimization.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/optimization.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/power_density_1D.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/power_density_1D.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_clustered.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py` & `FLORIS-3.4/floris/tools/optimization/legacy/scipy/yaw_wind_rose_parallel_clustered.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/other/boundary_grid.py` & `FLORIS-3.4/floris/tools/optimization/other/boundary_grid.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py` & `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_base.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py` & `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimization_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,18 +104,15 @@
                 y[x < x0 + 0.01] = -np.Inf
             return y
 
         def determine_if_in_wake(xt, yt):
             return (yt < wake_profile_ub_turbii(xt)) & (yt > wake_profile_lb_turbii(xt))
 
         is_downstream[ii] = not any(
-            [
-                determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii])
-                for iii in range(n_turbs)
-            ]
+            determine_if_in_wake(x_rot_srt[iii], y_rot_srt[iii]) for iii in range(n_turbs)
         )
 
         if plot_lines:
             x1 = np.max(x_rot_srt) + 500.0
             ax.fill_between(
                 [x0, x1, x1, x0],
                 [
```

### Comparing `FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py` & `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_scipy.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py` & `FLORIS-3.4/floris/tools/optimization/yaw_optimization/yaw_optimizer_sr.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,24 +10,27 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 
 import copy
+import warnings
 from time import perf_counter as timerpc
 
 import numpy as np
 import pandas as pd
 
+from floris.logging_manager import LoggerBase
+
 # from .yaw_optimizer_scipy import YawOptimizationScipy
 from .yaw_optimization_base import YawOptimization
 
 
-class YawOptimizationSR(YawOptimization):
+class YawOptimizationSR(YawOptimization, LoggerBase):
     def __init__(
         self,
         fi,
         minimum_yaw_angle=0.0,
         maximum_yaw_angle=25.0,
         yaw_angles_baseline=None,
         x0=None,
@@ -123,15 +126,19 @@
         farm_powers = np.zeros((yaw_angles_subset.shape[0], yaw_angles_subset.shape[1]))
 
         # Find indices of yaw angles that we previously already evaluated, and
         # prevent redoing the same calculations
         if use_memory:
             idx = (np.abs(yaw_angles_opt_subset - yaw_angles_subset) < 0.01).all(axis=2).all(axis=1)
             farm_powers[idx, :] = farm_power_opt_subset[idx, :]
-            print(f"Skipping {np.sum(idx)}/{len(idx)} calculations: already in memory.")
+            if self.print_progress:
+                self.logger.info(
+                    "Skipping {:d}/{:d} calculations: already in memory.".format(
+                        np.sum(idx), len(idx))
+                )
         else:
             idx = np.zeros(yaw_angles_subset.shape[0], dtype=bool)
 
         if not np.all(idx):
             # Now calculate farm powers for conditions we haven't yet evaluated previously
             start_time = timerpc()
             farm_powers[~idx, :] = self._calculate_farm_power(
@@ -214,38 +221,49 @@
         return farm_powers
 
     def optimize(self, print_progress=True):
         """
         Find the yaw angles that maximize the power production for every wind direction,
         wind speed and turbulence intensity.
         """
+        self.print_progress = print_progress
+
         # For each pass, from front to back
         ii = 0
         for Nii in range(len(self.Ny_passes)):
             # Disturb yaw angles for one turbine at a time, from front to back
             for turbine_depth in range(self.nturbs):
                 p = 100.0 * ii / (len(self.Ny_passes) * self.nturbs)
                 ii += 1
-                if print_progress:
+                if self.print_progress:
                     print(
                         f"[Serial Refine] Processing pass={Nii}, "
                         f"turbine_depth={turbine_depth} ({p:.1f}%)"
                     )
 
                 # Create grid to evaluate yaw angles for one turbine == turbine_depth
                 evaluation_grid = self._generate_evaluation_grid(
                     pass_depth=Nii,
                     turbine_depth=turbine_depth
                 )
 
                 # Evaluate grid of yaw angles, get farm powers and find optimal solutions
                 farm_powers = self._process_evaluation_grid()
 
+                # If farm powers contains any nans, then issue a warning
+                if np.any(np.isnan(farm_powers)):
+                    err_msg = (
+                        "NaNs found in farm powers during SerialRefine "
+                        "optimization routine. Proceeding to maximize over yaw "
+                        "settings that produce valid powers."
+                    )
+                    self.logger.warning(err_msg, stack_info=True)
+
                 # Find optimal solutions in new evaluation grid
-                args_opt = np.expand_dims(np.argmax(farm_powers, axis=0), axis=0)
+                args_opt = np.expand_dims(np.nanargmax(farm_powers, axis=0), axis=0)
                 farm_powers_opt_new = np.squeeze(
                     np.take_along_axis(farm_powers, args_opt, axis=0),
                     axis=0,
                 )
                 yaw_angles_opt_new = np.squeeze(
                     np.take_along_axis(
                         evaluation_grid,
```

### Comparing `FLORIS-3.3/floris/tools/parallel_computing_interface.py` & `FLORIS-3.4/floris/tools/parallel_computing_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,23 @@
 from floris.logging_manager import LoggerBase
 from floris.tools.optimization.yaw_optimization.yaw_optimizer_sr import YawOptimizationSR
 from floris.tools.uncertainty_interface import FlorisInterface, UncertaintyInterface
 
 
 def _load_local_floris_object(
     fi_dict,
-    het_map=None,
     unc_pmfs=None,
     fix_yaw_in_relative_frame=False
 ):
     # Load local FLORIS object
     if unc_pmfs is None:
-        fi = FlorisInterface(fi_dict, het_map=het_map)
+        fi = FlorisInterface(fi_dict)
     else:
         fi = UncertaintyInterface(
             fi_dict,
-            het_map=het_map,
             unc_pmfs=unc_pmfs,
             fix_yaw_in_relative_frame=fix_yaw_in_relative_frame,
         )
     return fi
 
 
 def _get_turbine_powers_serial(fi_information, yaw_angles=None):
@@ -213,15 +211,15 @@
                 wind_speeds = self.fi.floris.flow_field.wind_speeds[ws_id_split]
                 yaw_angles_subset = yaw_angles[wd_id_split[0]:wd_id_split[-1]+1, ws_id_split, :]
                 fi_dict_split["flow_field"]["wind_directions"] = wind_directions
                 fi_dict_split["flow_field"]["wind_speeds"] = wind_speeds
 
                 # Prepare lightweight data to pass along
                 if isinstance(self.fi, FlorisInterface):
-                    fi_information = (fi_dict_split, self.fi.het_map, None, None)
+                    fi_information = (fi_dict_split, None, None)
                 else:
                     fi_information = (
                         fi_dict_split,
                         self.fi.fi.het_map,
                         self.fi.unc_pmfs,
                         self.fi.fix_yaw_in_relative_frame
                     )
```

### Comparing `FLORIS-3.3/floris/tools/power_rose.py` & `FLORIS-3.4/floris/tools/power_rose.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/rews.py` & `FLORIS-3.4/floris/tools/rews.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/sowfa_utilities.py` & `FLORIS-3.4/floris/tools/sowfa_utilities.py`

 * *Files identical despite different names*

### Comparing `FLORIS-3.3/floris/tools/uncertainty_interface.py` & `FLORIS-3.4/floris/tools/uncertainty_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,28 +22,27 @@
 from floris.utilities import wrap_360
 
 
 class UncertaintyInterface(LoggerBase):
     def __init__(
         self,
         configuration,
-        het_map=None,
         unc_options=None,
         unc_pmfs=None,
         fix_yaw_in_relative_frame=False,
     ):
         """A wrapper around the nominal floris_interface class that adds
         uncertainty to the floris evaluations. One can specify a probability
         distribution function (pdf) for the ambient wind direction. Unless
         the exact pdf is specified manually using the option 'unc_pmfs', a
         Gaussian probability distribution function will be assumed.
 
         Args:
         configuration (:py:obj:`dict` or FlorisInterface object): The Floris
-            object, configuration dictarionary, JSON file, or YAML file. The
+            object, configuration dictarionary, or YAML file. The
             configuration should have the following inputs specified.
                 - **flow_field**: See `floris.simulation.flow_field.FlowField` for more details.
                 - **farm**: See `floris.simulation.farm.Farm` for more details.
                 - **turbine**: See `floris.simulation.turbine.Turbine` for more details.
                 - **wake**: See `floris.simulation.wake.WakeManager` for more details.
                 - **logging**: See `floris.simulation.floris.Floris` for more details.
         unc_options (dictionary, optional): A dictionary containing values
@@ -106,15 +105,15 @@
                 "pdf_cutoff": 0.995,  # Probability density function cut-off (-)
             }
 
         # Initialize floris object and uncertainty pdfs
         if isinstance(configuration, FlorisInterface):
             self.fi = configuration
         else:
-            self.fi = FlorisInterface(configuration, het_map=het_map)
+            self.fi = FlorisInterface(configuration)
 
         self.reinitialize_uncertainty(
             unc_options=unc_options,
             unc_pmfs=unc_pmfs,
             fix_yaw_in_relative_frame=fix_yaw_in_relative_frame,
         )
 
@@ -331,32 +330,23 @@
         wind_speeds=None,
         wind_directions=None,
         wind_shear=None,
         wind_veer=None,
         reference_wind_height=None,
         turbulence_intensity=None,
         air_density=None,
-        layout=None,
         layout_x=None,
         layout_y=None,
         turbine_type=None,
         solver_settings=None,
     ):
         """Pass to the FlorisInterface reinitialize function. To allow users
         to directly replace a FlorisInterface object with this
         UncertaintyInterface object, this function is required."""
 
-        if layout is not None:
-            self.logger.warning(
-                "Use the `layout_x` and `layout_y` parameters in place of `layout` "
-                "because the `layout` parameter will be deprecated in 3.3."
-            )
-            layout_x = layout[0]
-            layout_y = layout[1]
-
         # Just passes arguments to the floris object
         self.fi.reinitialize(
             wind_speeds=wind_speeds,
             wind_directions=wind_directions,
             wind_shear=wind_shear,
             wind_veer=wind_veer,
             reference_wind_height=reference_wind_height,
```

### Comparing `FLORIS-3.3/floris/tools/visualization.py` & `FLORIS-3.4/floris/tools/visualization.py`

 * *Files 18% similar despite different names*

```diff
@@ -18,32 +18,33 @@
 
 import matplotlib as mpl
 import matplotlib.colors as mplcolors
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from matplotlib import rcParams
+from scipy.spatial import ConvexHull
 
 from floris.simulation import Floris
 from floris.tools.cut_plane import CutPlane
 from floris.tools.floris_interface import FlorisInterface
-from floris.utilities import rotate_coordinates_rel_west
+from floris.utilities import rotate_coordinates_rel_west, wind_delta
 
 
 def show_plots():
     plt.show()
 
 def plot_turbines(
     ax,
     layout_x,
     layout_y,
     yaw_angles,
     rotor_diameters,
     color: str | None = None,
-    wind_direction: float = 270.0
+    wind_direction: float = 270.0,
 ):
     """
     Plot wind plant layout from turbine locations.
 
     Args:
         ax (:py:class:`matplotlib.pyplot.axes`): Figure axes.
         layout_x (np.array): Wind turbine locations (east-west).
@@ -52,50 +53,64 @@
         D (float): Wind turbine rotor diameter.
         color (str): Pyplot color option to plot the turbines.
         wind_direction (float): Wind direction (rotates farm)
     """
     if color is None:
         color = "k"
 
+    # Rotate layout to inertial frame for plotting turbines relative to wind direction
     coordinates_array = np.array([[x, y, 0.0] for x, y in list(zip(layout_x, layout_y))])
-    layout_x, layout_y, _ = rotate_coordinates_rel_west(
+    layout_x, layout_y, _, _, _ = rotate_coordinates_rel_west(
         np.array([wind_direction]),
         coordinates_array
     )
 
     for x, y, yaw, d in zip(layout_x[0,0], layout_y[0,0], yaw_angles, rotor_diameters):
         R = d / 2.0
         x_0 = x + np.sin(np.deg2rad(yaw)) * R
         x_1 = x - np.sin(np.deg2rad(yaw)) * R
         y_0 = y - np.cos(np.deg2rad(yaw)) * R
         y_1 = y + np.cos(np.deg2rad(yaw)) * R
         ax.plot([x_0, x_1], [y_0, y_1], color=color)
 
 
-def plot_turbines_with_fi(fi: FlorisInterface, ax=None, color=None, yaw_angles=None):
+def plot_turbines_with_fi(
+    fi: FlorisInterface,
+    ax=None,
+    color=None,
+    wd=None,
+    yaw_angles=None,
+):
     """
     Wrapper function to plot turbines which extracts the data
     from a FLORIS interface object
 
     Args:
-        fi (:py:class:`floris.tools.flow_data.FlowData`):
-                FlowData object.
-        ax (:py:class:`matplotlib.pyplot.axes`): figure axes.
-        color (str, optional): Color to plot turbines
+        fi (:py:class:`floris.tools.floris_interface.FlorisInterface`): FlorisInterface object.
+        ax (:py:class:`matplotlib.pyplot.axes`): Figure axes. Defaults to None.
+        color (str, optional): Color to plot turbines. Defaults to None.
+        wd (list, optional): The wind direction to plot the turbines relative to. Defaults to None.
+        yaw_angles (NDArray, optional): The yaw angles for the turbines. Defaults to None.
     """
     if not ax:
         fig, ax = plt.subplots()
     if yaw_angles is None:
         yaw_angles = fi.floris.farm.yaw_angles
+    if wd is None:
+        wd = fi.floris.flow_field.wind_directions[0]
+
+    # Rotate yaw angles to inertial frame for plotting turbines relative to wind direction
+    yaw_angles = yaw_angles - wind_delta(np.array(wd))
+
     plot_turbines(
         ax,
         fi.layout_x,
         fi.layout_y,
-        yaw_angles[0, 0],
-        fi.floris.farm.rotor_diameters[0, 0],
+        yaw_angles.flatten(),
+        fi.floris.farm.rotor_diameters.flatten(),
         color=color,
         wind_direction=fi.floris.flow_field.wind_directions[0],
     )
 
 
 def add_turbine_id_labels(fi: FlorisInterface, ax: plt.Axes, **kwargs):
     """
@@ -105,20 +120,22 @@
     kwargs are passed to Text
     (https://matplotlib.org/stable/api/text_api.html#matplotlib.text.Text).
 
     Args:
         fi (FlorisInterface): Simulation object to get the layout and index information.
         ax (plt.Axes): Axes object to add the labels.
     """
+
+    # Rotate layout to inertial frame for plotting turbines relative to wind direction
     coordinates_array = np.array([
         [x, y, 0.0]
         for x, y in list(zip(fi.layout_x, fi.layout_y))
     ])
     wind_direction = fi.floris.flow_field.wind_directions[0]
-    layout_x, layout_y, _ = rotate_coordinates_rel_west(
+    layout_x, layout_y, _, _, _ = rotate_coordinates_rel_west(
         np.array([wind_direction]),
         coordinates_array
     )
 
     for i in range(fi.floris.farm.n_turbines):
         ax.annotate(
             i,
@@ -144,23 +161,26 @@
             Defaults to None.
         **kwargs: Additional parameters to pass to `ax.contour`.
     """
 
     if not ax:
         fig, ax = plt.subplots()
 
-    # Reshape UMesh internally
-    x1_mesh = cut_plane.df.x1.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
-    x2_mesh = cut_plane.df.x2.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
-    u_mesh = cut_plane.df.u.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
-    Zm = np.ma.masked_where(np.isnan(u_mesh), u_mesh)
     rcParams["contour.negative_linestyle"] = "solid"
 
     # Plot the cut-through
-    contours = ax.contour(x1_mesh, x2_mesh, Zm, levels=levels, colors=colors, **kwargs)
+    contours = ax.tricontour(
+        cut_plane.df.x1,
+        cut_plane.df.x2,
+        cut_plane.df.u,
+        levels=levels,
+        colors=colors,
+        extend="both",
+        **kwargs,
+    )
 
     ax.clabel(contours, contours.levels, inline=True, fontsize=10, colors="black")
 
     # Make equal axis
     ax.set_aspect("equal")
 
 
@@ -168,85 +188,228 @@
     cut_plane,
     ax=None,
     vel_component='u',
     min_speed=None,
     max_speed=None,
     cmap="coolwarm",
     levels=None,
+    clevels=None,
     color_bar=False,
     title="",
     **kwargs
 ):
     """
     Generate pseudocolor mesh plot of the cut_plane.
 
     Args:
         cut_plane (:py:class:`~.tools.cut_plane.CutPlane`): 2D
             plane through wind plant.
-        ax (:py:class:`matplotlib.pyplot.axes`): Figure axes. Defaults
+        ax (:py:class:`matplotlib.pyplot.axes`, optional): Figure axes. Defaults
             to None.
+        vel_component (str, optional): The velocity component that the cut plane is
+            perpendicular to.
         min_speed (float, optional): Minimum value of wind speed for
             contours. Defaults to None.
         max_speed (float, optional): Maximum value of wind speed for
             contours. Defaults to None.
         cmap (str, optional): Colormap specifier. Defaults to
             'coolwarm'.
+        levels (np.array, optional): Contour levels for line contour plot.
+            Defaults to None.
+        clevels (np.array, optional): Contour levels for tricontourf plot.
+            Defaults to None.
+        color_bar (Boolean, optional): Flag to include a color bar on the plot.
+            Defaults to False.
+        title (str, optional): User-supplied title for the plot. Defaults to "".
+        **kwargs: Additional parameters to pass to line contour plot.
 
     Returns:
         im (:py:class:`matplotlib.plt.pcolormesh`): Image handle.
     """
 
     if not ax:
         fig, ax = plt.subplots()
+
     if vel_component=='u':
-        vel_mesh = cut_plane.df.u.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        # vel_mesh = cut_plane.df.u.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
         if min_speed is None:
             min_speed = cut_plane.df.u.min()
         if max_speed is None:
             max_speed = cut_plane.df.u.max()
     elif vel_component=='v':
-        vel_mesh = cut_plane.df.v.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        # vel_mesh = cut_plane.df.v.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
         if min_speed is None:
             min_speed = cut_plane.df.v.min()
         if max_speed is None:
             max_speed = cut_plane.df.v.max()
     elif vel_component=='w':
-        vel_mesh = cut_plane.df.w.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        # vel_mesh = cut_plane.df.w.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
         if min_speed is None:
             min_speed = cut_plane.df.w.min()
         if max_speed is None:
             max_speed = cut_plane.df.w.max()
 
-    # Reshape to 2d for plotting
-    x1_mesh = cut_plane.df.x1.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
-    x2_mesh = cut_plane.df.x2.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
-    Zm = np.ma.masked_where(np.isnan(vel_mesh), vel_mesh)
+    # Allow separate number of levels for tricontourf and for line_contour
+    if clevels is None:
+        clevels = levels
 
     # Plot the cut-through
-    im = ax.pcolormesh(
-        x1_mesh,
-        x2_mesh,
-        Zm,
+    im = ax.tricontourf(
+        cut_plane.df.x1,
+        cut_plane.df.x2,
+        cut_plane.df.u,
+        vmin=min_speed,
+        vmax=max_speed,
+        levels=clevels,
         cmap=cmap,
+        extend="both",
+    )
+
+    # Add line contour
+    line_contour_cut_plane(
+        cut_plane,
+        ax=ax,
+        levels=levels,
+        colors="b",
+        linewidths=0.8,
+        alpha=0.3,
+        **kwargs
+    )
+
+    if cut_plane.normal_vector == "x":
+        ax.invert_xaxis()
+
+    if color_bar:
+        cbar = plt.colorbar(im, ax=ax)
+        cbar.set_label('m/s')
+
+    # Set the title
+    ax.set_title(title)
+
+    # Make equal axis
+    ax.set_aspect("equal")
+
+    return im
+
+
+def visualize_heterogeneous_cut_plane(
+    cut_plane,
+    fi,
+    ax=None,
+    vel_component='u',
+    min_speed=None,
+    max_speed=None,
+    cmap="coolwarm",
+    levels=None,
+    clevels=None,
+    color_bar=False,
+    title="",
+    plot_het_bounds=True,
+    **kwargs
+):
+    """
+    Generate pseudocolor mesh plot of the heterogeneous cut_plane.
+
+    Args:
+        cut_plane (:py:class:`~.tools.cut_plane.CutPlane`): 2D
+            plane through wind plant.
+        fi (:py:class:`~.tools.floris_interface.FlorisInterface`): FlorisInterface object.
+        ax (:py:class:`matplotlib.pyplot.axes`): Figure axes. Defaults
+            to None.
+        vel_component (str, optional): The velocity component that the cut plane is
+            perpendicular to.
+        min_speed (float, optional): Minimum value of wind speed for
+            contours. Defaults to None.
+        max_speed (float, optional): Maximum value of wind speed for
+            contours. Defaults to None.
+        cmap (str, optional): Colormap specifier. Defaults to
+            'coolwarm'.
+        levels (np.array, optional): Contour levels for line contour plot.
+            Defaults to None.
+        clevels (np.array, optional): Contour levels for tricontourf plot.
+            Defaults to None.
+        color_bar (Boolean, optional): Flag to include a color bar on the plot.
+            Defaults to False.
+        title (str, optional): User-supplied title for the plot. Defaults to "".
+        plot_het_bonds (boolean, optional): Flag to include the user-defined bounds of the
+            heterogeneous wind speed area. Defaults to True.
+        **kwargs: Additional parameters to pass to line contour plot.
+
+    Returns:
+        im (:py:class:`matplotlib.plt.pcolormesh`): Image handle.
+    """
+
+    if not ax:
+        fig, ax = plt.subplots()
+    if vel_component=='u':
+        # vel_mesh = cut_plane.df.u.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        if min_speed is None:
+            min_speed = cut_plane.df.u.min()
+        if max_speed is None:
+            max_speed = cut_plane.df.u.max()
+    elif vel_component=='v':
+        # vel_mesh = cut_plane.df.v.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        if min_speed is None:
+            min_speed = cut_plane.df.v.min()
+        if max_speed is None:
+            max_speed = cut_plane.df.v.max()
+    elif vel_component=='w':
+        # vel_mesh = cut_plane.df.w.values.reshape(cut_plane.resolution[1], cut_plane.resolution[0])
+        if min_speed is None:
+            min_speed = cut_plane.df.w.min()
+        if max_speed is None:
+            max_speed = cut_plane.df.w.max()
+
+    # Allow separate number of levels for tricontourf and for line_contour
+    if clevels is None:
+        clevels = levels
+
+    # Plot the cut-through
+    im = ax.tricontourf(
+        cut_plane.df.x1,
+        cut_plane.df.x2,
+        cut_plane.df.u,
         vmin=min_speed,
         vmax=max_speed,
-        shading="nearest"
+        levels=clevels,
+        cmap=cmap,
+        extend="both",
     )
 
     # Add line contour
     line_contour_cut_plane(
         cut_plane,
         ax=ax,
         levels=levels,
         colors="b",
         linewidths=0.8,
         alpha=0.3,
         **kwargs
     )
 
+    # Plot the user-defined heterogeneous flow area
+    if plot_het_bounds:
+        points = np.array(
+            list(
+                zip(
+                    fi.floris.flow_field.heterogenous_inflow_config['x'],
+                    fi.floris.flow_field.heterogenous_inflow_config['y'],
+                )
+            )
+        )
+        hull = ConvexHull(points)
+        h = ax.plot(
+            points[np.append(hull.vertices, hull.vertices[0]),0],
+            points[np.append(hull.vertices, hull.vertices[0]), 1],
+            'k--',
+            lw=2,
+        )
+        ax.plot(points[hull.vertices,0], points[hull.vertices,1], 'ko')
+        ax.legend(h, ["defined heterogeneous bounds"], loc=1)
+
     if cut_plane.normal_vector == "x":
         ax.invert_xaxis()
 
     if color_bar:
         cbar = plt.colorbar(im, ax=ax)
         cbar.set_label('m/s')
 
@@ -323,47 +486,62 @@
     n_cols: int,
     t_range: range | None = None,
     cmap: str = "coolwarm",
     return_fig_objects: bool = False,
     save_path: Union[str, None] = None,
     show: bool = False
 ) -> Union[None, tuple[plt.figure, plt.axes, plt.axis, plt.colorbar]]:
-    """Plots the gridded turbine rotor values. This is intended to be used for
+    """
+    Plots the gridded turbine rotor values. This is intended to be used for
     understanding the differences between two sets of values, so each subplot can be
     used for inspection of what values are differing, and under what conditions.
 
     Parameters:
         values (np.ndarray): The 5-dimensional array of values to plot. Should be:
             N wind directions x N wind speeds x N turbines X N rotor points X N rotor points.
-        cmap (str): The matplotlib colormap to be used, default "coolwarm".
-        return_fig_objects (bool): Indicator to return the primary figure objects for
+        wd_index (int): The index for the wind direction to plot.
+        ws_index (int): The index of the wind speed to plot.
+        n_rows (int): The number of rows to include for subplots. With ncols, this should
+            generally add up to the number of turbines in the farm.
+        n_cols (int): The number of columns to include for subplots. With ncols, this should
+            generally add up to the number of turbines in the farm.
+        t_range (range | None): Optional. The turbine count used to create the title for each
+            subplot. If not provided, the size of the 2-th dimension of `values` is used.
+        cmap (str): Optional. The matplotlib colormap to be used, default "coolwarm".
+        return_fig_objects (bool): Optional. Flag to return the primary figure objects for
             further editing, default False.
-        save_path (str | None): Where to save the figure, if a value is provided.
-        t_range is turbine range; i.e. the turbine index to loop over
+        save_path (str | None): Optional. Where to save the figure, if a value is provided.
+        show (bool): Optional. Flag to run `plt.show()` to present all the plots
+            currently created with matplotlib.
 
     Returns:
         None | tuple[plt.figure, plt.axes, plt.axis, plt.colorbar]: If
         `return_fig_objects` is `False, then `None` is returned`, otherwise the primary
         figure objects are returned for custom editing.
 
     Example:
         from floris.tools.visualization import plot_rotor_values
-        plot_rotor_values(floris.flow_field.u, wd_index=0, ws_index=0)
-        plot_rotor_values(floris.flow_field.v, wd_index=0, ws_index=0)
-        plot_rotor_values(floris.flow_field.w, wd_index=0, ws_index=0, show=True)
+        plot_rotor_values(floris.flow_field.u, wd_index=0, ws_index=0, n_rows=1, ncols=4)
+        plot_rotor_values(floris.flow_field.v, wd_index=0, ws_index=0, n_rows=1, ncols=4)
+        plot_rotor_values(floris.flow_field.w, wd_index=0, ws_index=0, n_rows=1, ncols=4, show=True)
     """
 
     cmap = plt.cm.get_cmap(name=cmap)
 
     if t_range is None:
         t_range = range(values.shape[2])
 
     fig = plt.figure()
     axes = fig.subplots(n_rows, n_cols)
 
+    # For 1x1, fig.subplots returns an Axes object, but for more than 1x1 it returns a np.array.
+    # In this case, convert to an array so that the rest of this function can be simplified.
+    if n_rows == 1 and n_cols == 1:
+        axes = np.array([axes])
+
     titles = np.array([f"T{i}" for i in t_range])
 
     for ax, t, i in zip(axes.flatten(), titles, t_range):
 
         vmin = np.min(values[wd_index, ws_index])
         vmax = np.max(values[wd_index, ws_index])
```

### Comparing `FLORIS-3.3/floris/tools/wind_rose.py` & `FLORIS-3.4/floris/tools/wind_rose.py`

 * *Files 0% similar despite different names*

```diff
@@ -1474,14 +1474,15 @@
             # break
 
         # Configure the plot
         ax.legend(reversed(rects), ws_labels, **legend_kwargs)
         ax.set_theta_direction(-1)
         ax.set_theta_offset(np.pi / 2.0)
         ax.set_theta_zero_location("N")
+        ax.set_xticks(np.arange(0, 2*np.pi, np.pi/4))
         ax.set_xticklabels(["N", "NE", "E", "SE", "S", "SW", "W", "NW"])
 
         return ax
 
     def plot_wind_rose_ti(
         self,
         ax=None,
@@ -1548,14 +1549,15 @@
                 )
 
         # Configure the plot
         ax.legend(reversed(rects), ti_labels, loc="lower right", title="TI")
         ax.set_theta_direction(-1)
         ax.set_theta_offset(np.pi / 2.0)
         ax.set_theta_zero_location("N")
+        ax.set_xticks(np.arange(0, 2*np.pi, np.pi/4))
         ax.set_xticklabels(["N", "NE", "E", "SE", "S", "SW", "W", "NW"])
 
         return ax
 
     def plot_ti_ws(self, ax=None, ws_bins=np.arange(0, 26, 1.0)):
         """
         This method plots the wind speed frequency distribution of the WindRose
```

### Comparing `FLORIS-3.3/floris/turbine_library/iea_10MW.yaml` & `FLORIS-3.4/floris/turbine_library/iea_10MW.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 generator_efficiency: 1.0
 hub_height: 119.0
 pP: 1.88
 pT: 1.88
 rotor_diameter: 198.0
 TSR: 8.0
 ref_density_cp_ct: 1.225
+ref_tilt_cp_ct: 6.0
 power_thrust_table:
   power:
     - 0.000000
     - 0.000000
     - 0.074
     - 0.325100
     - 0.376200
```

### Comparing `FLORIS-3.3/floris/turbine_library/iea_15MW.yaml` & `FLORIS-3.4/floris/turbine_library/iea_15MW.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 generator_efficiency: 1.0
 hub_height: 150.0
 pP: 1.88
 pT: 1.88
 rotor_diameter: 242.24
 TSR: 8.0
 ref_density_cp_ct: 1.225
+ref_tilt_cp_ct: 6.0
 power_thrust_table:
   power:
     - 0.000000
     - 0.049361236
     - 0.224324252
     - 0.312216418
     - 0.36009987
```

### Comparing `FLORIS-3.3/floris/turbine_library/x_20MW.yaml` & `FLORIS-3.4/floris/turbine_library/x_20MW.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 turbine_type: 'x_20MW'
 generator_efficiency: 1.0
 hub_height: 165.0
 pP: 1.88
 pT: 1.88
 rotor_diameter: 252.0
 TSR: 8.0
+ref_density_cp_ct: 1.225
+ref_tilt_cp_ct: 5.0
 power_thrust_table:
   power:
     - 0.000000
     - 0.000000
     - 0.074000
     - 0.325100
     - 0.376200
```

### Comparing `FLORIS-3.3/floris/type_dec.py` & `FLORIS-3.4/floris/type_dec.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # License for the specific language governing permissions and limitations under
 # the License.
 
 # See https://floris.readthedocs.io for documentation
 
 from __future__ import annotations
 
+import copy
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Iterable,
     Tuple,
     Union,
@@ -33,31 +34,32 @@
 
 floris_float_type = np.float64
 
 NDArrayFloat = npt.NDArray[floris_float_type]
 NDArrayInt = npt.NDArray[np.int_]
 NDArrayFilter = Union[npt.NDArray[np.int_], npt.NDArray[np.bool_]]
 NDArrayObject = npt.NDArray[np.object_]
+NDArrayBool = npt.NDArray[np.bool_]
 
 
 ### Custom callables for attrs objects and functions
 
 def floris_array_converter(data: Iterable) -> np.ndarray:
     try:
         a = np.array(data, dtype=floris_float_type)
     except TypeError as e:
         raise TypeError(e.args[0] + f". Data given: {data}")
     return a
 
-def attr_serializer(inst: type, field: Attribute, value: Any):
+def _attr_serializer(inst: type, field: Attribute, value: Any):
     if isinstance(value, np.ndarray):
         return value.tolist()
     return value
 
-def attr_floris_filter(inst: Attribute, value: Any) -> bool:
+def _attr_floris_filter(inst: Attribute, value: Any) -> bool:
     if inst.init is False:
         return False
     if value is None:
         return False
     if isinstance(value, np.ndarray):
         if value.size == 0:
             return False
@@ -81,15 +83,14 @@
     """
     validator = attrs.validators.deep_iterable(
         member_validator=attrs.validators.instance_of(item_types),
         iterable_validator=attrs.validators.instance_of(iter_type),
     )
     return validator
 
-
 def convert_to_path(fn: str | Path) -> Path:
     """Converts an input string or pathlib.Path object to a fully resolved ``pathlib.Path``
     object.
 
     Args:
         fn (str | Path): The user input file path or file name.
 
@@ -109,15 +110,15 @@
     return fn
 
 
 @define
 class FromDictMixin:
     """
     A Mixin class to allow for kwargs overloading when a data class doesn't
-    have a specific parameter definied. This allows passing of larger dictionaries
+    have a specific parameter defined. This allows passing of larger dictionaries
     to a data class without throwing an error.
     """
 
     @classmethod
     def from_dict(cls, data: dict):
         """Maps a data dictionary to an `attr`-defined class.
 
@@ -126,14 +127,17 @@
         Args:
             data : dict
                 The data dictionary to be mapped.
         Returns:
             cls
                 The `attr`-defined class.
         """
+        # Make a copy of the input dict to prevent any side effects
+        data = copy.deepcopy(data)
+
         # Check for any inputs that aren't part of the class definition
         class_attr_names = [a.name for a in cls.__attrs_attrs__]
         extra_args = [d for d in data if d not in class_attr_names]
         if len(extra_args):
             raise AttributeError(
                 f"The initialization for {cls.__name__} was given extraneous inputs: {extra_args}"
             )
@@ -146,28 +150,29 @@
             for a in cls.__attrs_attrs__
             if a.init and a.default is attrs.NOTHING
         ]
         undefined = sorted(set(required_inputs) - set(kwargs))
 
         if undefined:
             raise AttributeError(
-                f"The class defintion for {cls.__name__} "
-                "is missing the following inputs: {undefined}"
+                f"The class definition for {cls.__name__} "
+                f"is missing the following inputs: {undefined}"
             )
         return cls(**kwargs)
 
     def as_dict(self) -> dict:
-        """Creates a JSON and YAML friendly dictionary that can be save for future reloading.
+        """Creates a YAML friendly dictionary that can be saved for future reloading.
         This dictionary will contain only `Python` types that can later be converted to their
-        proper `Turbine` formats.
+        proper formats. See `_attr_floris_filter` for detail on which attributes are
+        removed from the export.
 
         Returns:
-            dict: All key, vaue pais required for class recreation.
+            dict: All key, value pairs required for class recreation.
         """
-        return attrs.asdict(self, filter=attr_floris_filter, value_serializer=attr_serializer)
+        return attrs.asdict(self, filter=_attr_floris_filter, value_serializer=_attr_serializer)
 
 
 # Avoids constant redefinition of the same attr.ib properties for model attributes
 
 # from functools import partial, update_wrapper
 
 # def is_default(instance, attribute, value):
```

### Comparing `FLORIS-3.3/pyproject.toml` & `FLORIS-3.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -115,14 +115,15 @@
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.per-file-ignores]
 # F841 unused-variable: ignore since this file uses numexpr and many variables look unused
 "floris/simulation/wake_deflection/jimenez.py" = ["F841"]
 "floris/simulation/wake_velocity/jensen.py" = ["F841"]
 "floris/simulation/wake_velocity/gauss.py" = ["F841"]
+"floris/simulation/wake_velocity/empirical_gauss.py" = ["F841"]
 
 # I001 unsorted-imports: ignore because the import order is meaningful to navigate
 # import dependencies
 "floris/simulation/__init__.py" = ["I001"]
 
 # FIXME
 "floris/tools/interface_utilities.py" = ["F821"]
```

### Comparing `FLORIS-3.3/setup.py` & `FLORIS-3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -41,21 +41,25 @@
     "shapely",
 
     # utilities
     "coloredlogs>=10.0",
 ]
 
 # What packages are optional?
-# To use: pip install -e ".[develop]" or pip install "floris[develop]"
+# To use:
+#   pip install -e ".[docs,develop]"    install both sets of extras in editable install
+#   pip install -e ".[develop]"         installs only developer packages in editable install
+#   pip install "floris[develop]"       installs developer packages in non-editable install
 EXTRAS = {
     "docs": {
-        "jupyter-book",
+        "jupyter-book<=0.13.3",
         "sphinx-book-theme",
         "sphinx-autodoc-typehints",
         "sphinxcontrib-autoyaml",
+        "sphinxcontrib.mermaid",
     },
     "develop": {
         "pytest",
         "pre-commit",
         "ruff",
         "isort",
     },
```

