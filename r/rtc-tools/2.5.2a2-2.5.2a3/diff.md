# Comparing `tmp/rtc-tools-2.5.2a2.tar.gz` & `tmp/rtc-tools-2.5.2a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtc-tools-2.5.2a2.tar", last modified: Tue Mar 21 15:12:01 2023, max compression
+gzip compressed data, was "rtc-tools-2.5.2a3.tar", last modified: Tue May 16 09:48:45 2023, max compression
```

## Comparing `rtc-tools-2.5.2a2.tar` & `rtc-tools-2.5.2a3.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.323503 rtc-tools-2.5.2a2/
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/COPYING.LESSER
--rw-rw-rw-   0 root         (0) root         (0)       78 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1184 2023-03-21 15:12:01.323503 rtc-tools-2.5.2a2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      750 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/README.md
--rw-rw-rw-   0 root         (0) root         (0)      388 2023-03-21 15:12:01.324503 rtc-tools-2.5.2a2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2054 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.302502 rtc-tools-2.5.2a2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.307502 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1184 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2071 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      151 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      130 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-21 15:12:01.000000 rtc-tools-2.5.2a2/src/rtc_tools.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.324503 rtc-tools-2.5.2a2/src/rtctools/
--rw-rw-rw-   0 root         (0) root         (0)      106 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.310502 rtc-tools-2.5.2a2/src/rtctools/_internal/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/_internal/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5336 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/_internal/alias_tools.py
--rw-rw-rw-   0 root         (0) root         (0)      903 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/_internal/caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2243 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/_internal/casadi_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     1084 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/_internal/debug_check_helpers.py
--rw-r--r--   0 root         (0) root         (0)      499 2023-03-21 15:12:01.324503 rtc-tools-2.5.2a2/src/rtctools/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.313502 rtc-tools-2.5.2a2/src/rtctools/data/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4947 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/csv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.314503 rtc-tools-2.5.2a2/src/rtctools/data/interpolation/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/interpolation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline.py
--rw-rw-rw-   0 root         (0) root         (0)     6002 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1607 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline2d.py
--rw-rw-rw-   0 root         (0) root         (0)    18692 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/netcdf.py
--rw-rw-rw-   0 root         (0) root         (0)    42363 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/pi.py
--rw-rw-rw-   0 root         (0) root         (0)     8853 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/rtc.py
--rw-rw-rw-   0 root         (0) root         (0)    13011 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/data/storage.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.321503 rtc-tools-2.5.2a2/src/rtctools/optimization/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   116465 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/collocated_integrated_optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     9030 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/control_tree_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16651 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/csv_lookup_table_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11624 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    31616 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    39951 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/goal_programming_mixin_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6782 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/homotopy_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     3126 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/initial_state_estimation_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11817 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1019 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/linearization_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     8736 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    13293 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/min_abs_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    16202 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/modelica_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     7259 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/netcdf_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    43078 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/optimization_problem.py
--rw-rw-rw-   0 root         (0) root         (0)    10785 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    25126 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/single_pass_goal_programming_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     1753 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/optimization/timeseries.py
--rw-rw-rw-   0 root         (0) root         (0)     4193 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/rtctoolsapp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-21 15:12:01.323503 rtc-tools-2.5.2a2/src/rtctools/simulation/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/simulation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6606 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/simulation/csv_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     6163 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/simulation/io_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)     9048 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/simulation/pi_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    35345 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/simulation/simulation_problem.py
--rw-rw-rw-   0 root         (0) root         (0)     7371 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/src/rtctools/util.py
--rw-rw-rw-   0 root         (0) root         (0)    68611 2023-03-21 15:11:54.000000 rtc-tools-2.5.2a2/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.651263 rtc-tools-2.5.2a3/
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/COPYING.LESSER
+-rw-rw-rw-   0 root         (0) root         (0)       78 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-16 09:48:45.651263 rtc-tools-2.5.2a3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      750 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      388 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2016 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.629262 rtc-tools-2.5.2a3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.635262 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1184 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2071 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      151 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 09:48:45.000000 rtc-tools-2.5.2a3/src/rtc_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/src/rtctools/
+-rw-rw-rw-   0 root         (0) root         (0)      106 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.638262 rtc-tools-2.5.2a3/src/rtctools/_internal/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5336 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/alias_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)      903 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2243 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/casadi_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     1084 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/_internal/debug_check_helpers.py
+-rw-r--r--   0 root         (0) root         (0)      499 2023-05-16 09:48:45.652263 rtc-tools-2.5.2a3/src/rtctools/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.640262 rtc-tools-2.5.2a3/src/rtctools/data/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4947 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/csv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.642263 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5985 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1607 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline2d.py
+-rw-rw-rw-   0 root         (0) root         (0)    18692 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/netcdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    43530 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/pi.py
+-rw-rw-rw-   0 root         (0) root         (0)     8853 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/rtc.py
+-rw-rw-rw-   0 root         (0) root         (0)    13011 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/data/storage.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.649263 rtc-tools-2.5.2a3/src/rtctools/optimization/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   116480 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/collocated_integrated_optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     9026 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/control_tree_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16651 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/csv_lookup_table_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11624 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    31608 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    41999 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6782 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/homotopy_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     3126 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/initial_state_estimation_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11817 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1019 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/linearization_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8736 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    13293 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/min_abs_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    16198 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/modelica_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     7259 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/netcdf_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    43074 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/optimization_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)    10783 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    25126 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/single_pass_goal_programming_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     1753 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/optimization/timeseries.py
+-rw-rw-rw-   0 root         (0) root         (0)     4193 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/rtctoolsapp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 09:48:45.650263 rtc-tools-2.5.2a3/src/rtctools/simulation/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6606 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/csv_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     6163 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/io_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)     8922 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/pi_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    35341 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/simulation/simulation_problem.py
+-rw-rw-rw-   0 root         (0) root         (0)     7371 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/src/rtctools/util.py
+-rw-rw-rw-   0 root         (0) root         (0)    68611 2023-05-16 09:48:39.000000 rtc-tools-2.5.2a3/versioneer.py
```

### Comparing `rtc-tools-2.5.2a2/COPYING.LESSER` & `rtc-tools-2.5.2a3/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/PKG-INFO` & `rtc-tools-2.5.2a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a2
+Version: 2.5.2a3
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a2/README.md` & `rtc-tools-2.5.2a3/README.md`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/setup.py` & `rtc-tools-2.5.2a3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,38 +25,38 @@
 Operating System :: Microsoft :: Windows
 Operating System :: POSIX
 Operating System :: Unix
 Operating System :: MacOS
 """
 
 setup(
-    name = 'rtc-tools',
-    version = versioneer.get_version(),
-    maintainer = 'Deltares',
-    author = 'Deltares',
-    description = DOCLINES[0],
-    long_description = '\n'.join(DOCLINES[2:]),
-    url = 'https://oss.deltares.nl/web/rtc-tools/home',
+    name='rtc-tools',
+    version=versioneer.get_version(),
+    maintainer='Deltares',
+    author='Deltares',
+    description=DOCLINES[0],
+    long_description='\n'.join(DOCLINES[2:]),
+    url='https://oss.deltares.nl/web/rtc-tools/home',
     download_url='http://gitlab.com/deltares/rtc-tools/',
-    classifiers = [_f for _f in CLASSIFIERS.split('\n') if _f],
-    platforms = ['Windows', 'Linux', 'Mac OS-X', 'Unix'],
-    packages = find_packages("src"),
-    package_dir = {"": "src"},
-    install_requires = ["casadi == 3.5.*",
-                        "numpy >= 1.16.0, <1.23",
-                        "scipy >= 1.0.0, <1.11",
-                        "pymoca == 0.9.*",
-                        "rtc-tools-channel-flow >= 1.1.0"],
-    tests_require = ['pytest', 'pytest-runner'],
-    extras_require = {
+    classifiers=[_f for _f in CLASSIFIERS.split('\n') if _f],
+    platforms=['Windows', 'Linux', 'Mac OS-X', 'Unix'],
+    packages=find_packages("src"),
+    package_dir={"": "src"},
+    install_requires=["casadi == 3.5.*",
+                      "numpy >= 1.16.0, <1.23",
+                      "scipy >= 1.0.0, <1.11",
+                      "pymoca == 0.9.*",
+                      "rtc-tools-channel-flow >= 1.1.0"],
+    tests_require=['pytest', 'pytest-runner'],
+    extras_require={
         'netcdf':  ["netCDF4"],
         'all': ["netCDF4"],
     },
     python_requires='>=3.5',
-    cmdclass = versioneer.get_cmdclass(),
+    cmdclass=versioneer.get_cmdclass(),
     entry_points={
         'console_scripts': [
             'rtc-tools-download-examples = rtctools.rtctoolsapp:download_examples',
             'rtc-tools-copy-libraries = rtctools.rtctoolsapp:copy_libraries',
         ]
     },
 )
```

### Comparing `rtc-tools-2.5.2a2/src/rtc_tools.egg-info/PKG-INFO` & `rtc-tools-2.5.2a3/src/rtc_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rtc-tools
-Version: 2.5.2a2
+Version: 2.5.2a3
 Summary: Toolbox for control and optimization of water systems.
 Home-page: https://oss.deltares.nl/web/rtc-tools/home
 Author: Deltares
 Maintainer: Deltares
 License: UNKNOWN
 Download-URL: http://gitlab.com/deltares/rtc-tools/
 Platform: Windows
```

### Comparing `rtc-tools-2.5.2a2/src/rtc_tools.egg-info/SOURCES.txt` & `rtc-tools-2.5.2a3/src/rtc_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/_internal/alias_tools.py` & `rtc-tools-2.5.2a3/src/rtctools/_internal/alias_tools.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/_internal/caching.py` & `rtc-tools-2.5.2a3/src/rtctools/_internal/caching.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/_internal/casadi_helpers.py` & `rtc-tools-2.5.2a3/src/rtctools/_internal/casadi_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/_internal/debug_check_helpers.py` & `rtc-tools-2.5.2a3/src/rtctools/_internal/debug_check_helpers.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/csv.py` & `rtc-tools-2.5.2a3/src/rtctools/data/csv.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline.py` & `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline1d.py` & `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         H = jacobian(J, x_sym)
         bspline_prime_prime = Function('bspline_prime_prime', free_vars, [H])
 
         # Objective Function
         xpt = SX.sym('xpt')
         ypt = SX.sym('ypt')
         sq_diff = Function('sq_diff', [xpt, ypt], [
-                             (ypt - bspline(c, xpt))**2])
+            (ypt - bspline(c, xpt))**2])
         sq_diff = sq_diff.map(N, 'serial')
         f = sum2(sq_diff(SX(x), SX(y)))
 
         # Setup Curvature Constraints
         delta_c_max = np.full(num_knots - 1, inf)
         delta_c_min = np.full(num_knots - 1, -inf)
         max_slope_slope = np.full(num_test_points, inf)
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/interpolation/bspline2d.py` & `rtc-tools-2.5.2a3/src/rtctools/data/interpolation/bspline2d.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/netcdf.py` & `rtc-tools-2.5.2a3/src/rtctools/data/netcdf.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/pi.py` & `rtc-tools-2.5.2a3/src/rtctools/data/pi.py`

 * *Files 5% similar despite different names*

```diff
@@ -828,16 +828,48 @@
 
                 # Restore NaN
                 values[nans] = np.nan
 
         if self.__binary:
             f.close()
 
+        self.format_xml_data()
         self.__tree.write(self.__path_xml)
 
+    def format_xml_data(self):
+        """
+        Format the XML data
+
+        Make sure it has proper indentation and newlines.
+        """
+        self.format_xml_element(self.__xml_root)
+
+    @staticmethod
+    def format_xml_element(element: ET.Element, level=0):
+        """
+        Format an XML element
+
+        Make sure it has proper indentation and newlines.
+        This code is based on
+        https://stackoverflow.com/questions/3095434/inserting-newlines-in-xml-file-generated-via-xml-etree-elementtree-in-python
+        """
+        indent = "\n" + level*"  "
+        if len(element):
+            if not element.text or not element.text.strip():
+                element.text = indent + "  "
+            if not element.tail or not element.tail.strip():
+                element.tail = indent
+            for subelement in element:
+                Timeseries.format_xml_element(subelement, level+1)
+            if not element.tail or not element.tail.strip():
+                element.tail = indent
+        else:
+            if level and (not element.tail or not element.tail.strip()):
+                element.tail = indent
+
     @property
     def contains_ensemble(self):
         """
         Flag to indicate TimeSeries contains an ensemble.
         """
         return self.__contains_ensemble
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/rtc.py` & `rtc-tools-2.5.2a3/src/rtctools/data/rtc.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/data/storage.py` & `rtc-tools-2.5.2a3/src/rtctools/data/storage.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/collocated_integrated_optimization_problem.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/collocated_integrated_optimization_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -709,21 +709,21 @@
 
                 dae_residual_function_integrated = ca.Function(
                     'dae_residual_function_integrated',
                     [I,
                      I0,
                      symbolic_parameters,
                      ca.vertcat(*(
-                        [C0[i] for i in range(len(collocated_variables))] +
-                        [CI0[i] for i in range(len(self.dae_variables['constant_inputs']))] +
-                        [dt_sym] +
-                        collocated_variables +
-                        collocated_derivatives +
-                        self.dae_variables['constant_inputs'] +
-                        self.dae_variables['time']))],
+                         [C0[i] for i in range(len(collocated_variables))] +
+                         [CI0[i] for i in range(len(self.dae_variables['constant_inputs']))] +
+                         [dt_sym] +
+                         collocated_variables +
+                         collocated_derivatives +
+                         self.dae_variables['constant_inputs'] +
+                         self.dae_variables['time']))],
                     [dae_residual_integrated],
                     function_options)
 
                 # if not self.dae_is_external_function:
                 try:
                     dae_residual_function_integrated = dae_residual_function_integrated.expand()
                 except RuntimeError as e:
@@ -739,20 +739,20 @@
 
             # Initialize a Function for the DAE residual (collocated part)
             if len(collocated_variables) > 0:
                 self.__dae_residual_function_collocated = ca.Function(
                     'dae_residual_function_collocated',
                     [symbolic_parameters,
                      ca.vertcat(*(
-                        integrated_variables +
-                        collocated_variables +
-                        integrated_derivatives +
-                        collocated_derivatives +
-                        self.dae_variables['constant_inputs'] +
-                        self.dae_variables['time']))],
+                         integrated_variables +
+                         collocated_variables +
+                         integrated_derivatives +
+                         collocated_derivatives +
+                         self.dae_variables['constant_inputs'] +
+                         self.dae_variables['time']))],
                     [dae_residual_collocated],
                     function_options)
                 try:
                     self.__dae_residual_function_collocated = self.__dae_residual_function_collocated.expand()
                 except RuntimeError as e:
                     # We only expect to fail if the DAE was an external function
                     if "'eval_sx' not defined for External" in str(e):
@@ -856,21 +856,21 @@
             # The first argument is the guess for the new value of
             # integrated_states.
             [integrated_states_1] = integrator_step_function.call(
                 [integrated_states_0,
                  integrated_states_0,
                  symbolic_parameters,
                  ca.vertcat(
-                    collocated_states_0,
-                    constant_inputs_0,
-                    dt,
-                    collocated_states_1,
-                    collocated_finite_differences,
-                    constant_inputs_1,
-                    collocation_time_1 - t0)],
+                     collocated_states_0,
+                     constant_inputs_0,
+                     dt,
+                     collocated_states_1,
+                     collocated_finite_differences,
+                     constant_inputs_1,
+                     collocation_time_1 - t0)],
                 False, True)
             accumulated_Y.append(integrated_states_1)
 
             # Recompute finite differences with computed new state, for use in the collocation part below
             # We don't use substititute() for this, as it becomes expensive
             # over long integration horizons.
             if len(collocated_variables) > 0:
@@ -884,32 +884,32 @@
         # specifications, version 3.3.
         if len(collocated_variables) > 0:
             if theta < 1:
                 # Obtain state vector
                 [dae_residual_0] = dae_residual_function_collocated.call(
                     [symbolic_parameters,
                      ca.vertcat(
-                        integrated_states_0,
-                        collocated_states_0,
-                        integrated_finite_differences,
-                        collocated_finite_differences,
-                        constant_inputs_0,
-                        collocation_time_0 - t0)],
+                         integrated_states_0,
+                         collocated_states_0,
+                         integrated_finite_differences,
+                         collocated_finite_differences,
+                         constant_inputs_0,
+                         collocation_time_0 - t0)],
                     False, True)
             if theta > 0:
                 # Obtain state vector
                 [dae_residual_1] = dae_residual_function_collocated.call(
                     [symbolic_parameters,
                      ca.vertcat(
-                        integrated_states_1,
-                        collocated_states_1,
-                        integrated_finite_differences,
-                        collocated_finite_differences,
-                        constant_inputs_1,
-                        collocation_time_1 - t0)],
+                         integrated_states_1,
+                         collocated_states_1,
+                         integrated_finite_differences,
+                         collocated_finite_differences,
+                         constant_inputs_1,
+                         collocation_time_1 - t0)],
                     False, True)
             if theta == 0:
                 accumulated_Y.append(dae_residual_0)
             elif theta == 1:
                 accumulated_Y.append(dae_residual_1)
             else:
                 accumulated_Y.append(
@@ -969,33 +969,33 @@
 
         # Add constraints for initial conditions
         if self.__initial_residual_with_params_fun_map is None:
             initial_residual_with_params_fun = ca.Function(
                 'initial_residual_total',
                 [symbolic_parameters,
                  ca.vertcat(*(
-                    self.dae_variables['states'] +
-                    self.dae_variables['algebraics'] +
-                    self.dae_variables['control_inputs'] +
-                    integrated_derivatives +
-                    collocated_derivatives +
-                    self.dae_variables['constant_inputs'] +
-                    self.dae_variables['time']))],
+                     self.dae_variables['states'] +
+                     self.dae_variables['algebraics'] +
+                     self.dae_variables['control_inputs'] +
+                     integrated_derivatives +
+                     collocated_derivatives +
+                     self.dae_variables['constant_inputs'] +
+                     self.dae_variables['time']))],
                 [ca.veccat(dae_residual, initial_residual)],
                 function_options)
             self.__initial_residual_with_params_fun_map = initial_residual_with_params_fun.map(
                 self.ensemble_size)
         initial_residual_with_params_fun_map = self.__initial_residual_with_params_fun_map
         [res] = initial_residual_with_params_fun_map.call(
             [ensemble_aggregate["parameters"],
              ca.vertcat(*[
-                ensemble_aggregate["initial_state"],
-                ensemble_aggregate["initial_derivatives"],
-                ensemble_aggregate["initial_constant_inputs"],
-                ca.repmat([0.0], 1, self.ensemble_size)])],
+                 ensemble_aggregate["initial_state"],
+                 ensemble_aggregate["initial_derivatives"],
+                 ensemble_aggregate["initial_constant_inputs"],
+                 ca.repmat([0.0], 1, self.ensemble_size)])],
             False, True)
 
         res = ca.vec(res)
         g.append(res)
         zeros = [0.0] * res.size1()
         lbg.extend(zeros)
         ubg.extend(zeros)
@@ -1211,17 +1211,17 @@
 
             # Save these inputs such that can be used later in map_path_expression()
             self.__func_mapped_inputs.append(
                 (accumulation_X0, accumulation_U,
                  ca.repmat(ca.vertcat(parameters, extra_variables), 1, n_collocation_times - 1)))
 
             self.__func_initial_inputs.append([parameters, ca.vertcat(
-                        initial_state, initial_derivatives, initial_constant_inputs, 0.0,
-                        initial_path_variables, initial_extra_constant_inputs),
-                        extra_variables])
+                initial_state, initial_derivatives, initial_constant_inputs, 0.0,
+                initial_path_variables, initial_extra_constant_inputs),
+                extra_variables])
 
             integrators_and_collocation_and_path_constraints = accumulation(
                 *self.__func_mapped_inputs[ensemble_member])
 
             if len(integrated_variables) > 0:
                 integrators = integrators_and_collocation_and_path_constraints[0]
                 integrators_and_collocation_and_path_constraints = integrators_and_collocation_and_path_constraints[1]
@@ -1363,15 +1363,15 @@
                     [ca.vertcat(parameters)])
 
                 # Use mapped function to evaluate delay in terms of constant inputs
                 mapped_delay_function = ca.Function(
                     'delay_values',
                     self.dae_variables['time'] + self.dae_variables['constant_inputs'],
                     substituted_delay_durations
-                    ).map(len(collocation_times))
+                ).map(len(collocation_times))
 
                 # Call mapped delay function with inputs as arrays
                 evaluated_delay_durations = mapped_delay_function.call(
                     [collocation_times] +
                     [constant_inputs[v.name()] for v in self.dae_variables['constant_inputs']])
 
                 for i in range(len(delayed_feedback_expressions)):
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/control_tree_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/control_tree_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
 
                     # We select the scenario with the max min distance to the other branches
                     min_distances = np.array([
                         min([np.inf] + [distances[j, k]
                             for j, member_j in enumerate(branches[current_branch])
                             if member_j not in available and member_k in available])
                         for k, member_k in enumerate(branches[current_branch])
-                        ], dtype=np.float64)
+                    ], dtype=np.float64)
                     min_distances[np.where(min_distances == np.inf)] = -np.inf
 
                     idx = np.argmax(min_distances)
                     if min_distances[idx] <= 0:
                         idx = -1
                 else:
                     branches[current_branch + (i, )] = []
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/csv_lookup_table_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/csv_lookup_table_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/csv_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/goal_programming_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -418,15 +418,15 @@
             goal_functions = OrderedDict()
 
             for j, goal in enumerate(goals):
                 if (
                         not goal.has_target_bounds or
                         goal.violation_timeseries_id is not None or
                         goal.function_value_timeseries_id is not None
-                        ):
+                ):
                     goal_functions[j] = goal.function(self, ensemble_member)
 
             if is_path_goal:
                 expr = self.map_path_expression(
                     ca.vertcat(*goal_functions.values()), ensemble_member
                 )
             else:
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/goal_programming_mixin_base.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/goal_programming_mixin_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,93 +35,160 @@
         return OrderedDict()
 
 
 class Goal(metaclass=ABCMeta):
     r"""
     Base class for lexicographic goal programming goals.
 
-    A goal is defined by overriding the :func:`function` method.
+    **Types of goals**
 
-    :cvar function_range:   Range of goal function.  *Required if a target is set*.
-    :cvar function_nominal: Nominal value of function. Used for scaling.  Default is ``1``.
-    :cvar target_min:       Desired lower bound for goal function.  Default is ``numpy.nan``.
-    :cvar target_max:       Desired upper bound for goal function.  Default is ``numpy.nan``.
-    :cvar priority:         Integer priority of goal.  Default is ``1``.
-    :cvar weight:           Optional weighting applied to the goal.  Default is ``1.0``.
-    :cvar order:            Penalization order of goal violation.  Default is ``2``.
-    :cvar critical:         If ``True``, the algorithm will abort if this goal cannot be fully met.
-                            Default is ``False``.
-    :cvar relaxation:       Amount of slack added to the hard constraints related to the goal.
-                            Must be a nonnegative value. Default is ``0.0``.
+    There are 2 types of goals: minimization goals and target goals.
+
+    *Minimization goals*
+
+    Minimization goals are of the form:
+
+    .. math::
+        \text{minimize } f(x).
 
-    The target bounds indicate the range within the function should stay, *if possible*.  Goals
-    are, in that sense, *soft*, as opposed to standard hard constraints.
+    *Target goals*
 
-    Four types of goals can be created:
+    Target goals weakly enforce a constraint of the form
 
-    1. Minimization goal if no target bounds are set:
+    .. math::
+        m_{target} \leq g(x) \leq M_{target},
 
-       .. math::
+    by turning it into a minimization problem of the form
 
-            \min f
+    .. math::
+        \text{minimize } & \epsilon^r, \\
+        \text{subject to } &g_{low}(\epsilon) \leq g(x) \leq g_{up}(\epsilon), \\
+        \text{and } &0 \leq \epsilon \leq 1,
 
-    2. Lower bound goal if ``target_min`` is set:
+    where
 
-        .. math::
+    .. math::
+        g_{low}(\epsilon) &:= (1-\epsilon) m_{target} + \epsilon m, \\
+        g_{up}(\epsilon) &:= (1-\epsilon) M_{target} + \epsilon M.
 
-            m \leq f
+    Here, :math:`m` and :math:`M` are hard constraints for :math:`g(x)`,
+    :math:`m_{target}` and :math:`M_{target}` are target bounds for :math:`g(x)`,
+    :math:`\epsilon` is an auxiliary variable
+    that indicates how strongly the target bounds are violated,
+    and :math:`\epsilon^r` is a function that indicates the variation of :math:`\epsilon`,
+    where the order :math:`r` is by default :math:`2`.
+    We have
 
-    3. Upper bound goal if ``target_max`` is set:
+    .. math::
+        m < m_{target} \leq M_{target} < M.
 
-        .. math::
+    Note that when :math:`\epsilon=0`,
+    the constraint on :math:`g(x)` becomes
 
-            f \leq M
+    .. math::
+        m_{target} \leq g(x) \leq M_{target}
 
-    4. Combined lower and upper bound goal if ``target_min`` and ``target_max`` are both set:
+    and if :math:`\epsilon=1`, it becomes
 
-        .. math::
+    .. math::
+        m \leq g(x) \leq M.
 
-            m \leq f \leq M
 
-    Lower priority goals take precedence over higher priority goals.
+    **Scaling goals**
 
-    Goals with the same priority are weighted off against each other in a single objective function.
+    Goals can be scaled by a nominal value :math:`c_{nom}`
+    to improve the performance of the solvers.
+    In case of a minimization goal, the scaled problem is given by
 
-    In goals where a target is set:
-        * The function range interval must be provided as this is used to introduce hard constrains on the value that
-          the function can take. If one is unsure about which value the function can take, it is recommended to
-          overestimate this interval. However, an overestimated interval will negatively influence how accurately the
-          target bounds are met.
-        * The target provided must be contained in the function range.
-        * The function nominal is used to scale the constraints.
-        * If both a target_min and a target_max are set, the target maximum must be at least equal to minimum one.
-        * In a path goal, the target can be a Timeseries.
+    .. math::
+        \text{minimize } \hat{f}(x),
 
-    In minimization goals:
-        * The function range is not used and therefore cannot be set.
-        * The function nominal is used to scale the function value in the objective function. To ensure that all goals
-          are given a similar importance, it is crucial to provide an accurate estimate of this parameter.
+    where :math:`\hat{f}(x) := f(x) / c_{nom}`.
+    In case of a target goal, the scaled problem is given by
 
-    The goal violation value is taken to the order'th power in the objective function of the final
-    optimization problem.
+    .. math::
+        \text{minimize } & \epsilon^r, \\
+        \text{subject to } &\hat{g}_{low}(\epsilon) \leq \hat{g}(x) \leq \hat{g}_{up}(\epsilon), \\
+        \text{and } &0 \leq \epsilon \leq 1,
 
-    Relaxation is used to loosen the constraints that are set after the
-    optimization of the goal's priority. The unit of the relaxation is equal
-    to that of the goal function.
+    where :math:`\hat{g}(x) := g(x) / c_{nom}`,
+    :math:`\hat{g}_{low}(\epsilon) := {g}_{low}(\epsilon) / c_{nom}`,
+    and :math:`\hat{g}_{up}(\epsilon) := {g}_{up}(\epsilon) / c_{nom}`.
+
+
+    **Implementing goals**
+
+    A goal class is created by inheriting from the :py:class:Goal class and
+    overriding the :func:`function` method.
+    This method defines the goal function :math:`f(x)` in case of a minimization goal,
+    and the goal function :math:`g(x)` in case of a target goal.
+    A goal becomes a target goal
+    if either the class attribute ``target_min`` or ``target_max`` is set.
+
+    To further define a goal, the following class attributes can also be set.
+
+    :cvar function_range:   Range of goal function :math:`[m ,M]`.
+                            Only applies to target goals.
+                            Required for a target goal.
+    :cvar function_nominal: Nominal value of a function :math:`c_{nom}`.
+                            Used for scaling. Default is ``1``.
+    :cvar target_min:       Desired lower bound for goal function :math:`m_{target}`.
+                            Default is ``numpy.nan``.
+    :cvar target_max:       Desired upper bound for goal function :math:`M_{target}`.
+                            Default is ``numpy.nan``.
+    :cvar priority:         Priority of a goal. Default is ``1``.
+    :cvar weight:           Optional weighting applied to the goal. Default is ``1.0``.
+    :cvar order:            Penalization order of goal violation :math:`r`. Default is ``2``.
+    :cvar critical:         If ``True``, the algorithm will abort if this goal cannot be fully met.
+                            Default is ``False``.
+    :cvar relaxation:       Amount of slack added to the hard constraints related to the goal.
+                            Must be a nonnegative value.
+                            The unit is equal to that of the goal function.
+                            Default is ``0.0``.
+
+    When ``target_min`` is set, but not ``target_max``,
+    the target goal becomes a lower bound target goal
+    and the constraint on :math:`g(x)` becomes
+
+    .. math::
+        g_{low}(\epsilon) \leq g(x).
+
+    Similary, if ``target_max`` is set, but not ``target_min``,
+    the target goal becomes a upper bound target goal
+    and the constraint on :math:`g(x)` becomes
+
+    .. math::
+        g(x) \leq g_{up}(\epsilon).
+
+    Relaxation is used to loosen the constraints that are set
+    after the optimization of the goal's priority.
+
+    Notes:
+        *   If one is unsure about the function range,
+            it is recommended to overestimate this interval.
+            However, this will negatively influence how accurately the target bounds are met.
+        *   The function range should be strictly larger than the target range.
+            In particular, :math:`m < m_{target}` and :math:`M_{target} < M`.
+        *   In a path goal, the target can be a Timeseries.
+        *   In case of multiple goals with the same priority,
+            it is crucial that an accurate function nominal value is provided.
+            This ensures that all goals are given similar importance.
 
     A goal can be written in vector form. In a vector goal:
         * The goal size determines how many goals there are.
         * The goal function has shape ``(goal size, 1)``.
         * The function is either minimized or has, possibly various, targets.
         * Function nominal can either be an array with as many entries as the goal size or have a single value.
         * Function ranges can either be an array with as many entries as the goal size or have a single value.
         * In a goal, the target can either be an array with as many entries as the goal size or have a single value.
         * In a path goal, the target can also be a Timeseries whose values are either a 1-dimensional vector or have
           as many columns as the goal size.
 
+    **Examples**
+
     Example definition of the point goal :math:`x(t) \geq 1.1` for :math:`t=1.0` at priority 1::
 
         class MyGoal(Goal):
             def function(self, optimization_problem, ensemble_member):
                 # State 'x' at time t = 1.0
                 t = 1.0
                 return optimization_problem.state_at('x', t, ensemble_member)
@@ -137,14 +204,16 @@
                 # State 'x' at any point in time
                 return optimization_problem.state('x')
 
             function_range = (1.0, 2.0)
             target_min = 1.1
             priority = 2
 
+    **Note path goals**
+
     Note that for path goals, the ensemble member index is not passed to the call
     to :func:`OptimizationProblem.state`.  This call returns a time-independent symbol
     that is also independent of the active ensemble member.  Path goals are
     applied to all times and all ensemble members simultaneously.
 
     """
 
@@ -406,15 +475,15 @@
             self.max = max_
 
 
 class _GoalProgrammingMixinBase(OptimizationProblem, metaclass=ABCMeta):
 
     def _gp_n_objectives(self, subproblem_objectives, subproblem_path_objectives, ensemble_member):
         return ca.vertcat(*[o(self, ensemble_member) for o in subproblem_objectives]).size1() \
-               + ca.vertcat(*[o(self, ensemble_member) for o in subproblem_path_objectives]).size1()
+            + ca.vertcat(*[o(self, ensemble_member) for o in subproblem_path_objectives]).size1()
 
     def _gp_objective(self, subproblem_objectives, n_objectives, ensemble_member):
         if len(subproblem_objectives) > 0:
             acc_objective = ca.sum1(ca.vertcat(*[o(self, ensemble_member) for o in subproblem_objectives]))
 
             if self.goal_programming_options()['scale_by_problem_size']:
                 acc_objective = acc_objective / n_objectives
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/homotopy_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/homotopy_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/initial_state_estimation_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/initial_state_estimation_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/io_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/linearization_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/linearization_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/linearized_order_goal_programming_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/linearized_order_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/min_abs_goal_programming_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/min_abs_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/modelica_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/modelica_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 else:
                     self.__mx['control_inputs'].append(v.symbol)
 
         # Initialize nominals and types
         # These are not in @cached dictionary properties for backwards compatibility.
         self.__python_types = AliasDict(self.alias_relation)
         for v in itertools.chain(
-                    self.__pymoca_model.states, self.__pymoca_model.alg_states, self.__pymoca_model.inputs):
+                self.__pymoca_model.states, self.__pymoca_model.alg_states, self.__pymoca_model.inputs):
             self.__python_types[v.symbol.name()] = v.python_type
 
         # Initialize dae, initial residuals, as well as delay arguments
         # These are not in @cached dictionary properties so that we need to create the list
         # of function arguments only once.
         variable_lists = ['states', 'der_states', 'alg_states', 'inputs', 'constants', 'parameters']
         function_arguments = [self.__pymoca_model.time] + [
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/netcdf_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/netcdf_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/optimization_problem.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/optimization_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                     loop_error = self.loop_over_error[ii][2]
                     if loop_error_indicator and loop_error in return_status:
                         log_level = logging.INFO
                 except IndexError:
                     if loop_error_indicator:
                         log_level = logging.INFO
                 logger.log(log_level, "Solver succeeded with status {} ({}).".format(
-                        return_status, wall_clock_time))
+                    return_status, wall_clock_time))
             except (AttributeError, ValueError):
                 logger.log(log_level, "Solver succeeded with status {} ({}).".format(
                     return_status, wall_clock_time))
 
         # Do any postprocessing
         if postprocessing:
             self.post()
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/pi_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/pi_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     self._input_folder, pi_parameter_config_basename))
         except IOError:
             raise Exception(
                 "PIMixin: {}.xml not found in {}.".format(pi_parameter_config_basename, self._input_folder))
 
         try:
             self.__parameter_config_numerical = pi.ParameterConfig(
-                  self._input_folder, self.pi_parameter_config_numerical_basename)
+                self._input_folder, self.pi_parameter_config_numerical_basename)
         except IOError:
             self.__parameter_config_numerical = None
 
         try:
             self.__timeseries_import = pi.Timeseries(
                 self.__data_config, self._input_folder, self.timeseries_import_basename,
                 binary=self.pi_binary_timeseries, pi_validate_times=self.pi_validate_timeseries)
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/single_pass_goal_programming_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/single_pass_goal_programming_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/optimization/timeseries.py` & `rtc-tools-2.5.2a3/src/rtctools/optimization/timeseries.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/rtctoolsapp.py` & `rtc-tools-2.5.2a3/src/rtctools/rtctoolsapp.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/simulation/csv_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/simulation/csv_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/simulation/io_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/simulation/io_mixin.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/src/rtctools/simulation/pi_mixin.py` & `rtc-tools-2.5.2a3/src/rtctools/simulation/pi_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,27 +139,26 @@
         # Write the ensemble properties for the export file.
         self.__timeseries_export.ensemble_size = 1
         self.__timeseries_export.contains_ensemble = self.__timeseries_import.contains_ensemble
 
         # For all variables that are output variables the values are
         # extracted from the results.
         for variable in self._io_output_variables:
-            for alias in self.alias_relation.aliases(variable):
-                values = np.array(self._io_output[alias])
-                # Check if ID mapping is present
-                try:
-                    self.__data_config.pi_variable_ids(alias)
-                    # Add series to output file
-                    self.__timeseries_export.set(alias, values, unit=self.__timeseries_import.get_unit(alias))
-                    break
-                except KeyError:
-                    logger.debug(
-                        'PIMixin: variable {} has no mapping defined in rtcDataConfig '
-                        'so cannot be added to the output file.'.format(alias))
-                    continue
+            values = np.array(self._io_output[variable])
+            # Check if ID mapping is present
+            try:
+                self.__data_config.pi_variable_ids(variable)
+            except KeyError:
+                logger.debug(
+                    'PIMixin: variable {} has no mapping defined in rtcDataConfig '
+                    'so cannot be added to the output file.'.format(variable))
+                continue
+
+            # Add series to output file
+            self.__timeseries_export.set(variable, values, unit=self.__timeseries_import.get_unit(variable))
 
         # Write output file to disk
         self.__timeseries_export.write()
 
     @property
     def timeseries_import(self):
         """
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/simulation/simulation_problem.py` & `rtc-tools-2.5.2a3/src/rtctools/simulation/simulation_problem.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
                 'Simulation has failed to converge at time {}. Solver failed with status {}'.format(
                     self.get_current_time(), rootfinder_stats['nlpsol']['return_status']))
 
         if logger.getEffectiveLevel() == logging.DEBUG:
             # compute max residual
             largest_res = ca.norm_inf(
                 self.__res_vals(next_state, self.__dt, self.__state_vector[:-len(self.__mx['parameters'])])
-                )
+            )
             logger.debug('Residual maximum magnitude: {:.2E}'.format(float(largest_res)))
 
         # Update state vector
         self.__state_vector[:self.__states_end_index] = next_state.toarray().ravel()
 
     def simulate(self):
         """
```

### Comparing `rtc-tools-2.5.2a2/src/rtctools/util.py` & `rtc-tools-2.5.2a3/src/rtctools/util.py`

 * *Files identical despite different names*

### Comparing `rtc-tools-2.5.2a2/versioneer.py` & `rtc-tools-2.5.2a3/versioneer.py`

 * *Files identical despite different names*

