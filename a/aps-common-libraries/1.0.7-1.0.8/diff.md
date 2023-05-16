# Comparing `tmp/aps_common_libraries-1.0.7.tar.gz` & `tmp/aps_common_libraries-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aps_common_libraries-1.0.7.tar", last modified: Wed May 10 14:45:01 2023, max compression
+gzip compressed data, was "aps_common_libraries-1.0.8.tar", last modified: Tue May 16 12:16:43 2023, max compression
```

## Comparing `aps_common_libraries-1.0.7.tar` & `aps_common_libraries-1.0.8.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.275115 aps_common_libraries-1.0.7/
--rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.7/LICENSE
--rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.7/LICENSE.pdf
--rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.7/MANIFEST.in
--rw-r--r--   0 bishop    (1601)      907      876 2023-05-10 14:45:01.274427 aps_common_libraries-1.0.7/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.7/README.md
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.200554 aps_common_libraries-1.0.7/aps/
--rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.7/aps/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.209685 aps_common_libraries-1.0.7/aps/common/
--rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.7/aps/common/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.214222 aps_common_libraries-1.0.7/aps/common/__test/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.7/aps/common/__test/__init__.py
--rw-r--r--   0 bishop    (1601)      907     3683 2023-05-05 00:42:24.000000 aps_common_libraries-1.0.7/aps/common/__test/singletons.py
--rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.7/aps/common/__test/test.py
--rw-r--r--   0 bishop    (1601)      907     5739 2023-05-05 00:41:47.000000 aps_common_libraries-1.0.7/aps/common/__test/test2.py
--rw-rw-rw-   0 bishop    (1601)      907    10116 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.7/aps/common/initializer.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.219193 aps_common_libraries-1.0.7/aps/common/io/
--rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.7/aps/common/io/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.7/aps/common/io/printout.py
--rw-r--r--   0 bishop    (1601)      907     3693 2023-05-04 23:44:10.000000 aps_common_libraries-1.0.7/aps/common/io/sys_commands.py
--rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.7/aps/common/io/tcp_client.py
--rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.7/aps/common/io/tiff_file.py
--rw-rw-rw-   0 bishop    (1601)      907    20774 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.7/aps/common/logger.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.220355 aps_common_libraries-1.0.7/aps/common/measurment/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.7/aps/common/measurment/__init__.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.224010 aps_common_libraries-1.0.7/aps/common/measurment/beamline/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/__init__.py
--rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/image_collector.py
--rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/image_processor.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.247263 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/
--rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/SPINNet_estimate.py
--rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/WXST.py
--rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/diffraction_process.py
--rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/euclidean_dist.py
--rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/func.py
--rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/func_light.py
--rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/gui_func.py
--rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/integration.py
--rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/main.py
--rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/pattern_find.py
--rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/pattern_propagate.py
--rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/utils.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.250256 aps_common_libraries-1.0.7/aps/common/ml/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.7/aps/common/ml/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.7/aps/common/ml/data_structures.py
--rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.7/aps/common/ml/mocks.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.254809 aps_common_libraries-1.0.7/aps/common/plot/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.7/aps/common/plot/__init__.py
--rw-r--r--   0 bishop    (1601)      907    45238 2023-05-10 12:48:38.000000 aps_common_libraries-1.0.7/aps/common/plot/gui.py
--rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.7/aps/common/plot/image.py
--rw-rw-rw-   0 bishop    (1601)      907     6365 2023-02-16 16:28:45.000000 aps_common_libraries-1.0.7/aps/common/plot/qt_application.py
--rw-rw-rw-   0 bishop    (1601)      907    16735 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.7/aps/common/plotter.py
--rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.7/aps/common/reflection.py
--rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.7/aps/common/registry.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.261518 aps_common_libraries-1.0.7/aps/common/scripts/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.7/aps/common/scripts/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.7/aps/common/scripts/abstract_command_line_script.py
--rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.7/aps/common/scripts/generic_process_manager.py
--rw-rw-rw-   0 bishop    (1601)      907     8024 2023-05-10 00:09:44.000000 aps_common_libraries-1.0.7/aps/common/scripts/generic_qt_script.py
--rw-rw-rw-   0 bishop    (1601)      907     4357 2023-05-10 14:40:34.000000 aps_common_libraries-1.0.7/aps/common/scripts/script_data.py
--rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.7/aps/common/scripts/script_registry.py
--rw-rw-rw-   0 bishop    (1601)      907     4677 2023-05-05 00:43:28.000000 aps_common_libraries-1.0.7/aps/common/singleton.py
--rw-rw-rw-   0 bishop    (1601)      907    10093 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.7/aps/common/traffic_light.py
--rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.7/aps/common/utilities.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.266831 aps_common_libraries-1.0.7/aps/common/widgets/
--rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.7/aps/common/widgets/__init__.py
--rw-rw-rw-   0 bishop    (1601)      907     4081 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.7/aps/common/widgets/close_app_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.7/aps/common/widgets/context_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.7/aps/common/widgets/generic_widget.py
--rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.7/aps/common/widgets/log_stream_widget.py
-drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-10 14:45:01.273192 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/
--rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-10 14:45:00.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/PKG-INFO
--rw-rw-rw-   0 bishop    (1601)      907     2268 2023-05-10 14:45:01.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/SOURCES.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-10 14:45:00.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/dependency_links.txt
--rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-10 14:45:00.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/namespace_packages.txt
--rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/not-zip-safe
--rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-10 14:45:00.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/requires.txt
--rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-10 14:45:00.000000 aps_common_libraries-1.0.7/aps_common_libraries.egg-info/top_level.txt
--rw-r--r--   0 bishop    (1601)      907       38 2023-05-10 14:45:01.275415 aps_common_libraries-1.0.7/setup.cfg
--rw-r--r--   0 bishop    (1601)      907     5571 2023-05-10 14:44:56.000000 aps_common_libraries-1.0.7/setup.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.955949 aps_common_libraries-1.0.8/
+-rw-rw-rw-   0 bishop    (1601)      907     1080 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.8/LICENSE
+-rw-rw-rw-   0 bishop    (1601)      907    10366 2022-10-17 22:57:50.000000 aps_common_libraries-1.0.8/LICENSE.pdf
+-rw-rw-rw-   0 bishop    (1601)      907       66 2022-10-17 22:57:24.000000 aps_common_libraries-1.0.8/MANIFEST.in
+-rw-r--r--   0 bishop    (1601)      907      876 2023-05-16 12:16:43.955264 aps_common_libraries-1.0.8/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907       46 2022-10-17 22:27:30.000000 aps_common_libraries-1.0.8/README.md
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.879046 aps_common_libraries-1.0.8/aps/
+-rw-rw-rw-   0 bishop    (1601)      907     3471 2022-10-17 23:25:46.000000 aps_common_libraries-1.0.8/aps/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.886590 aps_common_libraries-1.0.8/aps/common/
+-rw-rw-rw-   0 bishop    (1601)      907     3426 2022-10-18 00:01:10.000000 aps_common_libraries-1.0.8/aps/common/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.890087 aps_common_libraries-1.0.8/aps/common/__test/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2023-02-17 17:17:14.000000 aps_common_libraries-1.0.8/aps/common/__test/__init__.py
+-rw-r--r--   0 bishop    (1601)      907     3683 2023-05-05 00:42:24.000000 aps_common_libraries-1.0.8/aps/common/__test/singletons.py
+-rw-rw-rw-   0 bishop    (1601)      907      548 2023-02-17 17:54:05.000000 aps_common_libraries-1.0.8/aps/common/__test/test.py
+-rw-r--r--   0 bishop    (1601)      907     5739 2023-05-05 00:41:47.000000 aps_common_libraries-1.0.8/aps/common/__test/test2.py
+-rw-rw-rw-   0 bishop    (1601)      907    10116 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.8/aps/common/initializer.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.895869 aps_common_libraries-1.0.8/aps/common/io/
+-rw-rw-rw-   0 bishop    (1601)      907     3344 2020-03-28 16:44:28.000000 aps_common_libraries-1.0.8/aps/common/io/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4627 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.8/aps/common/io/printout.py
+-rw-r--r--   0 bishop    (1601)      907     3693 2023-05-04 23:44:10.000000 aps_common_libraries-1.0.8/aps/common/io/sys_commands.py
+-rw-rw-rw-   0 bishop    (1601)      907     4434 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.8/aps/common/io/tcp_client.py
+-rw-rw-rw-   0 bishop    (1601)      907     8754 2022-10-17 22:43:33.000000 aps_common_libraries-1.0.8/aps/common/io/tiff_file.py
+-rw-rw-rw-   0 bishop    (1601)      907    20774 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.8/aps/common/logger.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.897126 aps_common_libraries-1.0.8/aps/common/measurment/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:27:18.000000 aps_common_libraries-1.0.8/aps/common/measurment/__init__.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.900880 aps_common_libraries-1.0.8/aps/common/measurment/beamline/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-07 15:31:01.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    10472 2023-03-29 01:21:24.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/image_collector.py
+-rw-r--r--   0 bishop    (1601)      907    32561 2023-03-31 13:27:26.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/image_processor.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.920880 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/
+-rw-rw-rw-   0 bishop    (1601)      907     5297 2022-10-28 18:51:12.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/SPINNet_estimate.py
+-rw-rw-rw-   0 bishop    (1601)      907    45615 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/WXST.py
+-rw-rw-rw-   0 bishop    (1601)      907     3453 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907    15218 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/diffraction_process.py
+-rw-rw-rw-   0 bishop    (1601)      907      872 2022-11-04 20:56:52.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/euclidean_dist.py
+-rw-rw-rw-   0 bishop    (1601)      907    19167 2022-11-25 18:22:48.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/func.py
+-rw-rw-rw-   0 bishop    (1601)      907    23426 2022-11-04 20:56:51.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/func_light.py
+-rw-rw-rw-   0 bishop    (1601)      907     2315 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/gui_func.py
+-rw-rw-rw-   0 bishop    (1601)      907     6834 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/integration.py
+-rw-rw-rw-   0 bishop    (1601)      907    77489 2023-03-31 13:34:40.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/main.py
+-rw-rw-rw-   0 bishop    (1601)      907     5964 2022-11-07 15:35:41.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/pattern_find.py
+-rw-rw-rw-   0 bishop    (1601)      907     7296 2022-11-07 15:35:42.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/pattern_propagate.py
+-rw-rw-rw-   0 bishop    (1601)      907      184 2022-10-14 18:17:50.000000 aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/utils.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.924942 aps_common_libraries-1.0.8/aps/common/ml/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-08 02:45:45.000000 aps_common_libraries-1.0.8/aps/common/ml/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     6469 2021-09-23 22:14:46.000000 aps_common_libraries-1.0.8/aps/common/ml/data_structures.py
+-rw-rw-rw-   0 bishop    (1601)      907     4889 2021-12-22 20:56:40.000000 aps_common_libraries-1.0.8/aps/common/ml/mocks.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.930738 aps_common_libraries-1.0.8/aps/common/plot/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.8/aps/common/plot/__init__.py
+-rw-r--r--   0 bishop    (1601)      907    45238 2023-05-10 12:48:38.000000 aps_common_libraries-1.0.8/aps/common/plot/gui.py
+-rw-rw-rw-   0 bishop    (1601)      907     4639 2022-11-18 03:11:28.000000 aps_common_libraries-1.0.8/aps/common/plot/image.py
+-rw-rw-rw-   0 bishop    (1601)      907     6494 2023-05-16 12:13:12.000000 aps_common_libraries-1.0.8/aps/common/plot/qt_application.py
+-rw-rw-rw-   0 bishop    (1601)      907    16735 2023-05-16 12:05:38.000000 aps_common_libraries-1.0.8/aps/common/plotter.py
+-rw-r--r--   0 bishop    (1601)      907     5229 2023-05-02 21:11:06.000000 aps_common_libraries-1.0.8/aps/common/reflection.py
+-rw-rw-rw-   0 bishop    (1601)      907     5129 2023-03-01 01:27:25.000000 aps_common_libraries-1.0.8/aps/common/registry.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.939422 aps_common_libraries-1.0.8/aps/common/scripts/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-11-10 21:26:33.000000 aps_common_libraries-1.0.8/aps/common/scripts/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     3533 2023-02-07 22:57:08.000000 aps_common_libraries-1.0.8/aps/common/scripts/abstract_command_line_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     3430 2023-02-10 22:33:06.000000 aps_common_libraries-1.0.8/aps/common/scripts/generic_process_manager.py
+-rw-rw-rw-   0 bishop    (1601)      907     8024 2023-05-10 00:09:44.000000 aps_common_libraries-1.0.8/aps/common/scripts/generic_qt_script.py
+-rw-rw-rw-   0 bishop    (1601)      907     4357 2023-05-10 14:40:34.000000 aps_common_libraries-1.0.8/aps/common/scripts/script_data.py
+-rw-rw-rw-   0 bishop    (1601)      907     4576 2022-11-10 17:23:20.000000 aps_common_libraries-1.0.8/aps/common/scripts/script_registry.py
+-rw-rw-rw-   0 bishop    (1601)      907     4677 2023-05-05 00:43:28.000000 aps_common_libraries-1.0.8/aps/common/singleton.py
+-rw-rw-rw-   0 bishop    (1601)      907    10093 2023-05-04 23:17:15.000000 aps_common_libraries-1.0.8/aps/common/traffic_light.py
+-rw-r--r--   0 bishop    (1601)      907     3543 2023-05-03 14:01:58.000000 aps_common_libraries-1.0.8/aps/common/utilities.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.945950 aps_common_libraries-1.0.8/aps/common/widgets/
+-rw-rw-rw-   0 bishop    (1601)      907     3390 2022-10-18 21:16:31.000000 aps_common_libraries-1.0.8/aps/common/widgets/__init__.py
+-rw-rw-rw-   0 bishop    (1601)      907     4214 2023-05-16 12:14:47.000000 aps_common_libraries-1.0.8/aps/common/widgets/close_app_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     5532 2023-02-27 21:48:03.000000 aps_common_libraries-1.0.8/aps/common/widgets/context_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     8506 2023-02-14 01:08:20.000000 aps_common_libraries-1.0.8/aps/common/widgets/generic_widget.py
+-rw-rw-rw-   0 bishop    (1601)      907     6095 2023-02-17 18:06:20.000000 aps_common_libraries-1.0.8/aps/common/widgets/log_stream_widget.py
+drwxr-xr-x   0 bishop    (1601)      907        0 2023-05-16 12:16:43.953948 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/
+-rw-rw-rw-   0 bishop    (1601)      907      876 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/PKG-INFO
+-rw-rw-rw-   0 bishop    (1601)      907     2268 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/SOURCES.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/dependency_links.txt
+-rw-rw-rw-   0 bishop    (1601)      907       15 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/namespace_packages.txt
+-rw-rw-rw-   0 bishop    (1601)      907        1 2022-10-17 23:01:46.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/not-zip-safe
+-rw-rw-rw-   0 bishop    (1601)      907      150 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/requires.txt
+-rw-rw-rw-   0 bishop    (1601)      907        4 2023-05-16 12:16:43.000000 aps_common_libraries-1.0.8/aps_common_libraries.egg-info/top_level.txt
+-rw-r--r--   0 bishop    (1601)      907       38 2023-05-16 12:16:43.956327 aps_common_libraries-1.0.8/setup.cfg
+-rw-r--r--   0 bishop    (1601)      907     5571 2023-05-16 12:16:28.000000 aps_common_libraries-1.0.8/setup.py
```

### Comparing `aps_common_libraries-1.0.7/LICENSE` & `aps_common_libraries-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/LICENSE.pdf` & `aps_common_libraries-1.0.8/LICENSE.pdf`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/PKG-INFO` & `aps_common_libraries-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps_common_libraries
-Version: 1.0.7
+Version: 1.0.8
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.7/aps/__init__.py` & `aps_common_libraries-1.0.8/aps/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/__init__.py` & `aps_common_libraries-1.0.8/aps/common/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/__test/__init__.py` & `aps_common_libraries-1.0.8/aps/common/__test/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/__test/singletons.py` & `aps_common_libraries-1.0.8/aps/common/__test/singletons.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/__test/test.py` & `aps_common_libraries-1.0.8/aps/common/__test/test.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/__test/test2.py` & `aps_common_libraries-1.0.8/aps/common/__test/test2.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/initializer.py` & `aps_common_libraries-1.0.8/aps/common/initializer.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/io/__init__.py` & `aps_common_libraries-1.0.8/aps/common/io/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/io/printout.py` & `aps_common_libraries-1.0.8/aps/common/io/printout.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/io/sys_commands.py` & `aps_common_libraries-1.0.8/aps/common/io/sys_commands.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/io/tcp_client.py` & `aps_common_libraries-1.0.8/aps/common/io/tcp_client.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/io/tiff_file.py` & `aps_common_libraries-1.0.8/aps/common/io/tiff_file.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/logger.py` & `aps_common_libraries-1.0.8/aps/common/logger.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/__init__.py` & `aps_common_libraries-1.0.8/aps/common/measurment/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/__init__.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/image_collector.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/image_collector.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/image_processor.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/image_processor.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/SPINNet_estimate.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/SPINNet_estimate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/WXST.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/WXST.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/__init__.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/diffraction_process.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/diffraction_process.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/euclidean_dist.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/euclidean_dist.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/func.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/func_light.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/func_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/gui_func.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/gui_func.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/integration.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/integration.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/main.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/main.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/pattern_find.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/pattern_find.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/measurment/beamline/wf/pattern_propagate.py` & `aps_common_libraries-1.0.8/aps/common/measurment/beamline/wf/pattern_propagate.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/ml/__init__.py` & `aps_common_libraries-1.0.8/aps/common/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/ml/data_structures.py` & `aps_common_libraries-1.0.8/aps/common/ml/data_structures.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/ml/mocks.py` & `aps_common_libraries-1.0.8/aps/common/ml/mocks.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/plot/__init__.py` & `aps_common_libraries-1.0.8/aps/common/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/plot/gui.py` & `aps_common_libraries-1.0.8/aps/common/plot/gui.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/plot/image.py` & `aps_common_libraries-1.0.8/aps/common/plot/image.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/plot/qt_application.py` & `aps_common_libraries-1.0.8/aps/common/plot/qt_application.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,32 +61,33 @@
 
 
 class QtApplicationMode:
     SHOW = 0
     HIDE = 99
 
 class QtApplicationFacade:
-    def show_application_closer(self): raise NotImplementedError()
+    def show_application_closer(self, minimized=False): raise NotImplementedError()
     def run_qt_application(self): raise NotImplementedError()
     def get_native_qt_object(self): raise NotImplementedError()
 
 class __NullQtApplication(QtApplicationFacade):
     def __init__(self): self.__qt_application = QApplication(sys.argv)
     def run_qt_application(self): self.__qt_application.exec_()
-    def show_application_closer(self): sys.exit(0)
+    def show_application_closer(self, minimized=False): sys.exit(0)
     def get_native_qt_object(self): return self.__qt_application
 
 class __QtApplication(QtApplicationFacade):
     def __init__(self):
         self.__qt_application = QApplication(sys.argv)
         self.__qt_application.setStyle(QStyleFactory.create('Fusion')) # 'Windows'
         self.__application_closer = CloseApp()
 
-    def show_application_closer(self):
-        self.__application_closer.show()
+    def show_application_closer(self, minimized=False):
+        if minimized: self.__application_closer.showMinimized()
+        else:         self.__application_closer.show()
 
     def run_qt_application(self):
         self.__qt_application.exec_()
 
     def get_native_qt_object(self): return self.__qt_application
 
 @Singleton
```

### Comparing `aps_common_libraries-1.0.7/aps/common/plotter.py` & `aps_common_libraries-1.0.8/aps/common/plotter.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/reflection.py` & `aps_common_libraries-1.0.8/aps/common/reflection.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/registry.py` & `aps_common_libraries-1.0.8/aps/common/registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/__init__.py` & `aps_common_libraries-1.0.8/aps/common/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/abstract_command_line_script.py` & `aps_common_libraries-1.0.8/aps/common/scripts/abstract_command_line_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/generic_process_manager.py` & `aps_common_libraries-1.0.8/aps/common/scripts/generic_process_manager.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/generic_qt_script.py` & `aps_common_libraries-1.0.8/aps/common/scripts/generic_qt_script.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/script_data.py` & `aps_common_libraries-1.0.8/aps/common/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/scripts/script_registry.py` & `aps_common_libraries-1.0.8/aps/common/scripts/script_registry.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/singleton.py` & `aps_common_libraries-1.0.8/aps/common/singleton.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/traffic_light.py` & `aps_common_libraries-1.0.8/aps/common/traffic_light.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/utilities.py` & `aps_common_libraries-1.0.8/aps/common/utilities.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/widgets/__init__.py` & `aps_common_libraries-1.0.8/aps/common/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/widgets/close_app_widget.py` & `aps_common_libraries-1.0.8/aps/common/widgets/close_app_widget.py`

 * *Files 8% similar despite different names*

```diff
@@ -41,20 +41,24 @@
 # LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN       #
 # ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE         #
 # POSSIBILITY OF SUCH DAMAGE.                                             #
 # #########################################################################
 
 import sys
 from PyQt5.QtWidgets import QMainWindow, QWidget, QHBoxLayout
+from PyQt5.QtCore import Qt
+
 from aps.common.plot.gui import widgetBox, button, ConfirmDialog
 
 class CloseApp(QMainWindow):
     def __init__(self, parent=None):
         super(CloseApp, self).__init__(parent)
 
+        self.setWindowFlags(Qt.CustomizeWindowHint | Qt.WindowTitleHint | Qt.WindowMinimizeButtonHint)
+
         self.setWindowTitle("Close Application")
         container_widget = QWidget()
         container_widget.setLayout(QHBoxLayout())
 
         box = widgetBox(container_widget)
         button(box, container_widget, "Exit", callback=self.close_all, height=50, width=200)
```

### Comparing `aps_common_libraries-1.0.7/aps/common/widgets/context_widget.py` & `aps_common_libraries-1.0.8/aps/common/widgets/context_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/widgets/generic_widget.py` & `aps_common_libraries-1.0.8/aps/common/widgets/generic_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps/common/widgets/log_stream_widget.py` & `aps_common_libraries-1.0.8/aps/common/widgets/log_stream_widget.py`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/aps_common_libraries.egg-info/PKG-INFO` & `aps_common_libraries-1.0.8/aps_common_libraries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: aps-common-libraries
-Version: 1.0.7
+Version: 1.0.8
 Summary: APS Common Libraries
 Home-page: https://github.com/APS-XSD-OPT-Group/Common-Libraries
 Author: Luca Rebuffi
 Author-email: lrebuffi@anl.gov
 Maintainer: XSD-OPT Group @ APS-ANL
 Maintainer-email: lrebuffi@anl.gov
 License: BSD-3
```

### Comparing `aps_common_libraries-1.0.7/aps_common_libraries.egg-info/SOURCES.txt` & `aps_common_libraries-1.0.8/aps_common_libraries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aps_common_libraries-1.0.7/setup.py` & `aps_common_libraries-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 try:
     from setuptools import find_packages, setup
 except AttributeError:
     from setuptools import find_packages, setup
 
 NAME = 'aps_common_libraries'
 
-VERSION = '1.0.7'
+VERSION = '1.0.8'
 ISRELEASED = False
 
 DESCRIPTION = 'APS Common Libraries'
 README_FILE = os.path.join(os.path.dirname(__file__), 'README.md')
 LONG_DESCRIPTION = open(README_FILE).read()
 AUTHOR = 'Luca Rebuffi'
 AUTHOR_EMAIL = 'lrebuffi@anl.gov'
```

