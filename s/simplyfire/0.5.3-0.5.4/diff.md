# Comparing `tmp/simplyfire-0.5.3.tar.gz` & `tmp/simplyfire-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplyfire-0.5.3.tar", last modified: Tue May 16 01:39:20 2023, max compression
+gzip compressed data, was "simplyfire-0.5.4.tar", last modified: Tue May 16 01:55:11 2023, max compression
```

## Comparing `simplyfire-0.5.3.tar` & `simplyfire-0.5.4.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.172795 simplyfire-0.5.3/
--rw-rw-rw-   0        0        0    33092 2023-05-01 23:06:43.000000 simplyfire-0.5.3/LICENSE
--rw-rw-rw-   0        0        0       66 2023-05-01 23:06:43.000000 simplyfire-0.5.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1947 2023-05-16 01:39:20.172795 simplyfire-0.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2023-05-01 23:06:43.000000 simplyfire-0.5.3/README.md
--rw-rw-rw-   0        0        0      108 2023-05-01 23:06:43.000000 simplyfire-0.5.3/pyproject.toml
--rw-rw-rw-   0        0        0      170 2023-05-16 01:39:20.176795 simplyfire-0.5.3/setup.cfg
--rw-rw-rw-   0        0        0     2564 2023-05-16 01:37:59.000000 simplyfire-0.5.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.032796 simplyfire-0.5.3/simplyfire/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.088799 simplyfire-0.5.3/simplyfire/__pycache__/
--rw-rw-rw-   0        0        0      174 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     3926 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/__pycache__/__main__.cpython-311.pyc
--rw-rw-rw-   0        0        0    24549 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/__pycache__/app.cpython-311.pyc
--rw-rw-rw-   0        0        0    15816 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/app.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.096795 simplyfire-0.5.3/simplyfire/backend/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/backend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.100796 simplyfire-0.5.3/simplyfire/backend/__pycache__/
--rw-rw-rw-   0        0        0      182 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/backend/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    20804 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/backend/__pycache__/interface.cpython-311.pyc
--rw-rw-rw-   0        0        0    27912 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/backend/__pycache__/interpreter.cpython-311.pyc
--rw-rw-rw-   0        0        0     5714 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/backend/__pycache__/plugin_manager.cpython-311.pyc
--rw-rw-rw-   0        0        0    16487 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/backend/interface.py
--rw-rw-rw-   0        0        0    22220 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/backend/interpreter.py
--rw-rw-rw-   0        0        0     4163 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/backend/plugin_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.112794 simplyfire-0.5.3/simplyfire/img/
--rw-rw-rw-   0        0        0      239 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/arrow.png
--rw-rw-rw-   0        0        0   123774 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/loading.gif
--rw-rw-rw-   0        0        0   108307 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/logo.ico
--rw-rw-rw-   0        0        0   106769 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/logo_bw.ico
--rw-rw-rw-   0        0        0      255 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/pan_up.png
--rw-rw-rw-   0        0        0      553 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/x_zoom_in.png
--rw-rw-rw-   0        0        0      482 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/x_zoom_out.png
--rw-rw-rw-   0        0        0      528 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/y_zoom_in.png
--rw-rw-rw-   0        0        0      506 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/y_zoom_out.png
--rw-rw-rw-   0        0        0      597 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/img/zoom_in_y.png
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.124797 simplyfire-0.5.3/simplyfire/layout/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/__init__.py
--rw-rw-rw-   0        0        0    28853 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/batch_popup.py
--rw-rw-rw-   0        0        0    12580 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/graph_panel.py
--rw-rw-rw-   0        0        0     4461 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/log_display.py
--rw-rw-rw-   0        0        0     8569 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/menubar.py
--rw-rw-rw-   0        0        0     5979 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/plugin_tab.py
--rw-rw-rw-   0        0        0     2635 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/results_display.py
--rw-rw-rw-   0        0        0    12488 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/setting_tab.py
--rw-rw-rw-   0        0        0    16937 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/layout/trace_display.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.000698 simplyfire-0.5.3/simplyfire/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.128796 simplyfire-0.5.3/simplyfire/plugins/comparison_plot/
--rw-rw-rw-   0        0        0    15742 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/comparison_plot/comparison_GUI.py
--rw-rw-rw-   0        0        0      200 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/comparison_plot/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.128796 simplyfire-0.5.3/simplyfire/plugins/evoked_basic/
--rw-rw-rw-   0        0        0    15452 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/evoked_basic/evoked_GUI.py
--rw-rw-rw-   0        0        0     2721 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/evoked_basic/evoked_analysis.py
--rw-rw-rw-   0        0        0      232 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/evoked_basic/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.132796 simplyfire-0.5.3/simplyfire/plugins/mini_analysis/
--rw-rw-rw-   0        0        0    89249 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/mini_analysis/mini_GUI.py
--rw-rw-rw-   0        0        0    61353 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/mini_analysis/mini_analysis.py
--rw-rw-rw-   0        0        0      236 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/mini_analysis/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.136798 simplyfire-0.5.3/simplyfire/plugins/navigation/
--rw-rw-rw-   0        0        0     8946 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/navigation/navigation.py
--rw-rw-rw-   0        0        0      172 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/navigation/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.140797 simplyfire-0.5.3/simplyfire/plugins/process_recording/
--rw-rw-rw-   0        0        0      254 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/process_recording/plugin.yaml
--rw-rw-rw-   0        0        0    20784 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/process_recording/process_GUI.py
--rw-rw-rw-   0        0        0     5259 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/process_recording/process_recording.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.140797 simplyfire-0.5.3/simplyfire/plugins/style/
--rw-rw-rw-   0        0        0      199 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/style/plugin.yaml
--rw-rw-rw-   0        0        0     5451 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/style/style_tab.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.144796 simplyfire-0.5.3/simplyfire/plugins/sweeps/
--rw-rw-rw-   0        0        0      201 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/sweeps/plugin.yaml
--rw-rw-rw-   0        0        0    14881 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/plugins/sweeps/sweeps_GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.144796 simplyfire-0.5.3/simplyfire/setting/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.148795 simplyfire-0.5.3/simplyfire/setting/__pycache__/
--rw-rw-rw-   0        0        0      182 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/setting/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     8282 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/setting/__pycache__/config.cpython-311.pyc
--rw-rw-rw-   0        0        0     6453 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/setting/config.py
--rw-rw-rw-   0        0        0     3517 2023-05-16 01:38:13.000000 simplyfire-0.5.3/simplyfire/setting/default_config.yaml
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.152795 simplyfire-0.5.3/simplyfire/temp/
--rw-rw-rw-   0        0        0      218 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/temp/README.md
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/temp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.164793 simplyfire-0.5.3/simplyfire/utils/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.172795 simplyfire-0.5.3/simplyfire/utils/__pycache__/
--rw-rw-rw-   0        0        0      180 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0     6248 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/abfWriter.cpython-311.pyc
--rw-rw-rw-   0        0        0    40642 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/custom_widgets.cpython-311.pyc
--rw-rw-rw-   0        0        0     4602 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/formatting.cpython-311.pyc
--rw-rw-rw-   0        0        0    27038 2023-05-16 01:33:31.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/recording.cpython-311.pyc
--rw-rw-rw-   0        0        0     4947 2023-05-16 01:33:30.000000 simplyfire-0.5.3/simplyfire/utils/__pycache__/validation.cpython-311.pyc
--rw-rw-rw-   0        0        0     6411 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/abfWriter.py
--rw-rw-rw-   0        0        0     6620 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/calculate.py
--rw-rw-rw-   0        0        0    23659 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/custom_widgets.py
--rw-rw-rw-   0        0        0     3311 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/formatting.py
--rw-rw-rw-   0        0        0     2932 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/plugin_GUI.py
--rw-rw-rw-   0        0        0     8664 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/plugin_controller.py
--rw-rw-rw-   0        0        0     7778 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/plugin_form.py
--rw-rw-rw-   0        0        0     1900 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/plugin_popup.py
--rw-rw-rw-   0        0        0     8023 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/plugin_table.py
--rw-rw-rw-   0        0        0    19383 2023-05-16 01:35:09.000000 simplyfire-0.5.3/simplyfire/utils/recording.py
--rw-rw-rw-   0        0        0    11690 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/scrollable_option_frame.py
--rw-rw-rw-   0        0        0     2651 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/threader.py
--rw-rw-rw-   0        0        0     3932 2023-05-01 23:06:43.000000 simplyfire-0.5.3/simplyfire/utils/validation.py
-drwxrwxrwx   0        0        0        0 2023-05-16 01:39:20.080796 simplyfire-0.5.3/simplyfire.egg-info/
--rw-rw-rw-   0        0        0     1947 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3278 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 23:21:50.000000 simplyfire-0.5.3/simplyfire.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 01:39:19.000000 simplyfire-0.5.3/simplyfire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.887534 simplyfire-0.5.4/
+-rw-rw-rw-   0        0        0    33092 2023-05-01 23:06:43.000000 simplyfire-0.5.4/LICENSE
+-rw-rw-rw-   0        0        0       66 2023-05-01 23:06:43.000000 simplyfire-0.5.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1947 2023-05-16 01:55:11.887534 simplyfire-0.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-05-01 23:06:43.000000 simplyfire-0.5.4/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-01 23:06:43.000000 simplyfire-0.5.4/pyproject.toml
+-rw-rw-rw-   0        0        0      170 2023-05-16 01:55:11.891562 simplyfire-0.5.4/setup.cfg
+-rw-rw-rw-   0        0        0     2564 2023-05-16 01:54:11.000000 simplyfire-0.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.743533 simplyfire-0.5.4/simplyfire/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.803540 simplyfire-0.5.4/simplyfire/__pycache__/
+-rw-rw-rw-   0        0        0      174 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     3926 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/__pycache__/__main__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    24549 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/__pycache__/app.cpython-311.pyc
+-rw-rw-rw-   0        0        0    15816 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/app.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.807535 simplyfire-0.5.4/simplyfire/backend/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/backend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.815535 simplyfire-0.5.4/simplyfire/backend/__pycache__/
+-rw-rw-rw-   0        0        0      182 2023-05-16 01:33:31.000000 simplyfire-0.5.4/simplyfire/backend/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    20804 2023-05-16 01:33:31.000000 simplyfire-0.5.4/simplyfire/backend/__pycache__/interface.cpython-311.pyc
+-rw-rw-rw-   0        0        0    27912 2023-05-16 01:33:31.000000 simplyfire-0.5.4/simplyfire/backend/__pycache__/interpreter.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5714 2023-05-16 01:33:31.000000 simplyfire-0.5.4/simplyfire/backend/__pycache__/plugin_manager.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16459 2023-05-16 01:49:36.000000 simplyfire-0.5.4/simplyfire/backend/interface.py
+-rw-rw-rw-   0        0        0    22220 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/backend/interpreter.py
+-rw-rw-rw-   0        0        0     4163 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/backend/plugin_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.827532 simplyfire-0.5.4/simplyfire/img/
+-rw-rw-rw-   0        0        0      239 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/arrow.png
+-rw-rw-rw-   0        0        0   123774 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/loading.gif
+-rw-rw-rw-   0        0        0   108307 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/logo.ico
+-rw-rw-rw-   0        0        0   106769 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/logo_bw.ico
+-rw-rw-rw-   0        0        0      255 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/pan_up.png
+-rw-rw-rw-   0        0        0      553 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/x_zoom_in.png
+-rw-rw-rw-   0        0        0      482 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/x_zoom_out.png
+-rw-rw-rw-   0        0        0      528 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/y_zoom_in.png
+-rw-rw-rw-   0        0        0      506 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/y_zoom_out.png
+-rw-rw-rw-   0        0        0      597 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/img/zoom_in_y.png
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.835536 simplyfire-0.5.4/simplyfire/layout/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/__init__.py
+-rw-rw-rw-   0        0        0    28853 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/batch_popup.py
+-rw-rw-rw-   0        0        0    12580 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/graph_panel.py
+-rw-rw-rw-   0        0        0     4461 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/log_display.py
+-rw-rw-rw-   0        0        0     8569 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/menubar.py
+-rw-rw-rw-   0        0        0     5979 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/plugin_tab.py
+-rw-rw-rw-   0        0        0     2635 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/results_display.py
+-rw-rw-rw-   0        0        0    12488 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/setting_tab.py
+-rw-rw-rw-   0        0        0    16937 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/layout/trace_display.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.731521 simplyfire-0.5.4/simplyfire/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.839532 simplyfire-0.5.4/simplyfire/plugins/comparison_plot/
+-rw-rw-rw-   0        0        0    15742 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/comparison_plot/comparison_GUI.py
+-rw-rw-rw-   0        0        0      200 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/comparison_plot/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.843532 simplyfire-0.5.4/simplyfire/plugins/evoked_basic/
+-rw-rw-rw-   0        0        0    15452 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/evoked_basic/evoked_GUI.py
+-rw-rw-rw-   0        0        0     2721 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/evoked_basic/evoked_analysis.py
+-rw-rw-rw-   0        0        0      232 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/evoked_basic/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.847532 simplyfire-0.5.4/simplyfire/plugins/mini_analysis/
+-rw-rw-rw-   0        0        0    89249 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/mini_analysis/mini_GUI.py
+-rw-rw-rw-   0        0        0    61353 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/mini_analysis/mini_analysis.py
+-rw-rw-rw-   0        0        0      236 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/mini_analysis/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.847532 simplyfire-0.5.4/simplyfire/plugins/navigation/
+-rw-rw-rw-   0        0        0     8946 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/navigation/navigation.py
+-rw-rw-rw-   0        0        0      172 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/navigation/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.851533 simplyfire-0.5.4/simplyfire/plugins/process_recording/
+-rw-rw-rw-   0        0        0      254 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/process_recording/plugin.yaml
+-rw-rw-rw-   0        0        0    20784 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/process_recording/process_GUI.py
+-rw-rw-rw-   0        0        0     5259 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/process_recording/process_recording.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.855531 simplyfire-0.5.4/simplyfire/plugins/style/
+-rw-rw-rw-   0        0        0      199 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/style/plugin.yaml
+-rw-rw-rw-   0        0        0     5451 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/style/style_tab.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.855531 simplyfire-0.5.4/simplyfire/plugins/sweeps/
+-rw-rw-rw-   0        0        0      201 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/sweeps/plugin.yaml
+-rw-rw-rw-   0        0        0    14881 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/plugins/sweeps/sweeps_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.859532 simplyfire-0.5.4/simplyfire/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.859532 simplyfire-0.5.4/simplyfire/setting/__pycache__/
+-rw-rw-rw-   0        0        0      182 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/setting/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     8282 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/setting/__pycache__/config.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6453 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/setting/config.py
+-rw-rw-rw-   0        0        0     3517 2023-05-16 01:53:44.000000 simplyfire-0.5.4/simplyfire/setting/default_config.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.863532 simplyfire-0.5.4/simplyfire/temp/
+-rw-rw-rw-   0        0        0      218 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/temp/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/temp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.879534 simplyfire-0.5.4/simplyfire/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.887534 simplyfire-0.5.4/simplyfire/utils/__pycache__/
+-rw-rw-rw-   0        0        0      180 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6248 2023-05-16 01:33:31.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/abfWriter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    40642 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/custom_widgets.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4602 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/formatting.cpython-311.pyc
+-rw-rw-rw-   0        0        0    26984 2023-05-16 01:42:05.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/recording.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4947 2023-05-16 01:33:30.000000 simplyfire-0.5.4/simplyfire/utils/__pycache__/validation.cpython-311.pyc
+-rw-rw-rw-   0        0        0     6411 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/abfWriter.py
+-rw-rw-rw-   0        0        0     6620 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/calculate.py
+-rw-rw-rw-   0        0        0    23659 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/custom_widgets.py
+-rw-rw-rw-   0        0        0     3311 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/formatting.py
+-rw-rw-rw-   0        0        0     2932 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/plugin_GUI.py
+-rw-rw-rw-   0        0        0     8664 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/plugin_controller.py
+-rw-rw-rw-   0        0        0     7778 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/plugin_form.py
+-rw-rw-rw-   0        0        0     1900 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/plugin_popup.py
+-rw-rw-rw-   0        0        0     8023 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/plugin_table.py
+-rw-rw-rw-   0        0        0    19383 2023-05-16 01:35:09.000000 simplyfire-0.5.4/simplyfire/utils/recording.py
+-rw-rw-rw-   0        0        0    11690 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/scrollable_option_frame.py
+-rw-rw-rw-   0        0        0     2651 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/threader.py
+-rw-rw-rw-   0        0        0     3932 2023-05-01 23:06:43.000000 simplyfire-0.5.4/simplyfire/utils/validation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:55:11.795534 simplyfire-0.5.4/simplyfire.egg-info/
+-rw-rw-rw-   0        0        0     1947 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3278 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 23:21:50.000000 simplyfire-0.5.4/simplyfire.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 01:55:11.000000 simplyfire-0.5.4/simplyfire.egg-info/top_level.txt
```

### Comparing `simplyfire-0.5.3/LICENSE` & `simplyfire-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/PKG-INFO` & `simplyfire-0.5.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.5.3
+Version: 0.5.4
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
 Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simplyfire-0.5.3/README.md` & `simplyfire-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/setup.py` & `simplyfire-0.5.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 """
 from setuptools import setup, find_packages
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='simplyfire',
-    version='0.5.3',
+    version='0.5.4',
     author='Megumi Mori, Andrew Rosko',
     description='Customizable electrophysiology analysis software',
     long_description=readme,
     long_description_content_type='text/markdown',
     url="https://simplyfire.readthedocs.io/",
     pakage_dir={'simplyfire':'simplyfire'},
     packages = find_packages(),
```

### Comparing `simplyfire-0.5.3/simplyfire/__main__.py` & `simplyfire-0.5.4/simplyfire/__main__.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/__pycache__/__main__.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/__pycache__/__main__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/__pycache__/app.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/__pycache__/app.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/app.py` & `simplyfire-0.5.4/simplyfire/app.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/backend/__pycache__/interface.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/backend/__pycache__/interface.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/backend/__pycache__/interpreter.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/backend/__pycache__/interpreter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/backend/__pycache__/plugin_manager.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/backend/__pycache__/plugin_manager.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/backend/interface.py` & `simplyfire-0.5.4/simplyfire/backend/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 import pandas as pd
 import os
 # This module is the workhorse of the GUI
 # Use this module to connect analysis functions to the GUI
 from simplyfire.utils import abfWriter
 from simplyfire.utils.recording import Recording
-from psutil import Process
 
 mini_df = pd.DataFrame()
 current_channel = 0
 
 
 ##########################
 # Undo controls
```

### Comparing `simplyfire-0.5.3/simplyfire/backend/interpreter.py` & `simplyfire-0.5.4/simplyfire/backend/interpreter.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/backend/plugin_manager.py` & `simplyfire-0.5.4/simplyfire/backend/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/loading.gif` & `simplyfire-0.5.4/simplyfire/img/loading.gif`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/logo.ico` & `simplyfire-0.5.4/simplyfire/img/logo.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/logo_bw.ico` & `simplyfire-0.5.4/simplyfire/img/logo_bw.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/x_zoom_in.png` & `simplyfire-0.5.4/simplyfire/img/x_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/y_zoom_in.png` & `simplyfire-0.5.4/simplyfire/img/y_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/img/zoom_in_y.png` & `simplyfire-0.5.4/simplyfire/img/zoom_in_y.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/batch_popup.py` & `simplyfire-0.5.4/simplyfire/layout/batch_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/graph_panel.py` & `simplyfire-0.5.4/simplyfire/layout/graph_panel.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/log_display.py` & `simplyfire-0.5.4/simplyfire/layout/log_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/menubar.py` & `simplyfire-0.5.4/simplyfire/layout/menubar.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/plugin_tab.py` & `simplyfire-0.5.4/simplyfire/layout/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/results_display.py` & `simplyfire-0.5.4/simplyfire/layout/results_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/setting_tab.py` & `simplyfire-0.5.4/simplyfire/layout/setting_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/layout/trace_display.py` & `simplyfire-0.5.4/simplyfire/layout/trace_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/comparison_plot/comparison_GUI.py` & `simplyfire-0.5.4/simplyfire/plugins/comparison_plot/comparison_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/evoked_basic/evoked_GUI.py` & `simplyfire-0.5.4/simplyfire/plugins/evoked_basic/evoked_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/evoked_basic/evoked_analysis.py` & `simplyfire-0.5.4/simplyfire/plugins/evoked_basic/evoked_analysis.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/mini_analysis/mini_GUI.py` & `simplyfire-0.5.4/simplyfire/plugins/mini_analysis/mini_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/mini_analysis/mini_analysis.py` & `simplyfire-0.5.4/simplyfire/plugins/mini_analysis/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/navigation/navigation.py` & `simplyfire-0.5.4/simplyfire/plugins/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/process_recording/process_GUI.py` & `simplyfire-0.5.4/simplyfire/plugins/process_recording/process_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/process_recording/process_recording.py` & `simplyfire-0.5.4/simplyfire/plugins/process_recording/process_recording.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/style/style_tab.py` & `simplyfire-0.5.4/simplyfire/plugins/style/style_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/plugins/sweeps/sweeps_GUI.py` & `simplyfire-0.5.4/simplyfire/plugins/sweeps/sweeps_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/setting/__pycache__/config.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/setting/__pycache__/config.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/setting/config.py` & `simplyfire-0.5.4/simplyfire/setting/config.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/setting/default_config.yaml` & `simplyfire-0.5.4/simplyfire/setting/default_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # The key_map dict is used to map most of the core key-bindings.
 # Key names follow the tkinter convention.
 # Until a key-mapper feature is added (planned for future releases),
 # the keys can be edited here.
 #################################################################
 
 # version
-version : '0.5.3'
+version : '0.5.4'
 
 #aesthetics
 geometry : '900x600'
 zoomed : 0
 
 relative_cp_width : 0.25
 cp_width : 270
```

### Comparing `simplyfire-0.5.3/simplyfire/utils/__pycache__/abfWriter.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/utils/__pycache__/abfWriter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/__pycache__/custom_widgets.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/utils/__pycache__/custom_widgets.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/__pycache__/formatting.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/utils/__pycache__/formatting.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/__pycache__/recording.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/utils/__pycache__/recording.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,20 +1,20 @@
 magic:    0xa70d0d0a
-moddate:  0x03465064 (Mon May  1 23:06:43 2023 UTC)
-files sz: 19411
+moddate:  0xcddd6264 (Tue May 16 01:35:09 2023 UTC)
+files sz: 19383
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
       0x970064005a00640164026c015a02640164026c035a03640164036c046d
       055a050100640164046c066d075a070100640164056c086d095a09010064
-      0164066c0a6d0b5a0b0100640164076c0c6d0d5a0d010002004700640884
-      006409a6020000ab0200000000000000005a0e64025300
+      0164066c0a6d0b5a0b010002004700640784006408a6020000ab02000000
+      00000000005a0c64025300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 ('\nRead abf files and store as Recording class\nData format for recording data used in the SimplyFire software.\n\nSimplyFire - Customizable analysis of electrophysiology data\nCopyright (C) 2022 Megumi Mori\nThis program comes with ABSOLUTELY NO WARRANTY\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU General Public License as published by\nthe Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n')
                  4 STORE_NAME               0 (__doc__)
    
     22           6 LOAD_CONST               1 (0)
                  8 LOAD_CONST               2 (None)
@@ -50,132 +50,124 @@
     27          58 LOAD_CONST               1 (0)
                 60 LOAD_CONST               6 (('ceil',))
                 62 IMPORT_NAME             10 (math)
                 64 IMPORT_FROM             11 (ceil)
                 66 STORE_NAME              11 (ceil)
                 68 POP_TOP
    
-    28          70 LOAD_CONST               1 (0)
-                72 LOAD_CONST               7 (('Process',))
-                74 IMPORT_NAME             12 (psutil)
-                76 IMPORT_FROM             13 (Process)
-                78 STORE_NAME              13 (Process)
-                80 POP_TOP
-   
-    30          82 PUSH_NULL
-                84 LOAD_BUILD_CLASS
-                86 LOAD_CONST               8 (<code object Recording, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 30>)
-                88 MAKE_FUNCTION            0
-                90 LOAD_CONST               9 ('Recording')
-                92 PRECALL                  2
-                96 CALL                     2
-               106 STORE_NAME              14 (Recording)
-               108 LOAD_CONST               2 (None)
-               110 RETURN_VALUE
+    29          70 PUSH_NULL
+                72 LOAD_BUILD_CLASS
+                74 LOAD_CONST               7 (<code object Recording, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 29>)
+                76 MAKE_FUNCTION            0
+                78 LOAD_CONST               8 ('Recording')
+                80 PRECALL                  2
+                84 CALL                     2
+                94 STORE_NAME              12 (Recording)
+                96 LOAD_CONST               2 (None)
+                98 RETURN_VALUE
    consts
       '\nRead abf files and store as Recording class\nData format for recording data used in the SimplyFire software.\n\nSimplyFire - Customizable analysis of electrophysiology data\nCopyright (C) 2022 Megumi Mori\nThis program comes with ABSOLUTELY NO WARRANTY\n\nThis program is free software: you can redistribute it and/or modify\nit under the terms of the GNU General Public License as published by\nthe Free Software Foundation, either version 3 of the License, or\n(at your option) any later version.\n\nThis program is distributed in the hope that it will be useful,\nbut WITHOUT ANY WARRANTY; without even the implied warranty of\nMERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the\nGNU General Public License for more details.\n\nYou should have received a copy of the GNU General Public License\nalong with this program.  If not, see <https://www.gnu.org/licenses/>.\n'
       0
       None
       ('abf',)
       ('abfWriter',)
       ('config',)
       ('ceil',)
-      ('Process',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 2
          flags     : 0
          code
             0x970065005a0164005a02640184005a03640284005a04640384005a0564
             0484005a066417640884015a07640984005a086418640a84015a09640b84
             005a0a6419640e84015a0b641a640f84015a0c641a641084015a0d641a64
             1184015a0e641a641284015a0f641b641384015a10641b641484015a1164
             1c641584015a12641684005a1364055300
-          30           0 RESUME                   0
+          29           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Recording')
                        8 STORE_NAME               2 (__qualname__)
          
-          31          10 LOAD_CONST               1 (<code object __init__, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 31>)
+          30          10 LOAD_CONST               1 (<code object __init__, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 30>)
                       12 MAKE_FUNCTION            0
                       14 STORE_NAME               3 (__init__)
          
-          39          16 LOAD_CONST               2 (<code object _open_file, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 39>)
+          38          16 LOAD_CONST               2 (<code object _open_file, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 38>)
                       18 MAKE_FUNCTION            0
                       20 STORE_NAME               4 (_open_file)
          
-          51          22 LOAD_CONST               3 (<code object read_abf, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 51>)
+          50          22 LOAD_CONST               3 (<code object read_abf, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 50>)
                       24 MAKE_FUNCTION            0
                       26 STORE_NAME               5 (read_abf)
          
-          80          28 LOAD_CONST               4 (<code object read_csv, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 80>)
+          79          28 LOAD_CONST               4 (<code object read_csv, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 79>)
                       30 MAKE_FUNCTION            0
                       32 STORE_NAME               6 (read_csv)
          
-         131          34 LOAD_CONST              23 ((None, 0, False))
-                      36 LOAD_CONST               8 (<code object save, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 131>)
+         130          34 LOAD_CONST              23 ((None, 0, False))
+                      36 LOAD_CONST               8 (<code object save, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 130>)
                       38 MAKE_FUNCTION            1 (defaults)
                       40 STORE_NAME               7 (save)
          
-         149          42 LOAD_CONST               9 (<code object write_abf, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 149>)
+         148          42 LOAD_CONST               9 (<code object write_abf, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 148>)
                       44 MAKE_FUNCTION            0
                       46 STORE_NAME               8 (write_abf)
          
-         153          48 LOAD_CONST              24 ((None,))
-                      50 LOAD_CONST              10 (<code object write_csv, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 153>)
+         152          48 LOAD_CONST              24 ((None,))
+                      50 LOAD_CONST              10 (<code object write_csv, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 152>)
                       52 MAKE_FUNCTION            1 (defaults)
                       54 STORE_NAME               9 (write_csv)
          
-         172          56 LOAD_CONST              11 (<code object set_channel, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 172>)
+         171          56 LOAD_CONST              11 (<code object set_channel, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 171>)
                       58 MAKE_FUNCTION            0
                       60 STORE_NAME              10 (set_channel)
          
-         181          62 LOAD_CONST              25 (('continuous', None, None, None, True))
-                      64 LOAD_CONST              14 (<code object replace_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 181>)
+         180          62 LOAD_CONST              25 (('continuous', None, None, None, True))
+                      64 LOAD_CONST              14 (<code object replace_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 180>)
                       66 MAKE_FUNCTION            1 (defaults)
                       68 STORE_NAME              11 (replace_y_data)
          
-         220          70 LOAD_CONST              26 (('continuous', None, None, None))
-                      72 LOAD_CONST              15 (<code object get_y_matrix, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 220>)
+         219          70 LOAD_CONST              26 (('continuous', None, None, None))
+                      72 LOAD_CONST              15 (<code object get_y_matrix, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 219>)
                       74 MAKE_FUNCTION            1 (defaults)
                       76 STORE_NAME              12 (get_y_matrix)
          
-         261          78 LOAD_CONST              26 (('continuous', None, None, None))
-                      80 LOAD_CONST              16 (<code object get_x_matrix, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 261>)
+         260          78 LOAD_CONST              26 (('continuous', None, None, None))
+                      80 LOAD_CONST              16 (<code object get_x_matrix, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 260>)
                       82 MAKE_FUNCTION            1 (defaults)
                       84 STORE_NAME              13 (get_x_matrix)
          
-         293          86 LOAD_CONST              26 (('continuous', None, None, None))
-                      88 LOAD_CONST              17 (<code object get_xs, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 293>)
+         292          86 LOAD_CONST              26 (('continuous', None, None, None))
+                      88 LOAD_CONST              17 (<code object get_xs, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 292>)
                       90 MAKE_FUNCTION            1 (defaults)
                       92 STORE_NAME              14 (get_xs)
          
-         317          94 LOAD_CONST              26 (('continuous', None, None, None))
-                      96 LOAD_CONST              18 (<code object get_ys, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 317>)
+         316          94 LOAD_CONST              26 (('continuous', None, None, None))
+                      96 LOAD_CONST              18 (<code object get_ys, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 316>)
                       98 MAKE_FUNCTION            1 (defaults)
                      100 STORE_NAME              15 (get_ys)
          
-         349         102 LOAD_CONST              27 ((None, None))
-                     104 LOAD_CONST              19 (<code object save_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 349>)
+         348         102 LOAD_CONST              27 ((None, None))
+                     104 LOAD_CONST              19 (<code object save_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 348>)
                      106 MAKE_FUNCTION            1 (defaults)
                      108 STORE_NAME              16 (save_y_data)
          
-         369         110 LOAD_CONST              27 ((None, None))
-                     112 LOAD_CONST              20 (<code object load_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 369>)
+         368         110 LOAD_CONST              27 ((None, None))
+                     112 LOAD_CONST              20 (<code object load_y_data, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 368>)
                      114 MAKE_FUNCTION            1 (defaults)
                      116 STORE_NAME              17 (load_y_data)
          
-         380         118 LOAD_CONST              28 ((None, 0))
-                     120 LOAD_CONST              21 (<code object append_sweep, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 380>)
+         379         118 LOAD_CONST              28 ((None, 0))
+                     120 LOAD_CONST              21 (<code object append_sweep, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 379>)
                      122 MAKE_FUNCTION            1 (defaults)
                      124 STORE_NAME              18 (append_sweep)
          
-         404         126 LOAD_CONST              22 (<code object delete_last_sweep, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 404>)
+         403         126 LOAD_CONST              22 (<code object delete_last_sweep, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 403>)
                      128 MAKE_FUNCTION            0
                      130 STORE_NAME              19 (delete_last_sweep)
                      132 LOAD_CONST               5 (None)
                      134 RETURN_VALUE
          consts
             'Recording'
             code
@@ -184,33 +176,33 @@
                stacksize : 3
                flags     : 3
                code
                   0x97007c017c005f00000000000000000064017c005f0100000000000000
                   0064017c005f02000000000000000064017c005f0300000000000000007c
                   00a00400000000000000000000000000000000000000007c01a6010000ab
                   010000000000000000010064005300
-                31           0 RESUME                   0
+                30           0 RESUME                   0
                
-                32           2 LOAD_FAST                1 (filepath)
+                31           2 LOAD_FAST                1 (filepath)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (filepath)
                
-                34          16 LOAD_CONST               1 (0)
+                33          16 LOAD_CONST               1 (0)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (channel)
                
-                35          30 LOAD_CONST               1 (0)
+                34          30 LOAD_CONST               1 (0)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (added_sweep_count)
                
-                36          44 LOAD_CONST               1 (0)
+                35          44 LOAD_CONST               1 (0)
                             46 LOAD_FAST                0 (self)
                             48 STORE_ATTR               3 (sweep_count)
                
-                37          58 LOAD_FAST                0 (self)
+                36          58 LOAD_FAST                0 (self)
                             60 LOAD_METHOD              4 (_open_file)
                             82 LOAD_FAST                1 (filepath)
                             84 PRECALL                  1
                             88 CALL                     1
                             98 POP_TOP
                            100 LOAD_CONST               0 (None)
                            102 RETURN_VALUE
@@ -219,15 +211,15 @@
                   0
                names      ('filepath', 'channel', 'added_sweep_count', 'sweep_count', '_open_file')
                varnames   ('self', 'filepath')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       '__init__'
-               firstlineno 31
+               firstlineno 30
                lnotab 0x02010e020e010e010e01
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
@@ -238,83 +230,83 @@
                   00000000000000000000007c01a6010000ab0100000000000000005c0200
                   007c005f0500000000000000007c005f0600000000000000007c006a0300
                   0000000000000064026b020000000072177c00a007000000000000000000
                   00000000000000000000007c01a6010000ab010000000000000000010064
                   0053007c006a03000000000000000064036b020000000072177c00a00800
                   000000000000000000000000000000000000007c01a6010000ab01000000
                   000000000001006400530064005300
-                39           0 RESUME                   0
+                38           0 RESUME                   0
                
-                40           2 LOAD_GLOBAL              0 (os)
+                39           2 LOAD_GLOBAL              0 (os)
                             14 LOAD_ATTR                1 (path)
                             24 LOAD_METHOD              2 (splitext)
                             46 LOAD_FAST                1 (filename)
                             48 PRECALL                  1
                             52 CALL                     1
                             62 LOAD_CONST               1 (1)
                             64 BINARY_SUBSCR
                             74 LOAD_FAST                0 (self)
                             76 STORE_ATTR               3 (filetype)
                
-                41          86 LOAD_GLOBAL              0 (os)
+                40          86 LOAD_GLOBAL              0 (os)
                             98 LOAD_ATTR                1 (path)
                            108 LOAD_METHOD              4 (split)
                            130 LOAD_FAST                1 (filename)
                            132 PRECALL                  1
                            136 CALL                     1
                            146 UNPACK_SEQUENCE          2
                            150 LOAD_FAST                0 (self)
                            152 STORE_ATTR               5 (filedir)
                            162 LOAD_FAST                0 (self)
                            164 STORE_ATTR               6 (filename)
                
-                43         174 LOAD_FAST                0 (self)
+                42         174 LOAD_FAST                0 (self)
                            176 LOAD_ATTR                3 (filetype)
                            186 LOAD_CONST               2 ('.abf')
                            188 COMPARE_OP               2 (==)
                            194 POP_JUMP_FORWARD_IF_FALSE    23 (to 242)
                
-                44         196 LOAD_FAST                0 (self)
+                43         196 LOAD_FAST                0 (self)
                            198 LOAD_METHOD              7 (read_abf)
                            220 LOAD_FAST                1 (filename)
                            222 PRECALL                  1
                            226 CALL                     1
                            236 POP_TOP
                            238 LOAD_CONST               0 (None)
                            240 RETURN_VALUE
                
-                45     >>  242 LOAD_FAST                0 (self)
+                44     >>  242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                3 (filetype)
                            254 LOAD_CONST               3 ('.csv')
                            256 COMPARE_OP               2 (==)
                            262 POP_JUMP_FORWARD_IF_FALSE    23 (to 310)
                
-                46         264 LOAD_FAST                0 (self)
+                45         264 LOAD_FAST                0 (self)
                            266 LOAD_METHOD              8 (read_csv)
                            288 LOAD_FAST                1 (filename)
                            290 PRECALL                  1
                            294 CALL                     1
                            304 POP_TOP
                            306 LOAD_CONST               0 (None)
                            308 RETURN_VALUE
                
-                50     >>  310 LOAD_CONST               0 (None)
+                49     >>  310 LOAD_CONST               0 (None)
                            312 RETURN_VALUE
                consts
                   None
                   1
                   '.abf'
                   '.csv'
                names      ('os', 'path', 'splitext', 'filetype', 'split', 'filedir', 'filename', 'read_abf', 'read_csv')
                varnames   ('self', 'filename')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       '_open_file'
-               firstlineno 39
+               firstlineno 38
                lnotab 0x02015401580216012e0116012e04
             code
                argcount  : 2
                nlocals   : 4
                stacksize : 6
                flags     : 3
                code
@@ -337,127 +329,127 @@
                   005f1600000000000000007c026a1700000000000000007c005f18000000
                   00000000007c006a1800000000000000007c005f1900000000000000007c
                   026a1a00000000000000007c005f1b000000000000000074390000000000
                   00000000006a1d00000000000000007c026a1e00000000000000007c006a
                   0900000000000000007c006a1800000000000000007c006a1b0000000000
                   0000006603a6020000ab0200000000000000007c005f1f00000000000000
                   0064005300
-                51           0 RESUME                   0
+                50           0 RESUME                   0
                
-                52           2 LOAD_GLOBAL              1 (NULL + abf)
+                51           2 LOAD_GLOBAL              1 (NULL + abf)
                             14 LOAD_ATTR                1 (ABF)
                             24 LOAD_FAST                1 (filename)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 STORE_FAST               2 (data)
                
-                54          42 LOAD_FAST                2 (data)
+                53          42 LOAD_FAST                2 (data)
                             44 LOAD_ATTR                2 (dataRate)
                             54 LOAD_FAST                0 (self)
                             56 STORE_ATTR               3 (sampling_rate)
                
-                56          66 LOAD_GLOBAL              9 (NULL + len)
+                55          66 LOAD_GLOBAL              9 (NULL + len)
                             78 LOAD_GLOBAL             11 (NULL + str)
                             90 LOAD_FAST                0 (self)
                             92 LOAD_ATTR                3 (sampling_rate)
                            102 PRECALL                  1
                            106 CALL                     1
                            116 PRECALL                  1
                            120 CALL                     1
                            130 LOAD_CONST               1 (1)
                            132 BINARY_OP               10 (-)
                            136 LOAD_FAST                0 (self)
                            138 STORE_ATTR               6 (x_sigdig)
                
-                58         148 LOAD_CONST               1 (1)
+                57         148 LOAD_CONST               1 (1)
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                3 (sampling_rate)
                            162 BINARY_OP               11 (/)
                            166 LOAD_FAST                0 (self)
                            168 STORE_ATTR               7 (x_interval)
                
-                61         178 LOAD_FAST                2 (data)
+                60         178 LOAD_FAST                2 (data)
                            180 LOAD_ATTR                8 (channelCount)
                            190 LOAD_FAST                0 (self)
                            192 STORE_ATTR               9 (channel_count)
                
-                62         202 LOAD_FAST                2 (data)
+                61         202 LOAD_FAST                2 (data)
                            204 LOAD_ATTR               10 (adcNames)
                            214 LOAD_FAST                0 (self)
                            216 STORE_ATTR              11 (channel_names)
                
-                63         226 LOAD_FAST                2 (data)
+                62         226 LOAD_FAST                2 (data)
                            228 LOAD_ATTR               12 (adcUnits)
                            238 LOAD_FAST                0 (self)
                            240 STORE_ATTR              13 (channel_units)
                
-                64         250 LOAD_CONST               2 ('')
+                63         250 LOAD_CONST               2 ('')
                            252 BUILD_LIST               1
                            254 LOAD_FAST                0 (self)
                            256 LOAD_ATTR                9 (channel_count)
                            266 BINARY_OP                5 (*)
                            270 LOAD_FAST                0 (self)
                            272 STORE_ATTR              14 (channel_labels)
                
-                65         282 LOAD_GLOBAL             31 (NULL + range)
+                64         282 LOAD_GLOBAL             31 (NULL + range)
                            294 LOAD_FAST                0 (self)
                            296 LOAD_ATTR                9 (channel_count)
                            306 PRECALL                  1
                            310 CALL                     1
                            320 GET_ITER
                        >>  322 FOR_ITER                59 (to 442)
                            324 STORE_FAST               3 (c)
                
-                66         326 LOAD_FAST                2 (data)
+                65         326 LOAD_FAST                2 (data)
                            328 LOAD_METHOD             16 (setSweep)
                            350 LOAD_CONST               3 (0)
                            352 LOAD_FAST                3 (c)
                            354 PRECALL                  2
                            358 CALL                     2
                            368 POP_TOP
                
-                67         370 LOAD_FAST                2 (data)
+                66         370 LOAD_FAST                2 (data)
                            372 LOAD_ATTR               17 (sweepLabelY)
                            382 LOAD_METHOD             18 (replace)
                            404 LOAD_CONST               4 ('\x00')
                            406 LOAD_CONST               2 ('')
                            408 PRECALL                  2
                            412 CALL                     2
                            422 LOAD_FAST                0 (self)
                            424 LOAD_ATTR               14 (channel_labels)
                            434 LOAD_FAST                3 (c)
                            436 STORE_SUBSCR
                            440 JUMP_BACKWARD           60 (to 322)
                
-                69     >>  442 LOAD_FAST                2 (data)
+                68     >>  442 LOAD_FAST                2 (data)
                            444 LOAD_ATTR               19 (sweepUnitsX)
                            454 LOAD_FAST                0 (self)
                            456 STORE_ATTR              20 (x_unit)
                
-                70         466 LOAD_FAST                2 (data)
+                69         466 LOAD_FAST                2 (data)
                            468 LOAD_ATTR               21 (sweepLabelX)
                            478 LOAD_FAST                0 (self)
                            480 STORE_ATTR              22 (x_label)
                
-                73         490 LOAD_FAST                2 (data)
+                72         490 LOAD_FAST                2 (data)
                            492 LOAD_ATTR               23 (sweepCount)
                            502 LOAD_FAST                0 (self)
                            504 STORE_ATTR              24 (sweep_count)
                
-                74         514 LOAD_FAST                0 (self)
+                73         514 LOAD_FAST                0 (self)
                            516 LOAD_ATTR               24 (sweep_count)
                            526 LOAD_FAST                0 (self)
                            528 STORE_ATTR              25 (original_sweep_count)
                
-                75         538 LOAD_FAST                2 (data)
+                74         538 LOAD_FAST                2 (data)
                            540 LOAD_ATTR               26 (sweepPointCount)
                            550 LOAD_FAST                0 (self)
                            552 STORE_ATTR              27 (sweep_points)
                
-                78         562 LOAD_GLOBAL             57 (NULL + np)
+                77         562 LOAD_GLOBAL             57 (NULL + np)
                            574 LOAD_ATTR               29 (reshape)
                            584 LOAD_FAST                2 (data)
                            586 LOAD_ATTR               30 (data)
                            596 LOAD_FAST                0 (self)
                            598 LOAD_ATTR                9 (channel_count)
                            608 LOAD_FAST                0 (self)
                            610 LOAD_ATTR               24 (sweep_count)
@@ -478,15 +470,15 @@
                   '\x00'
                names      ('abf', 'ABF', 'dataRate', 'sampling_rate', 'len', 'str', 'x_sigdig', 'x_interval', 'channelCount', 'channel_count', 'adcNames', 'channel_names', 'adcUnits', 'channel_units', 'channel_labels', 'range', 'setSweep', 'sweepLabelY', 'replace', 'sweepUnitsX', 'x_unit', 'sweepLabelX', 'x_label', 'sweepCount', 'sweep_count', 'original_sweep_count', 'sweepPointCount', 'sweep_points', 'np', 'reshape', 'data', 'y_data')
                varnames   ('self', 'filename', 'data', 'c')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'read_abf'
-               firstlineno 51
+               firstlineno 50
                lnotab
                   0x02012802180252021e0318011801180120012c012c0148021801180318
                   0118011803
             code
                argcount  : 2
                nlocals   : 8
                stacksize : 13
@@ -536,241 +528,241 @@
                   000000742f000000000000000000006a1a00000000000000007c07a60100
                   00ab010000000000000000640164017c006a0200000000000000006603a6
                   020000ab0200000000000000007c005f15000000000000000090028c407c
                   006a01000000000000000064026b020000000072177c006a150000000000
                   0000006a1600000000000000006401190000000000000000007c005f0100
                   00000000000000640764076407a6020000ab020000000000000000010064
                   0753002300310073047702780359007701010059000100010064075300
-                80           0 RESUME                   0
+                79           0 RESUME                   0
                
-                84           2 LOAD_CONST               1 (1)
+                83           2 LOAD_CONST               1 (1)
                              4 LOAD_FAST                0 (self)
                              6 STORE_ATTR               0 (channel_count)
                
-                85          16 LOAD_CONST               2 (0)
+                84          16 LOAD_CONST               2 (0)
                             18 LOAD_FAST                0 (self)
                             20 STORE_ATTR               1 (sweep_count)
                
-                86          30 LOAD_CONST               2 (0)
+                85          30 LOAD_CONST               2 (0)
                             32 LOAD_FAST                0 (self)
                             34 STORE_ATTR               2 (sweep_points)
                
-                87          44 LOAD_CONST               3 ('sec')
+                86          44 LOAD_CONST               3 ('sec')
                             46 BUILD_LIST               1
                             48 LOAD_FAST                0 (self)
                             50 STORE_ATTR               3 (x_unit)
                
-                88          60 LOAD_CONST               4 ('N/A')
+                87          60 LOAD_CONST               4 ('N/A')
                             62 BUILD_LIST               1
                             64 LOAD_FAST                0 (self)
                             66 STORE_ATTR               4 (y_unit)
                
-                89          76 LOAD_CONST               4 ('N/A')
+                88          76 LOAD_CONST               4 ('N/A')
                             78 BUILD_LIST               1
                             80 LOAD_FAST                0 (self)
                             82 STORE_ATTR               5 (y_label)
                
-                90          92 LOAD_GLOBAL             13 (NULL + open)
+                89          92 LOAD_GLOBAL             13 (NULL + open)
                            104 LOAD_FAST                1 (filename)
                            106 LOAD_CONST               5 ('r')
                            108 PRECALL                  2
                            112 CALL                     2
                            122 BEFORE_WITH
                            124 STORE_FAST               2 (f)
                
-                91         126 LOAD_FAST                2 (f)
+                90         126 LOAD_FAST                2 (f)
                            128 LOAD_METHOD              7 (readlines)
                            150 PRECALL                  0
                            154 CALL                     0
                            164 GET_ITER
                        >>  166 EXTENDED_ARG             2
                            168 FOR_ITER               574 (to 1318)
                            170 STORE_FAST               3 (l)
                
-                92         172 LOAD_FAST                3 (l)
+                91         172 LOAD_FAST                3 (l)
                            174 LOAD_METHOD              8 (strip)
                            196 PRECALL                  0
                            200 CALL                     0
                            210 STORE_FAST               3 (l)
                
-                93         212 LOAD_FAST                3 (l)
+                92         212 LOAD_FAST                3 (l)
                            214 LOAD_CONST               2 (0)
                            216 BINARY_SUBSCR
                            226 LOAD_CONST               6 ('@')
                            228 COMPARE_OP               2 (==)
                            234 EXTENDED_ARG             1
                            236 POP_JUMP_FORWARD_IF_FALSE   293 (to 824)
                
-                94         238 LOAD_FAST                3 (l)
+                93         238 LOAD_FAST                3 (l)
                            240 LOAD_CONST               1 (1)
                            242 LOAD_CONST               7 (None)
                            244 BUILD_SLICE              2
                            246 BINARY_SUBSCR
                            256 LOAD_METHOD              9 (split)
                            278 LOAD_CONST               8 ('=')
                            280 PRECALL                  1
                            284 CALL                     1
                            294 LOAD_CONST               2 (0)
                            296 BINARY_SUBSCR
                            306 STORE_FAST               4 (header_label)
                
-                95         308 LOAD_FAST                3 (l)
+                94         308 LOAD_FAST                3 (l)
                            310 LOAD_CONST               1 (1)
                            312 LOAD_CONST               7 (None)
                            314 BUILD_SLICE              2
                            316 BINARY_SUBSCR
                            326 LOAD_METHOD              9 (split)
                            348 LOAD_CONST               8 ('=')
                            350 PRECALL                  1
                            354 CALL                     1
                            364 LOAD_CONST               1 (1)
                            366 BINARY_SUBSCR
                            376 STORE_FAST               5 (header_data)
                
-                96         378 LOAD_FAST                4 (header_label)
+                95         378 LOAD_FAST                4 (header_label)
                            380 LOAD_CONST               9 ('version')
                            382 COMPARE_OP               2 (==)
                            388 POP_JUMP_FORWARD_IF_FALSE     3 (to 396)
                
-                97         390 LOAD_FAST                5 (header_data)
+                96         390 LOAD_FAST                5 (header_data)
                            392 STORE_FAST               6 (version)
                            394 JUMP_BACKWARD          115 (to 166)
                
-                98     >>  396 LOAD_FAST                4 (header_label)
+                97     >>  396 LOAD_FAST                4 (header_label)
                            398 LOAD_CONST              10 ('sweep_count')
                            400 COMPARE_OP               2 (==)
                            406 POP_JUMP_FORWARD_IF_FALSE    33 (to 474)
                
-                99         408 LOAD_GLOBAL             21 (NULL + int)
+                98         408 LOAD_GLOBAL             21 (NULL + int)
                            420 LOAD_FAST                5 (header_data)
                            422 PRECALL                  1
                            426 CALL                     1
                            436 LOAD_FAST                0 (self)
                            438 STORE_ATTR               1 (sweep_count)
                
-               100         448 LOAD_FAST                0 (self)
+                99         448 LOAD_FAST                0 (self)
                            450 LOAD_ATTR                1 (sweep_count)
                            460 LOAD_FAST                0 (self)
                            462 STORE_ATTR              11 (original_sweep_count)
                            472 JUMP_BACKWARD          154 (to 166)
                
-               101     >>  474 LOAD_FAST                4 (header_label)
+               100     >>  474 LOAD_FAST                4 (header_label)
                            476 LOAD_CONST              11 ('sweep_points')
                            478 COMPARE_OP               2 (==)
                            484 POP_JUMP_FORWARD_IF_FALSE    21 (to 528)
                
-               102         486 LOAD_GLOBAL             21 (NULL + int)
+               101         486 LOAD_GLOBAL             21 (NULL + int)
                            498 LOAD_FAST                5 (header_data)
                            500 PRECALL                  1
                            504 CALL                     1
                            514 LOAD_FAST                0 (self)
                            516 STORE_ATTR               2 (sweep_points)
                            526 JUMP_BACKWARD          181 (to 166)
                
-               103     >>  528 LOAD_FAST                4 (header_label)
+               102     >>  528 LOAD_FAST                4 (header_label)
                            530 LOAD_CONST              12 ('sampling_rate')
                            532 COMPARE_OP               2 (==)
                            538 POP_JUMP_FORWARD_IF_FALSE    78 (to 696)
                
-               104         540 LOAD_GLOBAL             25 (NULL + float)
+               103         540 LOAD_GLOBAL             25 (NULL + float)
                            552 LOAD_FAST                5 (header_data)
                            554 PRECALL                  1
                            558 CALL                     1
                            568 LOAD_FAST                0 (self)
                            570 STORE_ATTR              13 (sampling_rate)
                
-               106         580 LOAD_GLOBAL             29 (NULL + len)
+               105         580 LOAD_GLOBAL             29 (NULL + len)
                            592 LOAD_GLOBAL             31 (NULL + str)
                            604 LOAD_FAST                0 (self)
                            606 LOAD_ATTR               13 (sampling_rate)
                            616 PRECALL                  1
                            620 CALL                     1
                            630 PRECALL                  1
                            634 CALL                     1
                            644 LOAD_CONST               1 (1)
                            646 BINARY_OP               10 (-)
                            650 LOAD_FAST                0 (self)
                            652 STORE_ATTR              16 (x_sigdig)
                
-               108         662 LOAD_CONST               1 (1)
+               107         662 LOAD_CONST               1 (1)
                            664 LOAD_FAST                0 (self)
                            666 LOAD_ATTR               13 (sampling_rate)
                            676 BINARY_OP               11 (/)
                            680 LOAD_FAST                0 (self)
                            682 STORE_ATTR              17 (x_interval)
                            692 EXTENDED_ARG             1
                            694 JUMP_BACKWARD          265 (to 166)
                
-               109     >>  696 LOAD_FAST                4 (header_label)
+               108     >>  696 LOAD_FAST                4 (header_label)
                            698 LOAD_CONST              13 ('channel_unit')
                            700 COMPARE_OP               2 (==)
                            706 POP_JUMP_FORWARD_IF_FALSE    10 (to 728)
                
-               110         708 LOAD_FAST                5 (header_data)
+               109         708 LOAD_FAST                5 (header_data)
                            710 BUILD_LIST               1
                            712 LOAD_FAST                0 (self)
                            714 STORE_ATTR              18 (channel_units)
                            724 EXTENDED_ARG             1
                            726 JUMP_BACKWARD          281 (to 166)
                
-               111     >>  728 LOAD_FAST                4 (header_label)
+               110     >>  728 LOAD_FAST                4 (header_label)
                            730 LOAD_CONST              14 ('channel_label')
                            732 COMPARE_OP               2 (==)
                            738 POP_JUMP_FORWARD_IF_FALSE    10 (to 760)
                
-               112         740 LOAD_FAST                5 (header_data)
+               111         740 LOAD_FAST                5 (header_data)
                            742 BUILD_LIST               1
                            744 LOAD_FAST                0 (self)
                            746 STORE_ATTR              19 (channel_labels)
                            756 EXTENDED_ARG             1
                            758 JUMP_BACKWARD          297 (to 166)
                
-               113     >>  760 LOAD_FAST                4 (header_label)
+               112     >>  760 LOAD_FAST                4 (header_label)
                            762 LOAD_CONST              15 ('x_unit')
                            764 COMPARE_OP               2 (==)
                            770 POP_JUMP_FORWARD_IF_FALSE    10 (to 792)
                
-               114         772 LOAD_FAST                5 (header_data)
+               113         772 LOAD_FAST                5 (header_data)
                            774 BUILD_LIST               1
                            776 LOAD_FAST                0 (self)
                            778 STORE_ATTR               3 (x_unit)
                            788 EXTENDED_ARG             1
                            790 JUMP_BACKWARD          313 (to 166)
                
-               115     >>  792 LOAD_FAST                4 (header_label)
+               114     >>  792 LOAD_FAST                4 (header_label)
                            794 LOAD_CONST              16 ('x_label')
                            796 COMPARE_OP               2 (==)
                            802 POP_JUMP_FORWARD_IF_FALSE     8 (to 820)
                
-               116         804 LOAD_FAST                5 (header_data)
+               115         804 LOAD_FAST                5 (header_data)
                            806 BUILD_LIST               1
                            808 LOAD_FAST                0 (self)
                            810 STORE_ATTR              20 (x_label)
                        >>  820 EXTENDED_ARG             1
                            822 JUMP_BACKWARD          329 (to 166)
                
-               118     >>  824 LOAD_FAST                0 (self)
+               117     >>  824 LOAD_FAST                0 (self)
                            826 LOAD_ATTR               21 (y_data)
                            836 LOAD_ATTR               22 (shape)
                            846 LOAD_CONST              17 (2)
                            848 BINARY_SUBSCR
                            858 LOAD_CONST               2 (0)
                            860 COMPARE_OP               4 (>)
                            866 POP_JUMP_FORWARD_IF_FALSE   109 (to 1086)
                
-               119         868 LOAD_GLOBAL             47 (NULL + np)
+               118         868 LOAD_GLOBAL             47 (NULL + np)
                            880 LOAD_ATTR               24 (append)
                            890 LOAD_FAST                0 (self)
                            892 LOAD_ATTR               21 (y_data)
                
-               120         902 LOAD_GLOBAL             47 (NULL + np)
+               119         902 LOAD_GLOBAL             47 (NULL + np)
                            914 LOAD_ATTR               25 (reshape)
                            924 LOAD_GLOBAL             47 (NULL + np)
                            936 LOAD_ATTR               26 (array)
-                           946 LOAD_CONST              18 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 120>)
+                           946 LOAD_CONST              18 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 119>)
                            948 MAKE_FUNCTION            0
                            950 LOAD_FAST                3 (l)
                            952 LOAD_METHOD              9 (split)
                            974 LOAD_CONST              19 (',')
                            976 PRECALL                  1
                            980 CALL                     1
                            990 GET_ITER
@@ -782,85 +774,85 @@
                           1022 LOAD_CONST               1 (1)
                           1024 LOAD_FAST                0 (self)
                           1026 LOAD_ATTR                2 (sweep_points)
                           1036 BUILD_TUPLE              3
                           1038 PRECALL                  2
                           1042 CALL                     2
                
-               121        1052 LOAD_CONST               1 (1)
+               120        1052 LOAD_CONST               1 (1)
                
-               119        1054 KW_NAMES                20
+               118        1054 KW_NAMES                20
                           1056 PRECALL                  3
                           1060 CALL                     3
                           1070 LOAD_FAST                0 (self)
                           1072 STORE_ATTR              21 (y_data)
                           1082 EXTENDED_ARG             1
                           1084 JUMP_BACKWARD          460 (to 166)
                
-               123     >> 1086 LOAD_CONST              21 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 123>)
+               122     >> 1086 LOAD_CONST              21 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 122>)
                           1088 MAKE_FUNCTION            0
                           1090 LOAD_FAST                3 (l)
                           1092 LOAD_METHOD              9 (split)
                           1114 LOAD_CONST              19 (',')
                           1116 PRECALL                  1
                           1120 CALL                     1
                           1130 GET_ITER
                           1132 PRECALL                  0
                           1136 CALL                     0
                           1146 STORE_FAST               7 (ys)
                
-               124        1148 LOAD_FAST                0 (self)
+               123        1148 LOAD_FAST                0 (self)
                           1150 LOAD_ATTR                2 (sweep_points)
                           1160 LOAD_CONST               2 (0)
                           1162 COMPARE_OP               2 (==)
                           1168 POP_JUMP_FORWARD_IF_FALSE    20 (to 1210)
                
-               125        1170 LOAD_GLOBAL             29 (NULL + len)
+               124        1170 LOAD_GLOBAL             29 (NULL + len)
                           1182 LOAD_FAST                7 (ys)
                           1184 PRECALL                  1
                           1188 CALL                     1
                           1198 LOAD_FAST                0 (self)
                           1200 STORE_ATTR               2 (sweep_points)
                
-               126     >> 1210 LOAD_GLOBAL             47 (NULL + np)
+               125     >> 1210 LOAD_GLOBAL             47 (NULL + np)
                           1222 LOAD_ATTR               25 (reshape)
                           1232 LOAD_GLOBAL             47 (NULL + np)
                           1244 LOAD_ATTR               26 (array)
                           1254 LOAD_FAST                7 (ys)
                           1256 PRECALL                  1
                           1260 CALL                     1
                
-               127        1270 LOAD_CONST               1 (1)
+               126        1270 LOAD_CONST               1 (1)
                           1272 LOAD_CONST               1 (1)
                           1274 LOAD_FAST                0 (self)
                           1276 LOAD_ATTR                2 (sweep_points)
                           1286 BUILD_TUPLE              3
                
-               126        1288 PRECALL                  2
+               125        1288 PRECALL                  2
                           1292 CALL                     2
                           1302 LOAD_FAST                0 (self)
                           1304 STORE_ATTR              21 (y_data)
                           1314 EXTENDED_ARG             2
                           1316 JUMP_BACKWARD          576 (to 166)
                
-               128     >> 1318 LOAD_FAST                0 (self)
+               127     >> 1318 LOAD_FAST                0 (self)
                           1320 LOAD_ATTR                1 (sweep_count)
                           1330 LOAD_CONST               2 (0)
                           1332 COMPARE_OP               2 (==)
                           1338 POP_JUMP_FORWARD_IF_FALSE    23 (to 1386)
                
-               129        1340 LOAD_FAST                0 (self)
+               128        1340 LOAD_FAST                0 (self)
                           1342 LOAD_ATTR               21 (y_data)
                           1352 LOAD_ATTR               22 (shape)
                           1362 LOAD_CONST               1 (1)
                           1364 BINARY_SUBSCR
                           1374 LOAD_FAST                0 (self)
                           1376 STORE_ATTR               1 (sweep_count)
                
-                90     >> 1386 LOAD_CONST               7 (None)
+                89     >> 1386 LOAD_CONST               7 (None)
                           1388 LOAD_CONST               7 (None)
                           1390 LOAD_CONST               7 (None)
                           1392 PRECALL                  2
                           1396 CALL                     2
                           1406 POP_TOP
                           1408 LOAD_CONST               7 (None)
                           1410 RETURN_VALUE
@@ -904,15 +896,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017401000000000000000000007c01a6010000ab
                         01000000000000000091028c125300
-                     120           0 RESUME                   0
+                     119           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                17 (to 42)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_GLOBAL              1 (NULL + float)
                                   22 LOAD_FAST                1 (i)
                                   24 PRECALL                  1
@@ -923,27 +915,27 @@
                      consts
                      names      ('float',)
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 120
+                     firstlineno 119
                      lnotab 0x
                   ','
                   ('axis',)
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017401000000000000000000007c01a6010000ab
                         01000000000000000091028c125300
-                     123           0 RESUME                   0
+                     122           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                17 (to 42)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_GLOBAL              1 (NULL + float)
                                   22 LOAD_FAST                1 (i)
                                   24 PRECALL                  1
@@ -954,23 +946,23 @@
                      consts
                      names      ('float',)
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 123
+                     firstlineno 122
                      lnotab 0x
                names      ('channel_count', 'sweep_count', 'sweep_points', 'x_unit', 'y_unit', 'y_label', 'open', 'readlines', 'strip', 'split', 'int', 'original_sweep_count', 'float', 'sampling_rate', 'len', 'str', 'x_sigdig', 'x_interval', 'channel_units', 'channel_labels', 'x_label', 'y_data', 'shape', 'np', 'append', 'reshape', 'array')
                varnames   ('self', 'filename', 'f', 'l', 'header_label', 'header_data', 'version', 'ys')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'read_csv'
-               firstlineno 80
+               firstlineno 79
                lnotab
                   0x02040e010e010e0110011001100122012e0128011a01460146010c0106
                   010c0128011a010c012a010c012802520222010c0114010c0114010c0114
                   010c0114022c012201960102fe20043e01160128013c0112ff1e0216012e
                   d9
             None
             0
@@ -995,37 +987,37 @@
                   0e0000000000000000000082017406000000000000000000006a04000000
                   0000000000a00800000000000000000000000000000000000000007c05a6
                   010000ab0100000000000000006406190000000000000000007d067c0664
                   076b020000000072177c00a0090000000000000000000000000000000000
                   0000007c05a6010000ab0100000000000000000100640053007c0664086b
                   020000000072187c00a00a00000000000000000000000000000000000000
                   007c057c02a6020000ab02000000000000000001006400530064005300
-               131           0 RESUME                   0
+               130           0 RESUME                   0
                
-               132           2 LOAD_FAST                2 (channels)
+               131           2 LOAD_FAST                2 (channels)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE    30 (to 66)
                
-               133           6 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 133>)
+               132           6 LOAD_CONST               1 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 132>)
                              8 MAKE_FUNCTION            0
                             10 LOAD_GLOBAL              1 (NULL + range)
                             22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                1 (channel_count)
                             34 PRECALL                  1
                             38 CALL                     1
                             48 GET_ITER
                             50 PRECALL                  0
                             54 CALL                     0
                             64 STORE_FAST               2 (channels)
                
-               134     >>   66 LOAD_FAST                3 (suffix)
+               133     >>   66 LOAD_FAST                3 (suffix)
                             68 LOAD_CONST               2 (0)
                             70 COMPARE_OP               4 (>)
                             76 POP_JUMP_FORWARD_IF_FALSE    61 (to 200)
                
-               135          78 LOAD_FAST                1 (filename)
+               134          78 LOAD_FAST                1 (filename)
                             80 LOAD_METHOD              2 (split)
                            102 LOAD_CONST               3 ('.')
                            104 PRECALL                  1
                            108 CALL                     1
                            118 LOAD_CONST               2 (0)
                            120 BINARY_SUBSCR
                            130 FORMAT_VALUE             0
@@ -1041,96 +1033,96 @@
                            180 LOAD_CONST               6 (1)
                            182 BINARY_SUBSCR
                            192 FORMAT_VALUE             0
                            194 BUILD_STRING             5
                            196 STORE_FAST               5 (fname)
                            198 JUMP_FORWARD             2 (to 204)
                
-               137     >>  200 LOAD_FAST                1 (filename)
+               136     >>  200 LOAD_FAST                1 (filename)
                            202 STORE_FAST               5 (fname)
                
-               138     >>  204 LOAD_GLOBAL              6 (os)
+               137     >>  204 LOAD_GLOBAL              6 (os)
                            216 LOAD_ATTR                4 (path)
                            226 LOAD_METHOD              5 (exists)
                            248 LOAD_FAST                5 (fname)
                            250 PRECALL                  1
                            254 CALL                     1
                            264 POP_JUMP_FORWARD_IF_FALSE    38 (to 342)
                
-               139         266 LOAD_FAST                4 (handle_error)
+               138         266 LOAD_FAST                4 (handle_error)
                            268 POP_JUMP_FORWARD_IF_FALSE    29 (to 328)
                
-               140         270 LOAD_FAST                0 (self)
+               139         270 LOAD_FAST                0 (self)
                            272 LOAD_METHOD              6 (save)
                            294 LOAD_FAST                1 (filename)
                            296 LOAD_FAST                2 (channels)
                            298 LOAD_FAST                3 (suffix)
                            300 LOAD_CONST               6 (1)
                            302 BINARY_OP                0 (+)
                            306 LOAD_FAST                4 (handle_error)
                            308 PRECALL                  4
                            312 CALL                     4
                            322 POP_TOP
                
-               141         324 LOAD_CONST               0 (None)
+               140         324 LOAD_CONST               0 (None)
                            326 RETURN_VALUE
                
-               143     >>  328 LOAD_GLOBAL             14 (FileExistsError)
+               142     >>  328 LOAD_GLOBAL             14 (FileExistsError)
                            340 RAISE_VARARGS            1
                
-               144     >>  342 LOAD_GLOBAL              6 (os)
+               143     >>  342 LOAD_GLOBAL              6 (os)
                            354 LOAD_ATTR                4 (path)
                            364 LOAD_METHOD              8 (splitext)
                            386 LOAD_FAST                5 (fname)
                            388 PRECALL                  1
                            392 CALL                     1
                            402 LOAD_CONST               6 (1)
                            404 BINARY_SUBSCR
                            414 STORE_FAST               6 (filetype)
                
-               145         416 LOAD_FAST                6 (filetype)
+               144         416 LOAD_FAST                6 (filetype)
                            418 LOAD_CONST               7 ('.abf')
                            420 COMPARE_OP               2 (==)
                            426 POP_JUMP_FORWARD_IF_FALSE    23 (to 474)
                
-               146         428 LOAD_FAST                0 (self)
+               145         428 LOAD_FAST                0 (self)
                            430 LOAD_METHOD              9 (write_abf)
                            452 LOAD_FAST                5 (fname)
                            454 PRECALL                  1
                            458 CALL                     1
                            468 POP_TOP
                            470 LOAD_CONST               0 (None)
                            472 RETURN_VALUE
                
-               147     >>  474 LOAD_FAST                6 (filetype)
+               146     >>  474 LOAD_FAST                6 (filetype)
                            476 LOAD_CONST               8 ('.csv')
                            478 COMPARE_OP               2 (==)
                            484 POP_JUMP_FORWARD_IF_FALSE    24 (to 534)
                
-               148         486 LOAD_FAST                0 (self)
+               147         486 LOAD_FAST                0 (self)
                            488 LOAD_METHOD             10 (write_csv)
                            510 LOAD_FAST                5 (fname)
                            512 LOAD_FAST                2 (channels)
                            514 PRECALL                  2
                            518 CALL                     2
                            528 POP_TOP
                            530 LOAD_CONST               0 (None)
                            532 RETURN_VALUE
                
-               147     >>  534 LOAD_CONST               0 (None)
+               146     >>  534 LOAD_CONST               0 (None)
                            536 RETURN_VALUE
                consts
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     133           0 RESUME                   0
+                     132           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_FAST                1 (i)
                                   12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
@@ -1138,46 +1130,46 @@
                      consts
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 133
+                     firstlineno 132
                      lnotab 0x
                   0
                   '.'
                   '('
                   ').'
                   1
                   '.abf'
                   '.csv'
                names      ('range', 'channel_count', 'split', 'os', 'path', 'exists', 'save', 'FileExistsError', 'splitext', 'write_abf', 'write_csv')
                varnames   ('self', 'filename', 'channels', 'suffix', 'handle_error', 'fname', 'filetype')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'save'
-               firstlineno 131
+               firstlineno 130
                lnotab
                   0x020104013c010c017a0204013e010401360104020e014a010c012e010c
                   0130ff
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000006a0100000000000000007c006a0200
                   000000000000007c017c006a0300000000000000007c006a040000000000
                   0000007c006a050000000000000000ac01a6050000ab0500000000000000
                   00010064005300
-               149           0 RESUME                   0
+               148           0 RESUME                   0
                
-               150           2 LOAD_GLOBAL              1 (NULL + abfWriter)
+               149           2 LOAD_GLOBAL              1 (NULL + abfWriter)
                             14 LOAD_ATTR                1 (writeABF1)
                             24 LOAD_FAST                0 (self)
                             26 LOAD_ATTR                2 (y_data)
                             36 LOAD_FAST                1 (filename)
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                3 (sampling_rate)
                             50 LOAD_FAST                0 (self)
@@ -1195,15 +1187,15 @@
                   ('sampleRateHz', 'units', 'labels')
                names      ('abfWriter', 'writeABF1', 'y_data', 'sampling_rate', 'channel_units', 'channel_labels')
                varnames   ('self', 'filename')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'write_abf'
-               firstlineno 149
+               firstlineno 148
                lnotab 0x0201
             code
                argcount  : 3
                nlocals   : 5
                stacksize : 12
                flags     : 3
                code
@@ -1233,145 +1225,145 @@
                   000000000000000000a00f00000000000000000000000000000000000000
                   00a6000000ab0000000000000000004400a6000000ab0000000000000000
                   00a6010000ab010000000000000000a6010000ab01000000000000000001
                   007c03a00200000000000000000000000000000000000000006403a60100
                   00ab01000000000000000001008c6c0900640064006400a6020000ab0200
                   000000000000000100640053002300310073047702780359007701010059
                   000100010064005300
-               153           0 RESUME                   0
+               152           0 RESUME                   0
                
-               154           2 LOAD_FAST                2 (channel)
+               153           2 LOAD_FAST                2 (channel)
                              4 POP_JUMP_FORWARD_IF_NOT_NONE     7 (to 20)
                
-               155           6 LOAD_FAST                0 (self)
+               154           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (channel)
                             18 STORE_FAST               2 (channel)
                
-               156     >>   20 LOAD_GLOBAL              3 (NULL + open)
+               155     >>   20 LOAD_GLOBAL              3 (NULL + open)
                             32 LOAD_FAST                1 (filename)
                             34 LOAD_CONST               1 ('x')
                             36 PRECALL                  2
                             40 CALL                     2
                             50 BEFORE_WITH
                             52 STORE_FAST               3 (f)
                
-               157          54 LOAD_FAST                3 (f)
+               156          54 LOAD_FAST                3 (f)
                             56 LOAD_METHOD              2 (write)
                             78 LOAD_CONST               2 ('@version=')
                             80 LOAD_GLOBAL              6 (config)
                             92 LOAD_ATTR                4 (version)
                            102 FORMAT_VALUE             0
                            104 LOAD_CONST               3 ('\n')
                            106 BUILD_STRING             3
                            108 PRECALL                  1
                            112 CALL                     1
                            122 POP_TOP
                
-               158         124 LOAD_FAST                3 (f)
+               157         124 LOAD_FAST                3 (f)
                            126 LOAD_METHOD              2 (write)
                            148 LOAD_CONST               4 ('@sweep_count=')
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                5 (sweep_count)
                            162 FORMAT_VALUE             0
                            164 LOAD_CONST               3 ('\n')
                            166 BUILD_STRING             3
                            168 PRECALL                  1
                            172 CALL                     1
                            182 POP_TOP
                
-               159         184 LOAD_FAST                3 (f)
+               158         184 LOAD_FAST                3 (f)
                            186 LOAD_METHOD              2 (write)
                            208 LOAD_CONST               5 ('@sweep_points=')
                            210 LOAD_FAST                0 (self)
                            212 LOAD_ATTR                6 (sweep_points)
                            222 FORMAT_VALUE             0
                            224 LOAD_CONST               3 ('\n')
                            226 BUILD_STRING             3
                            228 PRECALL                  1
                            232 CALL                     1
                            242 POP_TOP
                
-               160         244 LOAD_FAST                3 (f)
+               159         244 LOAD_FAST                3 (f)
                            246 LOAD_METHOD              2 (write)
                            268 LOAD_CONST               6 ('@channel_unit=')
                            270 LOAD_FAST                0 (self)
                            272 LOAD_ATTR                7 (channel_units)
                            282 LOAD_FAST                2 (channel)
                            284 BINARY_SUBSCR
                            294 FORMAT_VALUE             0
                            296 LOAD_CONST               3 ('\n')
                            298 BUILD_STRING             3
                            300 PRECALL                  1
                            304 CALL                     1
                            314 POP_TOP
                
-               161         316 LOAD_FAST                3 (f)
+               160         316 LOAD_FAST                3 (f)
                            318 LOAD_METHOD              2 (write)
                            340 LOAD_CONST               7 ('@channel_label=')
                            342 LOAD_FAST                0 (self)
                            344 LOAD_ATTR                8 (channel_labels)
                            354 LOAD_FAST                2 (channel)
                            356 BINARY_SUBSCR
                            366 FORMAT_VALUE             0
                            368 LOAD_CONST               3 ('\n')
                            370 BUILD_STRING             3
                            372 PRECALL                  1
                            376 CALL                     1
                            386 POP_TOP
                
-               162         388 LOAD_FAST                3 (f)
+               161         388 LOAD_FAST                3 (f)
                            390 LOAD_METHOD              2 (write)
                            412 LOAD_CONST               8 ('@sampling_rate=')
                            414 LOAD_FAST                0 (self)
                            416 LOAD_ATTR                9 (sampling_rate)
                            426 FORMAT_VALUE             0
                            428 LOAD_CONST               3 ('\n')
                            430 BUILD_STRING             3
                            432 PRECALL                  1
                            436 CALL                     1
                            446 POP_TOP
                
-               163         448 LOAD_FAST                3 (f)
+               162         448 LOAD_FAST                3 (f)
                            450 LOAD_METHOD              2 (write)
                            472 LOAD_CONST               9 ('@x_unit=')
                            474 LOAD_FAST                0 (self)
                            476 LOAD_ATTR               10 (x_unit)
                            486 FORMAT_VALUE             0
                            488 LOAD_CONST               3 ('\n')
                            490 BUILD_STRING             3
                            492 PRECALL                  1
                            496 CALL                     1
                            506 POP_TOP
                
-               164         508 LOAD_FAST                3 (f)
+               163         508 LOAD_FAST                3 (f)
                            510 LOAD_METHOD              2 (write)
                            532 LOAD_CONST              10 ('@x_label=')
                            534 LOAD_FAST                0 (self)
                            536 LOAD_ATTR               11 (x_label)
                            546 FORMAT_VALUE             0
                            548 LOAD_CONST               3 ('\n')
                            550 BUILD_STRING             3
                            552 PRECALL                  1
                            556 CALL                     1
                            566 POP_TOP
                
-               165         568 LOAD_GLOBAL             25 (NULL + range)
+               164         568 LOAD_GLOBAL             25 (NULL + range)
                            580 LOAD_FAST                0 (self)
                            582 LOAD_ATTR                5 (sweep_count)
                            592 PRECALL                  1
                            596 CALL                     1
                            606 GET_ITER
                        >>  608 FOR_ITER               107 (to 824)
                            610 STORE_FAST               4 (s)
                
-               166         612 LOAD_FAST                3 (f)
+               165         612 LOAD_FAST                3 (f)
                            614 LOAD_METHOD              2 (write)
                            636 LOAD_CONST              11 (',')
                            638 LOAD_METHOD             13 (join)
-                           660 LOAD_CONST              12 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 166>)
+                           660 LOAD_CONST              12 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 165>)
                            662 MAKE_FUNCTION            0
                            664 LOAD_FAST                0 (self)
                            666 LOAD_ATTR               14 (y_data)
                            676 LOAD_FAST                2 (channel)
                            678 LOAD_FAST                4 (s)
                            680 LOAD_CONST               0 (None)
                            682 LOAD_CONST               0 (None)
@@ -1386,25 +1378,25 @@
                            740 CALL                     0
                            750 PRECALL                  1
                            754 CALL                     1
                            764 PRECALL                  1
                            768 CALL                     1
                            778 POP_TOP
                
-               167         780 LOAD_FAST                3 (f)
+               166         780 LOAD_FAST                3 (f)
                            782 LOAD_METHOD              2 (write)
                            804 LOAD_CONST               3 ('\n')
                            806 PRECALL                  1
                            810 CALL                     1
                            820 POP_TOP
                            822 JUMP_BACKWARD          108 (to 608)
                
-               165     >>  824 NOP
+               164     >>  824 NOP
                
-               156         826 LOAD_CONST               0 (None)
+               155         826 LOAD_CONST               0 (None)
                            828 LOAD_CONST               0 (None)
                            830 LOAD_CONST               0 (None)
                            832 PRECALL                  2
                            836 CALL                     2
                            846 POP_TOP
                            848 LOAD_CONST               0 (None)
                            850 RETURN_VALUE
@@ -1442,15 +1434,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017401000000000000000000007c01a6010000ab
                         01000000000000000091028c125300
-                     166           0 RESUME                   0
+                     165           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                17 (to 42)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_GLOBAL              1 (NULL + str)
                                   22 LOAD_FAST                1 (i)
                                   24 PRECALL                  1
@@ -1461,66 +1453,66 @@
                      consts
                      names      ('str',)
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 166
+                     firstlineno 165
                      lnotab 0x
                names      ('channel', 'open', 'write', 'config', 'version', 'sweep_count', 'sweep_points', 'channel_units', 'channel_labels', 'sampling_rate', 'x_unit', 'x_label', 'range', 'join', 'y_data', 'tolist')
                varnames   ('self', 'filename', 'channel', 'f', 's')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'write_csv'
-               firstlineno 153
+               firstlineno 152
                lnotab
                   0x020104010e01220146013c013c01480148013c013c013c012c01a8012c
                   fe02f7
             code
                argcount  : 2
                nlocals   : 2
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a0000000000000000007c01190000000000000000007c005f
                   0100000000000000007c006a0200000000000000007c0119000000000000
                   0000007c005f0300000000000000007c017c005f04000000000000000064
                   005300
-               172           0 RESUME                   0
+               171           0 RESUME                   0
                
-               173           2 LOAD_FAST                0 (self)
+               172           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (channel_labels)
                             14 LOAD_FAST                1 (channel)
                             16 BINARY_SUBSCR
                             26 LOAD_FAST                0 (self)
                             28 STORE_ATTR               1 (y_label)
                
-               174          38 LOAD_FAST                0 (self)
+               173          38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (channel_units)
                             50 LOAD_FAST                1 (channel)
                             52 BINARY_SUBSCR
                             62 LOAD_FAST                0 (self)
                             64 STORE_ATTR               3 (y_unit)
                
-               178          74 LOAD_FAST                1 (channel)
+               177          74 LOAD_FAST                1 (channel)
                             76 LOAD_FAST                0 (self)
                             78 STORE_ATTR               4 (channel)
                             88 LOAD_CONST               0 (None)
                             90 RETURN_VALUE
                consts
                   None
                names      ('channel_labels', 'y_label', 'channel_units', 'y_unit', 'channel')
                varnames   ('self', 'channel')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'set_channel'
-               firstlineno 172
+               firstlineno 171
                lnotab 0x020124012404
             'continuous'
             True
             code
                argcount  : 6
                nlocals   : 9
                stacksize : 7
@@ -1550,95 +1542,95 @@
                   0200007d067d077c047c06190000000000000000007c006a080000000000
                   0000007c077c0364036403850266033c0000008c1b7c006a080000000000
                   00000053007c006a080000000000000000a0090000000000000000000000
                   000000000000000000a6000000ab0000000000000000007d08740f000000
                   000000000000007c02a6010000ab01000000000000000044005d155c0200
                   007d067d077c047c06190000000000000000007c087c077c036403640385
                   0266033c0000008c167c085300
-               181           0 RESUME                   0
+               180           0 RESUME                   0
                
-               190           2 LOAD_GLOBAL              1 (NULL + len)
+               189           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                4 (new_data)
                             16 LOAD_ATTR                1 (shape)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (3)
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_TRUE    10 (to 70)
                             50 LOAD_ASSERTION_ERROR
                             52 LOAD_CONST               2 ('Matrix shape mismatch - the input data must be a 3D numpy array')
                             54 PRECALL                  0
                             58 CALL                     0
                             68 RAISE_VARARGS            1
                
-               191     >>   70 LOAD_FAST                2 (channels)
+               190     >>   70 LOAD_FAST                2 (channels)
                             72 POP_JUMP_FORWARD_IF_NOT_NONE    26 (to 126)
                
-               192          74 LOAD_GLOBAL              5 (NULL + range)
+               191          74 LOAD_GLOBAL              5 (NULL + range)
                             86 LOAD_FAST                4 (new_data)
                             88 LOAD_ATTR                1 (shape)
                             98 LOAD_CONST               4 (0)
                            100 BINARY_SUBSCR
                            110 PRECALL                  1
                            114 CALL                     1
                            124 STORE_FAST               2 (channels)
                
-               194     >>  126 LOAD_FAST                1 (mode)
+               193     >>  126 LOAD_FAST                1 (mode)
                            128 LOAD_CONST               5 ('continuous')
                            130 COMPARE_OP               2 (==)
                            136 POP_JUMP_FORWARD_IF_FALSE   149 (to 436)
                
-               195         138 LOAD_FAST                4 (new_data)
+               194         138 LOAD_FAST                4 (new_data)
                            140 LOAD_ATTR                1 (shape)
                
-               196         150 LOAD_CONST               6 (2)
+               195         150 LOAD_CONST               6 (2)
                
-               195         152 BINARY_SUBSCR
+               194         152 BINARY_SUBSCR
                
-               196         162 LOAD_FAST                0 (self)
+               195         162 LOAD_FAST                0 (self)
                            164 LOAD_ATTR                3 (sweep_points)
                
-               195         174 BINARY_OP                6 (%)
+               194         174 BINARY_OP                6 (%)
                
-               196         178 LOAD_CONST               4 (0)
+               195         178 LOAD_CONST               4 (0)
                
-               195         180 COMPARE_OP               2 (==)
+               194         180 COMPARE_OP               2 (==)
                            186 POP_JUMP_FORWARD_IF_TRUE    19 (to 226)
                            188 LOAD_ASSERTION_ERROR
                
-               196         190 LOAD_CONST               7 ('Sweep length mismatch. Each sweep in "continuous" mode must be a multiple of ')
+               195         190 LOAD_CONST               7 ('Sweep length mismatch. Each sweep in "continuous" mode must be a multiple of ')
                            192 LOAD_FAST                0 (self)
                            194 LOAD_ATTR                3 (sweep_points)
                            204 FORMAT_VALUE             0
                            206 LOAD_CONST               8 (' datapoints')
                            208 BUILD_STRING             3
                
-               195         210 PRECALL                  0
+               194         210 PRECALL                  0
                            214 CALL                     0
                            224 RAISE_VARARGS            1
                
-               197     >>  226 LOAD_FAST                3 (sweeps)
+               196     >>  226 LOAD_FAST                3 (sweeps)
                            228 POP_JUMP_FORWARD_IF_NOT_NONE    47 (to 324)
                
-               198         230 LOAD_GLOBAL              5 (NULL + range)
+               197         230 LOAD_GLOBAL              5 (NULL + range)
                            242 LOAD_GLOBAL              9 (NULL + int)
                            254 LOAD_FAST                4 (new_data)
                            256 LOAD_ATTR                1 (shape)
                            266 LOAD_CONST               6 (2)
                            268 BINARY_SUBSCR
                            278 LOAD_FAST                0 (self)
                            280 LOAD_ATTR                3 (sweep_points)
                            290 BINARY_OP               11 (/)
                            294 PRECALL                  1
                            298 CALL                     1
                            308 PRECALL                  1
                            312 CALL                     1
                            322 STORE_FAST               3 (sweeps)
                
-               200     >>  324 LOAD_GLOBAL             11 (NULL + np)
+               199     >>  324 LOAD_GLOBAL             11 (NULL + np)
                            336 LOAD_ATTR                6 (reshape)
                            346 LOAD_FAST                4 (new_data)
                            348 LOAD_GLOBAL              1 (NULL + len)
                            360 LOAD_FAST                2 (channels)
                            362 PRECALL                  1
                            366 CALL                     1
                            376 LOAD_GLOBAL              1 (NULL + len)
@@ -1649,122 +1641,122 @@
                            406 LOAD_ATTR                3 (sweep_points)
                            416 BUILD_TUPLE              3
                            418 PRECALL                  2
                            422 CALL                     2
                            432 STORE_FAST               4 (new_data)
                            434 JUMP_FORWARD            78 (to 592)
                
-               202     >>  436 LOAD_FAST                1 (mode)
+               201     >>  436 LOAD_FAST                1 (mode)
                            438 LOAD_CONST               9 ('overlay')
                            440 COMPARE_OP               2 (==)
                            446 POP_JUMP_FORWARD_IF_FALSE    70 (to 588)
                
-               203         448 LOAD_FAST                4 (new_data)
+               202         448 LOAD_FAST                4 (new_data)
                            450 LOAD_ATTR                1 (shape)
                
-               204         460 LOAD_CONST               6 (2)
+               203         460 LOAD_CONST               6 (2)
                
-               203         462 BINARY_SUBSCR
+               202         462 BINARY_SUBSCR
                
-               204         472 LOAD_FAST                0 (self)
+               203         472 LOAD_FAST                0 (self)
                            474 LOAD_ATTR                3 (sweep_points)
                
-               203         484 COMPARE_OP               2 (==)
+               202         484 COMPARE_OP               2 (==)
                            490 POP_JUMP_FORWARD_IF_TRUE    19 (to 530)
                            492 LOAD_ASSERTION_ERROR
                
-               204         494 LOAD_CONST              10 ('Sweep length mismatch. Each sweep in "overlay" mode must be ')
+               203         494 LOAD_CONST              10 ('Sweep length mismatch. Each sweep in "overlay" mode must be ')
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR                3 (sweep_points)
                            508 FORMAT_VALUE             0
                            510 LOAD_CONST               8 (' datapoints')
                            512 BUILD_STRING             3
                
-               203         514 PRECALL                  0
+               202         514 PRECALL                  0
                            518 CALL                     0
                            528 RAISE_VARARGS            1
                
-               205     >>  530 LOAD_FAST                3 (sweeps)
+               204     >>  530 LOAD_FAST                3 (sweeps)
                            532 POP_JUMP_FORWARD_IF_NOT_NONE    26 (to 586)
                
-               206         534 LOAD_GLOBAL              5 (NULL + range)
+               205         534 LOAD_GLOBAL              5 (NULL + range)
                            546 LOAD_FAST                4 (new_data)
                            548 LOAD_ATTR                1 (shape)
                            558 LOAD_CONST              11 (1)
                            560 BINARY_SUBSCR
                            570 PRECALL                  1
                            574 CALL                     1
                            584 STORE_FAST               3 (sweeps)
                        >>  586 JUMP_FORWARD             2 (to 592)
                
-               208     >>  588 LOAD_CONST               3 (None)
+               207     >>  588 LOAD_CONST               3 (None)
                            590 RETURN_VALUE
                
-               209     >>  592 LOAD_FAST                5 (inplace)
+               208     >>  592 LOAD_FAST                5 (inplace)
                            594 POP_JUMP_FORWARD_IF_FALSE    49 (to 694)
                
-               210         596 LOAD_GLOBAL             15 (NULL + enumerate)
+               209         596 LOAD_GLOBAL             15 (NULL + enumerate)
                            608 LOAD_FAST                2 (channels)
                            610 PRECALL                  1
                            614 CALL                     1
                            624 GET_ITER
                        >>  626 FOR_ITER                26 (to 680)
                            628 UNPACK_SEQUENCE          2
                            632 STORE_FAST               6 (i)
                            634 STORE_FAST               7 (c)
                
-               211         636 LOAD_FAST                4 (new_data)
+               210         636 LOAD_FAST                4 (new_data)
                            638 LOAD_FAST                6 (i)
                            640 BINARY_SUBSCR
                            650 LOAD_FAST                0 (self)
                            652 LOAD_ATTR                8 (y_data)
                            662 LOAD_FAST                7 (c)
                            664 LOAD_FAST                3 (sweeps)
                            666 LOAD_CONST               3 (None)
                            668 LOAD_CONST               3 (None)
                            670 BUILD_SLICE              2
                            672 BUILD_TUPLE              3
                            674 STORE_SUBSCR
                            678 JUMP_BACKWARD           27 (to 626)
                
-               212     >>  680 LOAD_FAST                0 (self)
+               211     >>  680 LOAD_FAST                0 (self)
                            682 LOAD_ATTR                8 (y_data)
                            692 RETURN_VALUE
                
-               214     >>  694 LOAD_FAST                0 (self)
+               213     >>  694 LOAD_FAST                0 (self)
                            696 LOAD_ATTR                8 (y_data)
                            706 LOAD_METHOD              9 (copy)
                            728 PRECALL                  0
                            732 CALL                     0
                            742 STORE_FAST               8 (result)
                
-               215         744 LOAD_GLOBAL             15 (NULL + enumerate)
+               214         744 LOAD_GLOBAL             15 (NULL + enumerate)
                            756 LOAD_FAST                2 (channels)
                            758 PRECALL                  1
                            762 CALL                     1
                            772 GET_ITER
                        >>  774 FOR_ITER                21 (to 818)
                            776 UNPACK_SEQUENCE          2
                            780 STORE_FAST               6 (i)
                            782 STORE_FAST               7 (c)
                
-               216         784 LOAD_FAST                4 (new_data)
+               215         784 LOAD_FAST                4 (new_data)
                            786 LOAD_FAST                6 (i)
                            788 BINARY_SUBSCR
                            798 LOAD_FAST                8 (result)
                            800 LOAD_FAST                7 (c)
                            802 LOAD_FAST                3 (sweeps)
                            804 LOAD_CONST               3 (None)
                            806 LOAD_CONST               3 (None)
                            808 BUILD_SLICE              2
                            810 BUILD_TUPLE              3
                            812 STORE_SUBSCR
                            816 JUMP_BACKWARD           22 (to 774)
                
-               217     >>  818 LOAD_FAST                8 (result)
+               216     >>  818 LOAD_FAST                8 (result)
                            820 RETURN_VALUE
                consts
                   "\n        replaces y-values in specified sweeps and channels with data provided\n\n        mode: string {'continuous', 'overlay'} defaults to 'continuous'\n        channels: list of int - if None, defaults to first N channels that match the dimension of the input data\n        sweeps: list of int - only used for the 'overlay' plot_mode. If None, defaults to the first N sweeps that match the dimension of the input data\n        new_data: new y-values to replace. Must be a 3D float numpy array\n        "
                   3
                   'Matrix shape mismatch - the input data must be a 3D numpy array'
                   None
                   0
@@ -1777,15 +1769,15 @@
                   1
                names      ('len', 'shape', 'range', 'sweep_points', 'int', 'np', 'reshape', 'enumerate', 'y_data', 'copy')
                varnames   ('self', 'mode', 'channels', 'sweeps', 'new_data', 'inplace', 'i', 'c', 'result')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'replace_y_data'
-               firstlineno 181
+               firstlineno 180
                lnotab
                   0x02094401040134020c010c0102ff0a010cff040102ff0a0114ff100204
                   015e0270020c010c0102ff0a010cff0a0114ff1002040136020401040128
                   012c010e02320128012201
             code
                argcount  : 5
                nlocals   : 6
@@ -1836,101 +1828,101 @@
                   026603190000000000000000005300740b000000000000000000006408a6
                   010000ab01000000000000000001007c006a0600000000000000007c0319
                   0000000000000000006401640185027c0264016401850266031900000000
                   00000000007d05740b000000000000000000007c056a0700000000000000
                   00a6010000ab01000000000000000001007c006a0600000000000000007c
                   03190000000000000000006401640185027c026401640185026603190000
                   00000000000000530064015300
-               220           0 RESUME                   0
+               219           0 RESUME                   0
                
-               228           2 LOAD_FAST                3 (channels)
+               227           2 LOAD_FAST                3 (channels)
                              4 LOAD_CONST               1 (None)
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE    21 (to 56)
                
-               229          14 LOAD_GLOBAL              1 (NULL + range)
+               228          14 LOAD_GLOBAL              1 (NULL + range)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (channel_count)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (channels)
                             54 JUMP_FORWARD            27 (to 110)
                
-               230     >>   56 LOAD_GLOBAL              5 (NULL + type)
+               229     >>   56 LOAD_GLOBAL              5 (NULL + type)
                             68 LOAD_FAST                3 (channels)
                             70 PRECALL                  1
                             74 CALL                     1
                             84 LOAD_GLOBAL              6 (int)
                             96 COMPARE_OP               2 (==)
                            102 POP_JUMP_FORWARD_IF_FALSE     3 (to 110)
                
-               231         104 LOAD_FAST                3 (channels)
+               230         104 LOAD_FAST                3 (channels)
                            106 BUILD_LIST               1
                            108 STORE_FAST               3 (channels)
                
-               232     >>  110 LOAD_FAST                2 (sweeps)
+               231     >>  110 LOAD_FAST                2 (sweeps)
                            112 LOAD_CONST               1 (None)
                            114 COMPARE_OP               2 (==)
                            120 POP_JUMP_FORWARD_IF_FALSE    31 (to 184)
                
-               233         122 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 233>)
+               232         122 LOAD_CONST               2 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 232>)
                            124 MAKE_FUNCTION            0
                            126 LOAD_GLOBAL              1 (NULL + range)
                            138 LOAD_FAST                0 (self)
                            140 LOAD_ATTR                4 (sweep_count)
                            150 PRECALL                  1
                            154 CALL                     1
                            164 GET_ITER
                            166 PRECALL                  0
                            170 CALL                     0
                            180 STORE_FAST               2 (sweeps)
                            182 JUMP_FORWARD            27 (to 238)
                
-               234     >>  184 LOAD_GLOBAL              5 (NULL + type)
+               233     >>  184 LOAD_GLOBAL              5 (NULL + type)
                            196 LOAD_FAST                2 (sweeps)
                            198 PRECALL                  1
                            202 CALL                     1
                            212 LOAD_GLOBAL              6 (int)
                            224 COMPARE_OP               2 (==)
                            230 POP_JUMP_FORWARD_IF_FALSE     3 (to 238)
                
-               235         232 LOAD_FAST                2 (sweeps)
+               234         232 LOAD_FAST                2 (sweeps)
                            234 BUILD_LIST               1
                            236 STORE_FAST               2 (sweeps)
                
-               236     >>  238 LOAD_GLOBAL             11 (NULL + print)
+               235     >>  238 LOAD_GLOBAL             11 (NULL + print)
                            250 LOAD_FAST                3 (channels)
                            252 PRECALL                  1
                            256 CALL                     1
                            266 POP_TOP
                
-               237         268 LOAD_GLOBAL             11 (NULL + print)
+               236         268 LOAD_GLOBAL             11 (NULL + print)
                            280 LOAD_FAST                2 (sweeps)
                            282 PRECALL                  1
                            286 CALL                     1
                            296 POP_TOP
                
-               238         298 LOAD_GLOBAL             11 (NULL + print)
+               237         298 LOAD_GLOBAL             11 (NULL + print)
                            310 LOAD_FAST                0 (self)
                            312 LOAD_ATTR                6 (y_data)
                            322 LOAD_ATTR                7 (shape)
                            332 PRECALL                  1
                            336 CALL                     1
                            346 POP_TOP
                
-               240         348 LOAD_FAST                1 (mode)
+               239         348 LOAD_FAST                1 (mode)
                            350 LOAD_CONST               3 ('continuous')
                            352 COMPARE_OP               2 (==)
                            358 EXTENDED_ARG             1
                            360 POP_JUMP_FORWARD_IF_FALSE   279 (to 920)
                
-               241         362 LOAD_FAST                4 (xlim)
+               240         362 LOAD_FAST                4 (xlim)
                            364 POP_JUMP_FORWARD_IF_FALSE   195 (to 756)
                
-               242         366 LOAD_GLOBAL             17 (NULL + np)
+               241         366 LOAD_GLOBAL             17 (NULL + np)
                            378 LOAD_ATTR                9 (reshape)
                            388 LOAD_FAST                0 (self)
                            390 LOAD_ATTR                6 (y_data)
                            400 LOAD_FAST                3 (channels)
                            402 BINARY_SUBSCR
                            412 LOAD_CONST               1 (None)
                            414 LOAD_CONST               1 (None)
@@ -1938,32 +1930,32 @@
                            418 LOAD_FAST                2 (sweeps)
                            420 LOAD_CONST               1 (None)
                            422 LOAD_CONST               1 (None)
                            424 BUILD_SLICE              2
                            426 BUILD_TUPLE              3
                            428 BINARY_SUBSCR
                
-               243         438 LOAD_GLOBAL             21 (NULL + len)
+               242         438 LOAD_GLOBAL             21 (NULL + len)
                            450 LOAD_FAST                3 (channels)
                            452 PRECALL                  1
                            456 CALL                     1
                            466 LOAD_CONST               4 (1)
                            468 LOAD_GLOBAL             21 (NULL + len)
                            480 LOAD_FAST                2 (sweeps)
                            482 PRECALL                  1
                            486 CALL                     1
                            496 LOAD_FAST                0 (self)
                            498 LOAD_ATTR               11 (sweep_points)
                            508 BINARY_OP                5 (*)
                            512 BUILD_TUPLE              3
                
-               242         514 PRECALL                  2
+               241         514 PRECALL                  2
                            518 CALL                     2
                
-               244         528 LOAD_CONST               1 (None)
+               243         528 LOAD_CONST               1 (None)
                            530 LOAD_CONST               1 (None)
                            532 BUILD_SLICE              2
                            534 LOAD_CONST               1 (None)
                            536 LOAD_CONST               1 (None)
                            538 BUILD_SLICE              2
                            540 LOAD_GLOBAL             25 (NULL + max)
                            552 LOAD_CONST               5 (0)
@@ -1981,35 +1973,35 @@
                            624 LOAD_GLOBAL             29 (NULL + min)
                            636 LOAD_FAST                0 (self)
                            638 LOAD_ATTR                4 (sweep_count)
                            648 LOAD_FAST                0 (self)
                            650 LOAD_ATTR               11 (sweep_points)
                            660 BINARY_OP                5 (*)
                
-               245         664 LOAD_GLOBAL             31 (NULL + ceil)
+               244         664 LOAD_GLOBAL             31 (NULL + ceil)
                            676 LOAD_FAST                4 (xlim)
                            678 LOAD_CONST               4 (1)
                            680 BINARY_SUBSCR
                            690 LOAD_FAST                0 (self)
                            692 LOAD_ATTR               13 (x_interval)
                            702 BINARY_OP               11 (/)
                            706 PRECALL                  1
                            710 CALL                     1
                            720 LOAD_CONST               4 (1)
                            722 BINARY_OP                0 (+)
                
-               244         726 PRECALL                  2
+               243         726 PRECALL                  2
                            730 CALL                     2
                            740 BUILD_SLICE              2
                            742 BUILD_TUPLE              3
                
-               242         744 BINARY_SUBSCR
+               241         744 BINARY_SUBSCR
                            754 RETURN_VALUE
                
-               247     >>  756 LOAD_GLOBAL             17 (NULL + np)
+               246     >>  756 LOAD_GLOBAL             17 (NULL + np)
                            768 LOAD_ATTR                9 (reshape)
                            778 LOAD_FAST                0 (self)
                            780 LOAD_ATTR                6 (y_data)
                            790 LOAD_FAST                3 (channels)
                            792 BINARY_SUBSCR
                            802 LOAD_CONST               1 (None)
                            804 LOAD_CONST               1 (None)
@@ -2017,47 +2009,47 @@
                            808 LOAD_FAST                2 (sweeps)
                            810 LOAD_CONST               1 (None)
                            812 LOAD_CONST               1 (None)
                            814 BUILD_SLICE              2
                            816 BUILD_TUPLE              3
                            818 BINARY_SUBSCR
                
-               248         828 LOAD_GLOBAL             21 (NULL + len)
+               247         828 LOAD_GLOBAL             21 (NULL + len)
                            840 LOAD_FAST                3 (channels)
                            842 PRECALL                  1
                            846 CALL                     1
                            856 LOAD_CONST               4 (1)
                            858 LOAD_GLOBAL             21 (NULL + len)
                            870 LOAD_FAST                2 (sweeps)
                            872 PRECALL                  1
                            876 CALL                     1
                            886 LOAD_FAST                0 (self)
                            888 LOAD_ATTR               11 (sweep_points)
                            898 BINARY_OP                5 (*)
                            902 BUILD_TUPLE              3
                
-               247         904 PRECALL                  2
+               246         904 PRECALL                  2
                            908 CALL                     2
                            918 RETURN_VALUE
                
-               249     >>  920 LOAD_FAST                1 (mode)
+               248     >>  920 LOAD_FAST                1 (mode)
                            922 LOAD_CONST               6 ('overlay')
                            924 COMPARE_OP               2 (==)
                            930 POP_JUMP_FORWARD_IF_FALSE   243 (to 1418)
                
-               250         932 LOAD_FAST                4 (xlim)
+               249         932 LOAD_FAST                4 (xlim)
                            934 POP_JUMP_FORWARD_IF_FALSE   154 (to 1244)
                
-               251         936 LOAD_GLOBAL             11 (NULL + print)
+               250         936 LOAD_GLOBAL             11 (NULL + print)
                            948 LOAD_CONST               7 ('xlim overlay')
                            950 PRECALL                  1
                            954 CALL                     1
                            964 POP_TOP
                
-               252         966 LOAD_FAST                0 (self)
+               251         966 LOAD_FAST                0 (self)
                            968 LOAD_ATTR                6 (y_data)
                            978 LOAD_FAST                3 (channels)
                            980 BINARY_SUBSCR
                            990 LOAD_CONST               1 (None)
                            992 LOAD_CONST               1 (None)
                            994 BUILD_SLICE              2
                            996 LOAD_FAST                2 (sweeps)
@@ -2069,15 +2061,15 @@
                           1016 LOAD_CONST               1 (None)
                           1018 LOAD_CONST               1 (None)
                           1020 BUILD_SLICE              2
                           1022 LOAD_CONST               1 (None)
                           1024 LOAD_CONST               1 (None)
                           1026 BUILD_SLICE              2
                
-               253        1028 LOAD_GLOBAL             25 (NULL + max)
+               252        1028 LOAD_GLOBAL             25 (NULL + max)
                           1040 LOAD_CONST               5 (0)
                           1042 LOAD_GLOBAL              7 (NULL + int)
                           1054 LOAD_FAST                4 (xlim)
                           1056 LOAD_CONST               5 (0)
                           1058 BINARY_SUBSCR
                           1068 LOAD_FAST                0 (self)
                           1070 LOAD_ATTR               13 (x_interval)
@@ -2089,89 +2081,89 @@
                           1112 LOAD_GLOBAL             29 (NULL + min)
                           1124 LOAD_FAST                0 (self)
                           1126 LOAD_ATTR                4 (sweep_count)
                           1136 LOAD_FAST                0 (self)
                           1138 LOAD_ATTR               11 (sweep_points)
                           1148 BINARY_OP                5 (*)
                
-               254        1152 LOAD_GLOBAL             31 (NULL + ceil)
+               253        1152 LOAD_GLOBAL             31 (NULL + ceil)
                           1164 LOAD_FAST                4 (xlim)
                           1166 LOAD_CONST               4 (1)
                           1168 BINARY_SUBSCR
                           1178 LOAD_FAST                0 (self)
                           1180 LOAD_ATTR               13 (x_interval)
                           1190 BINARY_OP               11 (/)
                           1194 PRECALL                  1
                           1198 CALL                     1
                           1208 LOAD_CONST               4 (1)
                           1210 BINARY_OP                0 (+)
                
-               253        1214 PRECALL                  2
+               252        1214 PRECALL                  2
                           1218 CALL                     2
                           1228 BUILD_SLICE              2
                
-               252        1230 BUILD_TUPLE              3
+               251        1230 BUILD_TUPLE              3
                           1232 BINARY_SUBSCR
                           1242 RETURN_VALUE
                
-               256     >> 1244 LOAD_GLOBAL             11 (NULL + print)
+               255     >> 1244 LOAD_GLOBAL             11 (NULL + print)
                           1256 LOAD_CONST               8 ('no xlim overlay')
                           1258 PRECALL                  1
                           1262 CALL                     1
                           1272 POP_TOP
                
-               257        1274 LOAD_FAST                0 (self)
+               256        1274 LOAD_FAST                0 (self)
                           1276 LOAD_ATTR                6 (y_data)
                           1286 LOAD_FAST                3 (channels)
                           1288 BINARY_SUBSCR
                           1298 LOAD_CONST               1 (None)
                           1300 LOAD_CONST               1 (None)
                           1302 BUILD_SLICE              2
                           1304 LOAD_FAST                2 (sweeps)
                           1306 LOAD_CONST               1 (None)
                           1308 LOAD_CONST               1 (None)
                           1310 BUILD_SLICE              2
                           1312 BUILD_TUPLE              3
                           1314 BINARY_SUBSCR
                           1324 STORE_FAST               5 (return_val)
                
-               258        1326 LOAD_GLOBAL             11 (NULL + print)
+               257        1326 LOAD_GLOBAL             11 (NULL + print)
                           1338 LOAD_FAST                5 (return_val)
                           1340 LOAD_ATTR                7 (shape)
                           1350 PRECALL                  1
                           1354 CALL                     1
                           1364 POP_TOP
                
-               259        1366 LOAD_FAST                0 (self)
+               258        1366 LOAD_FAST                0 (self)
                           1368 LOAD_ATTR                6 (y_data)
                           1378 LOAD_FAST                3 (channels)
                           1380 BINARY_SUBSCR
                           1390 LOAD_CONST               1 (None)
                           1392 LOAD_CONST               1 (None)
                           1394 BUILD_SLICE              2
                           1396 LOAD_FAST                2 (sweeps)
                           1398 LOAD_CONST               1 (None)
                           1400 LOAD_CONST               1 (None)
                           1402 BUILD_SLICE              2
                           1404 BUILD_TUPLE              3
                           1406 BINARY_SUBSCR
                           1416 RETURN_VALUE
                
-               249     >> 1418 LOAD_CONST               1 (None)
+               248     >> 1418 LOAD_CONST               1 (None)
                           1420 RETURN_VALUE
                consts
                   "\n        returns a slice of the y_data\n        mode: 'continuous' or 'overlay'\n        channels: list of int - if None, defaults to all channels\n        sweeps: list of int - If None, defaults to all sweeps\n        xlim: float tuple [left, right] - If None, defaults to all data points in each sweep\n        "
                   None
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     233           0 RESUME                   0
+                     232           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                                    8 STORE_FAST               1 (i)
                                   10 LOAD_FAST                1 (i)
                                   12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
@@ -2179,29 +2171,29 @@
                      consts
                      names      ()
                      varnames   ('.0', 'i')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 233
+                     firstlineno 232
                      lnotab 0x
                   'continuous'
                   1
                   0
                   'overlay'
                   'xlim overlay'
                   'no xlim overlay'
                names      ('range', 'channel_count', 'type', 'int', 'sweep_count', 'print', 'y_data', 'shape', 'np', 'reshape', 'len', 'sweep_points', 'max', 'x_interval', 'min', 'ceil')
                varnames   ('self', 'mode', 'sweeps', 'channels', 'xlim', 'return_val')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'get_y_matrix'
-               firstlineno 220
+               firstlineno 219
                lnotab
                   0x02080c012a01300106010c013e01300106011e011e0132020e01040148
                   014cff0e0288013eff12fe0c0548014cff10020c0104011e013e017c013e
                   ff10ff0e041e013401280134f6
             code
                argcount  : 5
                nlocals   : 10
@@ -2248,53 +2240,53 @@
                   006a0a000000000000000064037c006a07000000000000000064047a0a00
                   007c006a0400000000000000007a0500007c006a070000000000000000a6
                   030000ab0300000000000000007d097413000000000000000000006a0e00
                   000000000000007c097419000000000000000000007c02a6010000ab0100
                   000000000000007419000000000000000000007c03a6010000ab01000000
                   00000000007a05000066017c096a0f00000000000000007a000000a60200
                   00ab020000000000000000530064015300
-               261           0 RESUME                   0
+               260           0 RESUME                   0
                
-               269           2 LOAD_FAST                3 (channels)
+               268           2 LOAD_FAST                3 (channels)
                              4 LOAD_CONST               1 (None)
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE    20 (to 54)
                
-               270          14 LOAD_GLOBAL              1 (NULL + range)
+               269          14 LOAD_GLOBAL              1 (NULL + range)
                             26 LOAD_FAST                0 (self)
                             28 LOAD_ATTR                1 (channel_count)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (channels)
                
-               272     >>   54 LOAD_FAST                1 (mode)
+               271     >>   54 LOAD_FAST                1 (mode)
                             56 LOAD_CONST               2 ('continuous')
                             58 COMPARE_OP               2 (==)
                             64 EXTENDED_ARG             1
                             66 POP_JUMP_FORWARD_IF_FALSE   360 (to 788)
                
-               273          68 LOAD_FAST                4 (xlim)
+               272          68 LOAD_FAST                4 (xlim)
                             70 POP_JUMP_FORWARD_IF_FALSE   146 (to 364)
                
-               274          72 LOAD_GLOBAL              5 (NULL + max)
+               273          72 LOAD_GLOBAL              5 (NULL + max)
                             84 LOAD_CONST               3 (0)
                             86 LOAD_GLOBAL              7 (NULL + int)
                             98 LOAD_FAST                4 (xlim)
                            100 LOAD_CONST               3 (0)
                            102 BINARY_SUBSCR
                            112 LOAD_FAST                0 (self)
                            114 LOAD_ATTR                4 (x_interval)
                            124 BINARY_OP               11 (/)
                            128 PRECALL                  1
                            132 CALL                     1
                            142 PRECALL                  2
                            146 CALL                     2
                            156 STORE_FAST               5 (start_idx)
                
-               275         158 LOAD_GLOBAL             11 (NULL + min)
+               274         158 LOAD_GLOBAL             11 (NULL + min)
                            170 LOAD_FAST                0 (self)
                            172 LOAD_ATTR                6 (sweep_count)
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR                7 (sweep_points)
                            194 BINARY_OP                5 (*)
                            198 LOAD_GLOBAL             17 (NULL + ceil)
                            210 LOAD_FAST                4 (xlim)
@@ -2307,15 +2299,15 @@
                            244 CALL                     1
                            254 LOAD_CONST               4 (1)
                            256 BINARY_OP                0 (+)
                            260 PRECALL                  2
                            264 CALL                     2
                            274 STORE_FAST               6 (end_idx)
                
-               276         276 LOAD_GLOBAL             19 (NULL + np)
+               275         276 LOAD_GLOBAL             19 (NULL + np)
                            288 LOAD_ATTR               10 (linspace)
                            298 LOAD_FAST                0 (self)
                            300 LOAD_ATTR                4 (x_interval)
                            310 LOAD_FAST                5 (start_idx)
                            312 BINARY_OP                5 (*)
                            316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                4 (x_interval)
@@ -2326,18 +2318,18 @@
                            338 BINARY_OP               10 (-)
                            342 LOAD_CONST               4 (1)
                            344 BINARY_OP                0 (+)
                            348 PRECALL                  3
                            352 CALL                     3
                            362 RETURN_VALUE
                
-               277     >>  364 LOAD_FAST                2 (sweeps)
+               276     >>  364 LOAD_FAST                2 (sweeps)
                            366 POP_JUMP_FORWARD_IF_NOT_NONE    59 (to 486)
                
-               278         368 LOAD_GLOBAL             19 (NULL + np)
+               277         368 LOAD_GLOBAL             19 (NULL + np)
                            380 LOAD_ATTR               10 (linspace)
                            390 LOAD_CONST               3 (0)
                            392 LOAD_FAST                0 (self)
                            394 LOAD_ATTR                6 (sweep_count)
                            404 LOAD_FAST                0 (self)
                            406 LOAD_ATTR                7 (sweep_points)
                            416 BINARY_OP                5 (*)
@@ -2351,38 +2343,38 @@
                            454 LOAD_FAST                0 (self)
                            456 LOAD_ATTR                7 (sweep_points)
                            466 BINARY_OP                5 (*)
                            470 PRECALL                  3
                            474 CALL                     3
                            484 RETURN_VALUE
                
-               280     >>  486 LOAD_GLOBAL             19 (NULL + np)
+               279     >>  486 LOAD_GLOBAL             19 (NULL + np)
                            498 LOAD_ATTR               11 (reshape)
                            508 LOAD_FAST                2 (sweeps)
                            510 LOAD_CONST               4 (1)
                            512 LOAD_GLOBAL             25 (NULL + len)
                            524 LOAD_FAST                2 (sweeps)
                            526 PRECALL                  1
                            530 CALL                     1
                            540 LOAD_CONST               4 (1)
                            542 BUILD_TUPLE              3
                            544 PRECALL                  2
                            548 CALL                     2
                            558 STORE_FAST               7 (mult)
                
-               281         560 LOAD_FAST                7 (mult)
+               280         560 LOAD_FAST                7 (mult)
                            562 LOAD_FAST                0 (self)
                            564 LOAD_ATTR                7 (sweep_points)
                            574 LOAD_FAST                0 (self)
                            576 LOAD_ATTR                4 (x_interval)
                            586 BINARY_OP                5 (*)
                            590 BINARY_OP                5 (*)
                            594 STORE_FAST               8 (offset)
                
-               282         596 LOAD_GLOBAL             19 (NULL + np)
+               281         596 LOAD_GLOBAL             19 (NULL + np)
                            608 LOAD_ATTR               10 (linspace)
                            618 LOAD_CONST               3 (0)
                            620 LOAD_FAST                0 (self)
                            622 LOAD_ATTR                7 (sweep_points)
                            632 LOAD_CONST               4 (1)
                            634 BINARY_OP               10 (-)
                            638 LOAD_FAST                0 (self)
@@ -2390,15 +2382,15 @@
                            650 BINARY_OP                5 (*)
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR                7 (sweep_points)
                            666 PRECALL                  3
                            670 CALL                     3
                            680 STORE_FAST               9 (one_row)
                
-               283         682 LOAD_GLOBAL             19 (NULL + np)
+               282         682 LOAD_GLOBAL             19 (NULL + np)
                            694 LOAD_ATTR               13 (repeat)
                            704 LOAD_FAST                9 (one_row)
                            706 LOAD_GLOBAL             25 (NULL + len)
                            718 LOAD_FAST                2 (sweeps)
                            720 PRECALL                  1
                            724 CALL                     1
                            734 LOAD_GLOBAL             25 (NULL + len)
@@ -2408,38 +2400,38 @@
                            762 BINARY_OP                5 (*)
                            766 PRECALL                  2
                            770 CALL                     2
                            780 LOAD_FAST                8 (offset)
                            782 BINARY_OP                0 (+)
                            786 RETURN_VALUE
                
-               284     >>  788 LOAD_FAST                1 (mode)
+               283     >>  788 LOAD_FAST                1 (mode)
                            790 LOAD_CONST               5 ('overlay')
                            792 COMPARE_OP               2 (==)
                            798 POP_JUMP_FORWARD_IF_FALSE   251 (to 1302)
                
-               285         800 LOAD_FAST                4 (xlim)
+               284         800 LOAD_FAST                4 (xlim)
                            802 POP_JUMP_FORWARD_IF_FALSE   147 (to 1098)
                
-               286         804 LOAD_GLOBAL              5 (NULL + max)
+               285         804 LOAD_GLOBAL              5 (NULL + max)
                            816 LOAD_CONST               3 (0)
                            818 LOAD_GLOBAL              7 (NULL + int)
                            830 LOAD_FAST                4 (xlim)
                            832 LOAD_CONST               3 (0)
                            834 BINARY_SUBSCR
                            844 LOAD_FAST                0 (self)
                            846 LOAD_ATTR                4 (x_interval)
                            856 BINARY_OP               11 (/)
                            860 PRECALL                  1
                            864 CALL                     1
                            874 PRECALL                  2
                            878 CALL                     2
                            888 STORE_FAST               5 (start_idx)
                
-               287         890 LOAD_GLOBAL             11 (NULL + min)
+               286         890 LOAD_GLOBAL             11 (NULL + min)
                            902 LOAD_FAST                0 (self)
                            904 LOAD_ATTR                6 (sweep_count)
                            914 LOAD_FAST                0 (self)
                            916 LOAD_ATTR                7 (sweep_points)
                            926 BINARY_OP                5 (*)
                            930 LOAD_GLOBAL             17 (NULL + ceil)
                            942 LOAD_FAST                4 (xlim)
@@ -2452,15 +2444,15 @@
                            976 CALL                     1
                            986 LOAD_CONST               4 (1)
                            988 BINARY_OP                0 (+)
                            992 PRECALL                  2
                            996 CALL                     2
                           1006 STORE_FAST               6 (end_idx)
                
-               288        1008 LOAD_GLOBAL             19 (NULL + np)
+               287        1008 LOAD_GLOBAL             19 (NULL + np)
                           1020 LOAD_ATTR               10 (linspace)
                           1030 LOAD_FAST                0 (self)
                           1032 LOAD_ATTR                4 (x_interval)
                           1042 LOAD_FAST                5 (start_idx)
                           1044 BINARY_OP                5 (*)
                           1048 LOAD_FAST                0 (self)
                           1050 LOAD_ATTR                4 (x_interval)
@@ -2472,15 +2464,15 @@
                           1074 LOAD_CONST               4 (1)
                           1076 BINARY_OP                0 (+)
                           1080 PRECALL                  3
                           1084 CALL                     3
                           1094 STORE_FAST               9 (one_row)
                           1096 JUMP_FORWARD            43 (to 1184)
                
-               290     >> 1098 LOAD_GLOBAL             19 (NULL + np)
+               289     >> 1098 LOAD_GLOBAL             19 (NULL + np)
                           1110 LOAD_ATTR               10 (linspace)
                           1120 LOAD_CONST               3 (0)
                           1122 LOAD_FAST                0 (self)
                           1124 LOAD_ATTR                7 (sweep_points)
                           1134 LOAD_CONST               4 (1)
                           1136 BINARY_OP               10 (-)
                           1140 LOAD_FAST                0 (self)
@@ -2488,15 +2480,15 @@
                           1152 BINARY_OP                5 (*)
                           1156 LOAD_FAST                0 (self)
                           1158 LOAD_ATTR                7 (sweep_points)
                           1168 PRECALL                  3
                           1172 CALL                     3
                           1182 STORE_FAST               9 (one_row)
                
-               291     >> 1184 LOAD_GLOBAL             19 (NULL + np)
+               290     >> 1184 LOAD_GLOBAL             19 (NULL + np)
                           1196 LOAD_ATTR               14 (broadcast_to)
                           1206 LOAD_FAST                9 (one_row)
                           1208 LOAD_GLOBAL             25 (NULL + len)
                           1220 LOAD_FAST                2 (sweeps)
                           1222 PRECALL                  1
                           1226 CALL                     1
                           1236 LOAD_GLOBAL             25 (NULL + len)
@@ -2508,30 +2500,30 @@
                           1270 LOAD_FAST                9 (one_row)
                           1272 LOAD_ATTR               15 (shape)
                           1282 BINARY_OP                0 (+)
                           1286 PRECALL                  2
                           1290 CALL                     2
                           1300 RETURN_VALUE
                
-               284     >> 1302 LOAD_CONST               1 (None)
+               283     >> 1302 LOAD_CONST               1 (None)
                           1304 RETURN_VALUE
                consts
                   "\n        returns a slice of the x_data\n        channels: list of int - if None, defaults to all channels\n        sweeps: list of int - only used for the 'overlay' plot_mode. If None, defaults to all sweeps\n        xlim: float tuple [left, right] - If None, defaults to all data points in each sweep\n        "
                   None
                   'continuous'
                   0
                   1
                   'overlay'
                names      ('range', 'channel_count', 'max', 'int', 'x_interval', 'min', 'sweep_count', 'sweep_points', 'ceil', 'np', 'linspace', 'reshape', 'len', 'repeat', 'broadcast_to', 'shape')
                varnames   ('self', 'mode', 'sweeps', 'channels', 'xlim', 'start_idx', 'end_idx', 'mult', 'offset', 'one_row')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'get_x_matrix'
-               firstlineno 261
+               firstlineno 260
                lnotab
                   0x02080c0128020e010401560176015801040176024a01240156016a010c
                   010401560176015a02560176f9
             code
                argcount  : 5
                nlocals   : 7
                stacksize : 7
@@ -2561,40 +2553,40 @@
                   007d06740f000000000000000000006a0800000000000000007c006a0200
                   000000000000007c057a0500007c006a0200000000000000007c067a0500
                   007c067c057a0a000064037a000000a6030000ab03000000000000000053
                   00740f000000000000000000006a08000000000000000064027c006a0500
                   0000000000000064037a0a00007c006a0200000000000000007a0500007c
                   006a050000000000000000a6030000ab0300000000000000005300640553
                   00
-               293           0 RESUME                   0
+               292           0 RESUME                   0
                
-               303           2 LOAD_FAST                1 (mode)
+               302           2 LOAD_FAST                1 (mode)
                              4 LOAD_CONST               1 ('continuous')
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE   207 (to 428)
                
-               304          14 LOAD_FAST                4 (xlim)
+               303          14 LOAD_FAST                4 (xlim)
                             16 POP_JUMP_FORWARD_IF_FALSE   146 (to 310)
                
-               305          18 LOAD_GLOBAL              1 (NULL + max)
+               304          18 LOAD_GLOBAL              1 (NULL + max)
                             30 LOAD_CONST               2 (0)
                             32 LOAD_GLOBAL              3 (NULL + int)
                             44 LOAD_FAST                4 (xlim)
                             46 LOAD_CONST               2 (0)
                             48 BINARY_SUBSCR
                             58 LOAD_FAST                0 (self)
                             60 LOAD_ATTR                2 (x_interval)
                             70 BINARY_OP               11 (/)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 PRECALL                  2
                             92 CALL                     2
                            102 STORE_FAST               5 (start_idx)
                
-               306         104 LOAD_GLOBAL              7 (NULL + min)
+               305         104 LOAD_GLOBAL              7 (NULL + min)
                            116 LOAD_FAST                0 (self)
                            118 LOAD_ATTR                4 (sweep_count)
                            128 LOAD_FAST                0 (self)
                            130 LOAD_ATTR                5 (sweep_points)
                            140 BINARY_OP                5 (*)
                            144 LOAD_CONST               3 (1)
                            146 BINARY_OP               10 (-)
@@ -2607,15 +2599,15 @@
                            188 BINARY_OP               11 (/)
                            192 PRECALL                  1
                            196 CALL                     1
                            206 PRECALL                  2
                            210 CALL                     2
                            220 STORE_FAST               6 (end_idx)
                
-               307         222 LOAD_GLOBAL             15 (NULL + np)
+               306         222 LOAD_GLOBAL             15 (NULL + np)
                            234 LOAD_ATTR                8 (linspace)
                            244 LOAD_FAST                0 (self)
                            246 LOAD_ATTR                2 (x_interval)
                            256 LOAD_FAST                5 (start_idx)
                            258 BINARY_OP                5 (*)
                            262 LOAD_FAST                0 (self)
                            264 LOAD_ATTR                2 (x_interval)
@@ -2626,15 +2618,15 @@
                            284 BINARY_OP               10 (-)
                            288 LOAD_CONST               3 (1)
                            290 BINARY_OP                0 (+)
                            294 PRECALL                  3
                            298 CALL                     3
                            308 RETURN_VALUE
                
-               308     >>  310 LOAD_GLOBAL             15 (NULL + np)
+               307     >>  310 LOAD_GLOBAL             15 (NULL + np)
                            322 LOAD_ATTR                8 (linspace)
                            332 LOAD_CONST               2 (0)
                            334 LOAD_FAST                0 (self)
                            336 LOAD_ATTR                4 (sweep_count)
                            346 LOAD_FAST                0 (self)
                            348 LOAD_ATTR                5 (sweep_points)
                            358 BINARY_OP                5 (*)
@@ -2648,38 +2640,38 @@
                            396 LOAD_FAST                0 (self)
                            398 LOAD_ATTR                5 (sweep_points)
                            408 BINARY_OP                5 (*)
                            412 PRECALL                  3
                            416 CALL                     3
                            426 RETURN_VALUE
                
-               309     >>  428 LOAD_FAST                1 (mode)
+               308     >>  428 LOAD_FAST                1 (mode)
                            430 LOAD_CONST               4 ('overlay')
                            432 COMPARE_OP               2 (==)
                            438 POP_JUMP_FORWARD_IF_FALSE   183 (to 806)
                
-               310         440 LOAD_FAST                4 (xlim)
+               309         440 LOAD_FAST                4 (xlim)
                            442 POP_JUMP_FORWARD_IF_FALSE   138 (to 720)
                
-               311         444 LOAD_GLOBAL              1 (NULL + max)
+               310         444 LOAD_GLOBAL              1 (NULL + max)
                            456 LOAD_CONST               2 (0)
                            458 LOAD_GLOBAL              3 (NULL + int)
                            470 LOAD_FAST                4 (xlim)
                            472 LOAD_CONST               2 (0)
                            474 BINARY_SUBSCR
                            484 LOAD_FAST                0 (self)
                            486 LOAD_ATTR                2 (x_interval)
                            496 BINARY_OP               11 (/)
                            500 PRECALL                  1
                            504 CALL                     1
                            514 PRECALL                  2
                            518 CALL                     2
                            528 STORE_FAST               5 (start_idx)
                
-               312         530 LOAD_GLOBAL              7 (NULL + min)
+               311         530 LOAD_GLOBAL              7 (NULL + min)
                            542 LOAD_FAST                0 (self)
                            544 LOAD_ATTR                5 (sweep_points)
                            554 LOAD_CONST               3 (1)
                            556 BINARY_OP               10 (-)
                            560 LOAD_GLOBAL             13 (NULL + ceil)
                            572 LOAD_FAST                4 (xlim)
                            574 LOAD_CONST               3 (1)
@@ -2689,15 +2681,15 @@
                            598 BINARY_OP               11 (/)
                            602 PRECALL                  1
                            606 CALL                     1
                            616 PRECALL                  2
                            620 CALL                     2
                            630 STORE_FAST               6 (end_idx)
                
-               313         632 LOAD_GLOBAL             15 (NULL + np)
+               312         632 LOAD_GLOBAL             15 (NULL + np)
                            644 LOAD_ATTR                8 (linspace)
                            654 LOAD_FAST                0 (self)
                            656 LOAD_ATTR                2 (x_interval)
                            666 LOAD_FAST                5 (start_idx)
                            668 BINARY_OP                5 (*)
                            672 LOAD_FAST                0 (self)
                            674 LOAD_ATTR                2 (x_interval)
@@ -2708,15 +2700,15 @@
                            694 BINARY_OP               10 (-)
                            698 LOAD_CONST               3 (1)
                            700 BINARY_OP                0 (+)
                            704 PRECALL                  3
                            708 CALL                     3
                            718 RETURN_VALUE
                
-               314     >>  720 LOAD_GLOBAL             15 (NULL + np)
+               313     >>  720 LOAD_GLOBAL             15 (NULL + np)
                            732 LOAD_ATTR                8 (linspace)
                            742 LOAD_CONST               2 (0)
                            744 LOAD_FAST                0 (self)
                            746 LOAD_ATTR                5 (sweep_points)
                            756 LOAD_CONST               3 (1)
                            758 BINARY_OP               10 (-)
                            762 LOAD_FAST                0 (self)
@@ -2724,30 +2716,30 @@
                            774 BINARY_OP                5 (*)
                            778 LOAD_FAST                0 (self)
                            780 LOAD_ATTR                5 (sweep_points)
                            790 PRECALL                  3
                            794 CALL                     3
                            804 RETURN_VALUE
                
-               309     >>  806 LOAD_CONST               5 (None)
+               308     >>  806 LOAD_CONST               5 (None)
                            808 RETURN_VALUE
                consts
                   '\n        returns a 1D numpy array representing the x-values in the recording.\n        Use this function to get x-values for plotting\n        mode: string\n            continuous, concatenate, or None\n        sweep: int\n        channel: int if None, defaults to current channel\n        xlim: float tuple - [left, right] If None, defaults to all x-values\n        '
                   'continuous'
                   0
                   1
                   'overlay'
                   None
                names      ('max', 'int', 'x_interval', 'min', 'sweep_count', 'sweep_points', 'ceil', 'np', 'linspace', 'return_val')
                varnames   ('self', 'mode', 'sweep', 'channel', 'xlim', 'start_idx', 'end_idx')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'get_xs'
-               firstlineno 293
+               firstlineno 292
                lnotab 0x020a0c01040156017601580176010c01040156016601580156fb
             code
                argcount  : 5
                nlocals   : 5
                stacksize : 11
                flags     : 3
                code
@@ -2770,49 +2762,49 @@
                   007c006a0500000000000000007a0b0000a6010000ab0100000000000000
                   00a6020000ab020000000000000000740d000000000000000000007c006a
                   0800000000000000007413000000000000000000007c0464041900000000
                   00000000007c006a0500000000000000007a0b0000a6010000ab01000000
                   000000000064047a000000a6020000ab0200000000000000008502660319
                   00000000000000000053007c006a0100000000000000007c037c02660219
                   000000000000000000530064015300
-               317           0 RESUME                   0
+               316           0 RESUME                   0
                
-               329           2 LOAD_FAST                3 (channel)
+               328           2 LOAD_FAST                3 (channel)
                              4 LOAD_CONST               1 (None)
                              6 COMPARE_OP               2 (==)
                             12 POP_JUMP_FORWARD_IF_FALSE     7 (to 28)
                
-               330          14 LOAD_FAST                0 (self)
+               329          14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                0 (channel)
                             26 STORE_FAST               3 (channel)
                
-               331     >>   28 LOAD_FAST                1 (mode)
+               330     >>   28 LOAD_FAST                1 (mode)
                             30 LOAD_CONST               2 ('continuous')
                             32 COMPARE_OP               2 (==)
                             38 POP_JUMP_FORWARD_IF_FALSE   184 (to 408)
                
-               332          40 LOAD_FAST                4 (xlim)
+               331          40 LOAD_FAST                4 (xlim)
                             42 POP_JUMP_FORWARD_IF_FALSE   144 (to 332)
                
-               334          44 LOAD_FAST                0 (self)
+               333          44 LOAD_FAST                0 (self)
                             46 LOAD_ATTR                1 (y_data)
                             56 LOAD_FAST                3 (channel)
                             58 LOAD_CONST               1 (None)
                             60 LOAD_CONST               1 (None)
                             62 BUILD_SLICE              2
                             64 LOAD_CONST               1 (None)
                             66 LOAD_CONST               1 (None)
                             68 BUILD_SLICE              2
                             70 BUILD_TUPLE              3
                             72 BINARY_SUBSCR
                             82 LOAD_METHOD              2 (ravel)
                            104 PRECALL                  0
                            108 CALL                     0
                
-               335         118 LOAD_GLOBAL              7 (NULL + max)
+               334         118 LOAD_GLOBAL              7 (NULL + max)
                            130 LOAD_CONST               3 (0)
                            132 LOAD_GLOBAL              9 (NULL + int)
                            144 LOAD_FAST                4 (xlim)
                            146 LOAD_CONST               3 (0)
                            148 BINARY_SUBSCR
                            158 LOAD_FAST                0 (self)
                            160 LOAD_ATTR                5 (x_interval)
@@ -2824,34 +2816,34 @@
                            202 LOAD_GLOBAL             13 (NULL + min)
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR                7 (sweep_count)
                            226 LOAD_FAST                0 (self)
                            228 LOAD_ATTR                8 (sweep_points)
                            238 BINARY_OP                5 (*)
                
-               336         242 LOAD_GLOBAL             19 (NULL + ceil)
+               335         242 LOAD_GLOBAL             19 (NULL + ceil)
                            254 LOAD_FAST                4 (xlim)
                            256 LOAD_CONST               4 (1)
                            258 BINARY_SUBSCR
                            268 LOAD_FAST                0 (self)
                            270 LOAD_ATTR                5 (x_interval)
                            280 BINARY_OP               11 (/)
                            284 PRECALL                  1
                            288 CALL                     1
                            298 LOAD_CONST               4 (1)
                            300 BINARY_OP                0 (+)
                
-               335         304 PRECALL                  2
+               334         304 PRECALL                  2
                            308 CALL                     2
                            318 BUILD_SLICE              2
                
-               334         320 BINARY_SUBSCR
+               333         320 BINARY_SUBSCR
                            330 RETURN_VALUE
                
-               339     >>  332 LOAD_FAST                0 (self)
+               338     >>  332 LOAD_FAST                0 (self)
                            334 LOAD_ATTR                1 (y_data)
                            344 LOAD_FAST                3 (channel)
                            346 LOAD_CONST               1 (None)
                            348 LOAD_CONST               1 (None)
                            350 BUILD_SLICE              2
                            352 LOAD_CONST               1 (None)
                            354 LOAD_CONST               1 (None)
@@ -2859,28 +2851,28 @@
                            358 BUILD_TUPLE              3
                            360 BINARY_SUBSCR
                            370 LOAD_METHOD              2 (ravel)
                            392 PRECALL                  0
                            396 CALL                     0
                            406 RETURN_VALUE
                
-               340     >>  408 LOAD_FAST                1 (mode)
+               339     >>  408 LOAD_FAST                1 (mode)
                            410 LOAD_CONST               5 ('overlay')
                            412 COMPARE_OP               2 (==)
                            418 POP_JUMP_FORWARD_IF_FALSE   125 (to 670)
                
-               341         420 LOAD_FAST                4 (xlim)
+               340         420 LOAD_FAST                4 (xlim)
                            422 POP_JUMP_FORWARD_IF_FALSE   108 (to 640)
                
-               343         424 LOAD_FAST                0 (self)
+               342         424 LOAD_FAST                0 (self)
                            426 LOAD_ATTR                1 (y_data)
                            436 LOAD_FAST                3 (channel)
                            438 LOAD_FAST                2 (sweep)
                
-               344         440 LOAD_GLOBAL              7 (NULL + max)
+               343         440 LOAD_GLOBAL              7 (NULL + max)
                            452 LOAD_CONST               3 (0)
                            454 LOAD_GLOBAL              9 (NULL + int)
                            466 LOAD_FAST                4 (xlim)
                            468 LOAD_CONST               3 (0)
                            470 BINARY_SUBSCR
                            480 LOAD_FAST                0 (self)
                            482 LOAD_ATTR                5 (x_interval)
@@ -2889,58 +2881,58 @@
                            500 CALL                     1
                            510 PRECALL                  2
                            514 CALL                     2
                            524 LOAD_GLOBAL             13 (NULL + min)
                            536 LOAD_FAST                0 (self)
                            538 LOAD_ATTR                8 (sweep_points)
                
-               345         548 LOAD_GLOBAL             19 (NULL + ceil)
+               344         548 LOAD_GLOBAL             19 (NULL + ceil)
                            560 LOAD_FAST                4 (xlim)
                            562 LOAD_CONST               4 (1)
                            564 BINARY_SUBSCR
                            574 LOAD_FAST                0 (self)
                            576 LOAD_ATTR                5 (x_interval)
                            586 BINARY_OP               11 (/)
                            590 PRECALL                  1
                            594 CALL                     1
                            604 LOAD_CONST               4 (1)
                            606 BINARY_OP                0 (+)
                
-               344         610 PRECALL                  2
+               343         610 PRECALL                  2
                            614 CALL                     2
                            624 BUILD_SLICE              2
                
-               343         626 BUILD_TUPLE              3
+               342         626 BUILD_TUPLE              3
                            628 BINARY_SUBSCR
                            638 RETURN_VALUE
                
-               347     >>  640 LOAD_FAST                0 (self)
+               346     >>  640 LOAD_FAST                0 (self)
                            642 LOAD_ATTR                1 (y_data)
                            652 LOAD_FAST                3 (channel)
                            654 LOAD_FAST                2 (sweep)
                            656 BUILD_TUPLE              2
                            658 BINARY_SUBSCR
                            668 RETURN_VALUE
                
-               340     >>  670 LOAD_CONST               1 (None)
+               339     >>  670 LOAD_CONST               1 (None)
                            672 RETURN_VALUE
                consts
                   "\n        returns a 1D numpy array representing the y-values of the recording.\n        Use this functions to get y-values for plotting\n        mode: string\n            'continuous', 'overlay', or None\n            if 'continuous', all sweeps are represented\n        sweep: int\n        channel: int\n            if empty, the current channel in the object is used\n        xlim: float tuple - [left, right] If None, defaults to all x-values\n        "
                   None
                   'continuous'
                   0
                   1
                   'overlay'
                names      ('channel', 'y_data', 'ravel', 'max', 'int', 'x_interval', 'min', 'sweep_count', 'sweep_points', 'ceil')
                varnames   ('self', 'mode', 'sweep', 'channel', 'xlim')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'get_ys'
-               firstlineno 317
+               firstlineno 316
                lnotab
                   0x020c0c010e010c0104024a017c013eff10ff0c054c010c01040210016c
                   013eff10ff0e041ef9
             code
                argcount  : 4
                nlocals   : 7
                stacksize : 10
@@ -2958,73 +2950,73 @@
                   090000000000000000000000000000000000000000640584007c006a0a00
                   000000000000007c05190000000000000000007c06190000000000000000
                   004400a6000000ab000000000000000000a6010000ab0100000000000000
                   00a6010000ab01000000000000000001007c04a008000000000000000000
                   00000000000000000000006406a6010000ab01000000000000000001008c
                   5b8c600900640764076407a6020000ab02000000000000000001006e0b23
                   00310073047702780359007701010059000100010064075300
-               349           0 RESUME                   0
+               348           0 RESUME                   0
                
-               357           2 LOAD_FAST                2 (channels)
+               356           2 LOAD_FAST                2 (channels)
                              4 POP_JUMP_FORWARD_IF_TRUE    20 (to 46)
                
-               358           6 LOAD_GLOBAL              1 (NULL + range)
+               357           6 LOAD_GLOBAL              1 (NULL + range)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (channel_count)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 STORE_FAST               2 (channels)
                
-               359     >>   46 LOAD_FAST                3 (sweeps)
+               358     >>   46 LOAD_FAST                3 (sweeps)
                             48 POP_JUMP_FORWARD_IF_TRUE    20 (to 90)
                
-               360          50 LOAD_GLOBAL              1 (NULL + range)
+               359          50 LOAD_GLOBAL              1 (NULL + range)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                2 (sweep_count)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 STORE_FAST               3 (sweeps)
                
-               361     >>   90 LOAD_GLOBAL              7 (NULL + os)
+               360     >>   90 LOAD_GLOBAL              7 (NULL + os)
                            102 LOAD_ATTR                4 (makedirs)
                            112 LOAD_GLOBAL              6 (os)
                            124 LOAD_ATTR                5 (path)
                            134 LOAD_METHOD              6 (dirname)
                            156 LOAD_FAST                1 (filename)
                            158 PRECALL                  1
                            162 CALL                     1
                            172 LOAD_CONST               1 (True)
                            174 KW_NAMES                 2
                            176 PRECALL                  2
                            180 CALL                     2
                            190 POP_TOP
                
-               362         192 LOAD_GLOBAL             15 (NULL + open)
+               361         192 LOAD_GLOBAL             15 (NULL + open)
                            204 LOAD_FAST                1 (filename)
                            206 LOAD_CONST               3 ('w')
                            208 PRECALL                  2
                            212 CALL                     2
                            222 BEFORE_WITH
                            224 STORE_FAST               4 (f)
                
-               363         226 LOAD_FAST                2 (channels)
+               362         226 LOAD_FAST                2 (channels)
                            228 GET_ITER
                        >>  230 FOR_ITER                95 (to 422)
                            232 STORE_FAST               5 (c)
                
-               364         234 LOAD_FAST                3 (sweeps)
+               363         234 LOAD_FAST                3 (sweeps)
                            236 GET_ITER
                        >>  238 FOR_ITER                90 (to 420)
                            240 STORE_FAST               6 (s)
                
-               365         242 LOAD_FAST                4 (f)
+               364         242 LOAD_FAST                4 (f)
                            244 LOAD_METHOD              8 (write)
                            266 LOAD_CONST               4 (',')
                            268 LOAD_METHOD              9 (join)
-                           290 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 365>)
+                           290 LOAD_CONST               5 (<code object <listcomp>, file "C:\Users\rosko\Documents\GitHub\SimplyFire\simplyfire\utils\recording.py", line 364>)
                            292 MAKE_FUNCTION            0
                            294 LOAD_FAST                0 (self)
                            296 LOAD_ATTR               10 (y_data)
                            306 LOAD_FAST                5 (c)
                            308 BINARY_SUBSCR
                            318 LOAD_FAST                6 (s)
                            320 BINARY_SUBSCR
@@ -3033,27 +3025,27 @@
                            336 CALL                     0
                            346 PRECALL                  1
                            350 CALL                     1
                            360 PRECALL                  1
                            364 CALL                     1
                            374 POP_TOP
                
-               366         376 LOAD_FAST                4 (f)
+               365         376 LOAD_FAST                4 (f)
                            378 LOAD_METHOD              8 (write)
                            400 LOAD_CONST               6 ('\n')
                            402 PRECALL                  1
                            406 CALL                     1
                            416 POP_TOP
                            418 JUMP_BACKWARD           91 (to 238)
                
-               364     >>  420 JUMP_BACKWARD           96 (to 230)
+               363     >>  420 JUMP_BACKWARD           96 (to 230)
                
-               363     >>  422 NOP
+               362     >>  422 NOP
                
-               362         424 LOAD_CONST               7 (None)
+               361         424 LOAD_CONST               7 (None)
                            426 LOAD_CONST               7 (None)
                            428 LOAD_CONST               7 (None)
                            430 PRECALL                  2
                            434 CALL                     2
                            444 POP_TOP
                            446 JUMP_FORWARD            11 (to 470)
                        >>  448 PUSH_EXC_INFO
@@ -3064,15 +3056,15 @@
                            458 POP_EXCEPT
                            460 RERAISE                  1
                        >>  462 POP_TOP
                            464 POP_EXCEPT
                            466 POP_TOP
                            468 POP_TOP
                
-               367     >>  470 LOAD_CONST               7 (None)
+               366     >>  470 LOAD_CONST               7 (None)
                            472 RETURN_VALUE
                ExceptionTable:
                  224 to 420 -> 448 [1] lasti
                  448 to 454 -> 456 [3] lasti
                  462 to 462 -> 456 [3] lasti
                consts
                   '\n        saves y_data of specified channels and sweeps in a temporary file\n\n        filename: str name of the file\n        channels: list of int, defaults to all channels if None\n        sweeps: list of int, defaults to all sweeps if None\n        '
@@ -3084,15 +3076,15 @@
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 5
                      flags     : 19
                      code
                         0x970067007c005d117d017401000000000000000000007c01a6010000ab
                         01000000000000000091028c125300
-                     365           0 RESUME                   0
+                     364           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                17 (to 42)
                                    8 STORE_FAST               1 (d)
                                   10 LOAD_GLOBAL              1 (NULL + str)
                                   22 LOAD_FAST                1 (d)
                                   24 PRECALL                  1
@@ -3103,25 +3095,25 @@
                      consts
                      names      ('str',)
                      varnames   ('.0', 'd')
                      freevars   ()
                      cellvars   ()
                      filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                      name       '<listcomp>'
-                     firstlineno 365
+                     firstlineno 364
                      lnotab 0x
                   '\n'
                   None
                names      ('range', 'channel_count', 'sweep_count', 'os', 'makedirs', 'path', 'dirname', 'open', 'write', 'join', 'y_data')
                varnames   ('self', 'filename', 'channels', 'sweeps', 'f', 'c', 's')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'save_y_data'
-               firstlineno 349
+               firstlineno 348
                lnotab 0x02080401280104012801660122010801080186012cfe02ff02ff2e05
             code
                argcount  : 4
                nlocals   : 7
                stacksize : 8
                flags     : 3
                code
@@ -3132,55 +3124,55 @@
                   0035007d047c0244005d3f7d057c0344005d3a7d06740900000000000000
                   0000006a0500000000000000007c04a00600000000000000000000000000
                   00000000000000a6000000ab000000000000000000740e00000000000000
                   0000006402ac03a6030000ab0300000000000000007c006a080000000000
                   0000007c057c0666023c0000008c3b8c400900640064006400a6020000ab
                   02000000000000000001006e0b2300310073047702780359007701010059
                   000100010064005300
-               369           0 RESUME                   0
+               368           0 RESUME                   0
                
-               370           2 LOAD_FAST                2 (channels)
+               369           2 LOAD_FAST                2 (channels)
                              4 POP_JUMP_FORWARD_IF_TRUE    20 (to 46)
                
-               371           6 LOAD_GLOBAL              1 (NULL + range)
+               370           6 LOAD_GLOBAL              1 (NULL + range)
                             18 LOAD_FAST                0 (self)
                             20 LOAD_ATTR                1 (channel_count)
                             30 PRECALL                  1
                             34 CALL                     1
                             44 STORE_FAST               2 (channels)
                
-               372     >>   46 LOAD_FAST                3 (sweeps)
+               371     >>   46 LOAD_FAST                3 (sweeps)
                             48 POP_JUMP_FORWARD_IF_TRUE    20 (to 90)
                
-               373          50 LOAD_GLOBAL              1 (NULL + range)
+               372          50 LOAD_GLOBAL              1 (NULL + range)
                             62 LOAD_FAST                0 (self)
                             64 LOAD_ATTR                2 (sweep_count)
                             74 PRECALL                  1
                             78 CALL                     1
                             88 STORE_FAST               3 (sweeps)
                
-               374     >>   90 LOAD_GLOBAL              7 (NULL + open)
+               373     >>   90 LOAD_GLOBAL              7 (NULL + open)
                            102 LOAD_FAST                1 (filename)
                            104 LOAD_CONST               1 ('r')
                            106 PRECALL                  2
                            110 CALL                     2
                            120 BEFORE_WITH
                            122 STORE_FAST               4 (f)
                
-               375         124 LOAD_FAST                2 (channels)
+               374         124 LOAD_FAST                2 (channels)
                            126 GET_ITER
                        >>  128 FOR_ITER                63 (to 256)
                            130 STORE_FAST               5 (c)
                
-               376         132 LOAD_FAST                3 (sweeps)
+               375         132 LOAD_FAST                3 (sweeps)
                            134 GET_ITER
                        >>  136 FOR_ITER                58 (to 254)
                            138 STORE_FAST               6 (i)
                
-               377         140 LOAD_GLOBAL              9 (NULL + np)
+               376         140 LOAD_GLOBAL              9 (NULL + np)
                            152 LOAD_ATTR                5 (fromstring)
                            162 LOAD_FAST                4 (f)
                            164 LOAD_METHOD              6 (readline)
                            186 PRECALL                  0
                            190 CALL                     0
                            200 LOAD_GLOBAL             14 (float)
                            212 LOAD_CONST               2 (',')
@@ -3191,19 +3183,19 @@
                            232 LOAD_ATTR                8 (y_data)
                            242 LOAD_FAST                5 (c)
                            244 LOAD_FAST                6 (i)
                            246 BUILD_TUPLE              2
                            248 STORE_SUBSCR
                            252 JUMP_BACKWARD           59 (to 136)
                
-               376     >>  254 JUMP_BACKWARD           64 (to 128)
+               375     >>  254 JUMP_BACKWARD           64 (to 128)
                
-               375     >>  256 NOP
+               374     >>  256 NOP
                
-               374         258 LOAD_CONST               0 (None)
+               373         258 LOAD_CONST               0 (None)
                            260 LOAD_CONST               0 (None)
                            262 LOAD_CONST               0 (None)
                            264 PRECALL                  2
                            268 CALL                     2
                            278 POP_TOP
                            280 JUMP_FORWARD            11 (to 304)
                        >>  282 PUSH_EXC_INFO
@@ -3214,15 +3206,15 @@
                            292 POP_EXCEPT
                            294 RERAISE                  1
                        >>  296 POP_TOP
                            298 POP_EXCEPT
                            300 POP_TOP
                            302 POP_TOP
                
-               378     >>  304 LOAD_CONST               0 (None)
+               377     >>  304 LOAD_CONST               0 (None)
                            306 RETURN_VALUE
                ExceptionTable:
                  122 to 254 -> 282 [1] lasti
                  282 to 288 -> 290 [3] lasti
                  296 to 296 -> 290 [3] lasti
                consts
                   None
@@ -3231,15 +3223,15 @@
                   ('dtype', 'sep')
                names      ('range', 'channel_count', 'sweep_count', 'open', 'np', 'fromstring', 'readline', 'float', 'y_data')
                varnames   ('self', 'filename', 'channels', 'sweeps', 'f', 'c', 'i')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'load_y_data'
-               firstlineno 369
+               firstlineno 368
                lnotab 0x0201040128010401280122010801080172ff02ff02ff2e04
             code
                argcount  : 4
                nlocals   : 6
                stacksize : 6
                flags     : 3
                code
@@ -3256,41 +3248,41 @@
                   13000000000000000000007c02a6010000ab01000000000000000064017c
                   006a0200000000000000006603a6020000ab0200000000000000007d057c
                   057c047c023c0000007407000000000000000000006a0400000000000000
                   007c006a0500000000000000007c046401ac02a6030000ab030000000000
                   0000007c005f0500000000000000007c0078016a0a000000000000000064
                   017a0d000063025f0a00000000000000007c0078016a0b00000000000000
                   0064017a0d000063025f0b000000000000000064065300
-               380           0 RESUME                   0
+               379           0 RESUME                   0
                
-               389           2 LOAD_FAST                1 (new_data)
+               388           2 LOAD_FAST                1 (new_data)
                              4 LOAD_ATTR                0 (shape)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (channel_count)
                             26 LOAD_CONST               1 (1)
                             28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                2 (sweep_points)
                             40 BUILD_TUPLE              3
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE    34 (to 118)
                
-               391          50 LOAD_GLOBAL              7 (NULL + np)
+               390          50 LOAD_GLOBAL              7 (NULL + np)
                             62 LOAD_ATTR                4 (append)
                             72 LOAD_FAST                0 (self)
                             74 LOAD_ATTR                5 (y_data)
                             84 LOAD_FAST                1 (new_data)
                             86 LOAD_CONST               1 (1)
                             88 KW_NAMES                 2
                             90 PRECALL                  3
                             94 CALL                     3
                            104 LOAD_FAST                0 (self)
                            106 STORE_ATTR               5 (y_data)
                            116 JUMP_FORWARD           158 (to 434)
                
-               394     >>  118 LOAD_GLOBAL              7 (NULL + np)
+               393     >>  118 LOAD_GLOBAL              7 (NULL + np)
                            130 LOAD_ATTR                6 (full)
                            140 LOAD_FAST                0 (self)
                            142 LOAD_ATTR                1 (channel_count)
                            152 LOAD_CONST               1 (1)
                            154 LOAD_FAST                0 (self)
                            156 LOAD_ATTR                2 (sweep_points)
                            166 BUILD_TUPLE              3
@@ -3298,75 +3290,75 @@
                            180 LOAD_ATTR                7 (float)
                            190 LOAD_FAST                3 (fill)
                            192 KW_NAMES                 3
                            194 PRECALL                  3
                            198 CALL                     3
                            208 STORE_FAST               4 (temp_data)
                
-               395         210 LOAD_FAST                1 (new_data)
+               394         210 LOAD_FAST                1 (new_data)
                            212 LOAD_ATTR                0 (shape)
                
-               396         222 LOAD_CONST               4 (-1)
+               395         222 LOAD_CONST               4 (-1)
                
-               395         224 BINARY_SUBSCR
+               394         224 BINARY_SUBSCR
                
-               396         234 LOAD_FAST                0 (self)
+               395         234 LOAD_FAST                0 (self)
                            236 LOAD_ATTR                2 (sweep_points)
                
-               395         246 COMPARE_OP               2 (==)
+               394         246 COMPARE_OP               2 (==)
                            252 POP_JUMP_FORWARD_IF_TRUE    10 (to 274)
                            254 LOAD_ASSERTION_ERROR
                
-               396         256 LOAD_CONST               5 ('dimension mismatch - the sweep length does not match the existing data')
+               395         256 LOAD_CONST               5 ('dimension mismatch - the sweep length does not match the existing data')
                
-               395         258 PRECALL                  0
+               394         258 PRECALL                  0
                            262 CALL                     0
                            272 RAISE_VARARGS            1
                
-               397     >>  274 LOAD_GLOBAL              7 (NULL + np)
+               396     >>  274 LOAD_GLOBAL              7 (NULL + np)
                            286 LOAD_ATTR                8 (reshape)
                            296 LOAD_FAST                1 (new_data)
                            298 LOAD_GLOBAL             19 (NULL + len)
                            310 LOAD_FAST                2 (channels)
                            312 PRECALL                  1
                            316 CALL                     1
                            326 LOAD_CONST               1 (1)
                            328 LOAD_FAST                0 (self)
                            330 LOAD_ATTR                2 (sweep_points)
                            340 BUILD_TUPLE              3
                            342 PRECALL                  2
                            346 CALL                     2
                            356 STORE_FAST               5 (new_data_reshape)
                
-               398         358 LOAD_FAST                5 (new_data_reshape)
+               397         358 LOAD_FAST                5 (new_data_reshape)
                            360 LOAD_FAST                4 (temp_data)
                            362 LOAD_FAST                2 (channels)
                            364 STORE_SUBSCR
                
-               399         368 LOAD_GLOBAL              7 (NULL + np)
+               398         368 LOAD_GLOBAL              7 (NULL + np)
                            380 LOAD_ATTR                4 (append)
                            390 LOAD_FAST                0 (self)
                            392 LOAD_ATTR                5 (y_data)
                            402 LOAD_FAST                4 (temp_data)
                            404 LOAD_CONST               1 (1)
                            406 KW_NAMES                 2
                            408 PRECALL                  3
                            412 CALL                     3
                            422 LOAD_FAST                0 (self)
                            424 STORE_ATTR               5 (y_data)
                
-               401     >>  434 LOAD_FAST                0 (self)
+               400     >>  434 LOAD_FAST                0 (self)
                            436 COPY                     1
                            438 LOAD_ATTR               10 (sweep_count)
                            448 LOAD_CONST               1 (1)
                            450 BINARY_OP               13 (+=)
                            454 SWAP                     2
                            456 STORE_ATTR              10 (sweep_count)
                
-               402         466 LOAD_FAST                0 (self)
+               401         466 LOAD_FAST                0 (self)
                            468 COPY                     1
                            470 LOAD_ATTR               11 (added_sweep_count)
                            480 LOAD_CONST               1 (1)
                            482 BINARY_OP               13 (+=)
                            486 SWAP                     2
                            488 STORE_ATTR              11 (added_sweep_count)
                            498 LOAD_CONST               6 (None)
@@ -3381,15 +3373,15 @@
                   None
                names      ('shape', 'channel_count', 'sweep_points', 'np', 'append', 'y_data', 'full', 'float', 'reshape', 'len', 'sweep_count', 'added_sweep_count')
                varnames   ('self', 'new_data', 'channels', 'fill', 'temp_data', 'new_data_reshape')
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'append_sweep'
-               firstlineno 380
+               firstlineno 379
                lnotab
                   0x0209300244035c010c0102ff0a010cff0a0102ff100254010a01420220
                   01
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 5
@@ -3397,27 +3389,27 @@
                code
                   0x97007c006a0000000000000000007c006a0100000000000000006b0200
                   0000007202640053007c006a020000000000000000640064008502640064
                   0185026400640085026603190000000000000000007c005f020000000000
                   0000007c0078016a00000000000000000064027a17000063025f00000000
                   00000000007c0078016a03000000000000000064027a17000063025f0300
                   0000000000000064005300
-               404           0 RESUME                   0
+               403           0 RESUME                   0
                
-               405           2 LOAD_FAST                0 (self)
+               404           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (sweep_count)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (original_sweep_count)
                             26 COMPARE_OP               2 (==)
                             32 POP_JUMP_FORWARD_IF_FALSE     2 (to 38)
                
-               406          34 LOAD_CONST               0 (None)
+               405          34 LOAD_CONST               0 (None)
                             36 RETURN_VALUE
                
-               407     >>   38 LOAD_FAST                0 (self)
+               406     >>   38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (y_data)
                             50 LOAD_CONST               0 (None)
                             52 LOAD_CONST               0 (None)
                             54 BUILD_SLICE              2
                             56 LOAD_CONST               0 (None)
                             58 LOAD_CONST               1 (-1)
                             60 BUILD_SLICE              2
@@ -3425,23 +3417,23 @@
                             64 LOAD_CONST               0 (None)
                             66 BUILD_SLICE              2
                             68 BUILD_TUPLE              3
                             70 BINARY_SUBSCR
                             80 LOAD_FAST                0 (self)
                             82 STORE_ATTR               2 (y_data)
                
-               408          92 LOAD_FAST                0 (self)
+               407          92 LOAD_FAST                0 (self)
                             94 COPY                     1
                             96 LOAD_ATTR                0 (sweep_count)
                            106 LOAD_CONST               2 (1)
                            108 BINARY_OP               23 (-=)
                            112 SWAP                     2
                            114 STORE_ATTR               0 (sweep_count)
                
-               409         124 LOAD_FAST                0 (self)
+               408         124 LOAD_FAST                0 (self)
                            126 COPY                     1
                            128 LOAD_ATTR                3 (added_sweep_count)
                            138 LOAD_CONST               2 (1)
                            140 BINARY_OP               23 (-=)
                            144 SWAP                     2
                            146 STORE_ATTR               3 (added_sweep_count)
                            156 LOAD_CONST               0 (None)
@@ -3452,34 +3444,34 @@
                   1
                names      ('sweep_count', 'original_sweep_count', 'y_data', 'added_sweep_count')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
                filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
                name       'delete_last_sweep'
-               firstlineno 404
+               firstlineno 403
                lnotab 0x02012001040136012001
             (None, 0, False)
             (None,)
             ('continuous', None, None, None, True)
             ('continuous', None, None, None)
             (None, None)
             (None, 0)
          names      ('__name__', '__module__', '__qualname__', '__init__', '_open_file', 'read_abf', 'read_csv', 'save', 'write_abf', 'write_csv', 'set_channel', 'replace_y_data', 'get_y_matrix', 'get_x_matrix', 'get_xs', 'get_ys', 'save_y_data', 'load_y_data', 'append_sweep', 'delete_last_sweep')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
          name       'Recording'
-         firstlineno 30
+         firstlineno 29
          lnotab
             0x0a010608060c061d063308120604081306090827082908200818082008
             14080b0818
       'Recording'
-   names      ('__doc__', 'numpy', 'np', 'os', 'pyabf', 'abf', 'simplyfire.utils', 'abfWriter', 'simplyfire.setting', 'config', 'math', 'ceil', 'psutil', 'Process', 'Recording')
+   names      ('__doc__', 'numpy', 'np', 'os', 'pyabf', 'abf', 'simplyfire.utils', 'abfWriter', 'simplyfire.setting', 'config', 'math', 'ceil', 'Recording')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   'C:\\Users\\rosko\\Documents\\GitHub\\SimplyFire\\simplyfire\\utils\\recording.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010415080108010c010c010c010c010c02
+   lnotab 0x00ff02010415080108010c010c010c010c02
```

### Comparing `simplyfire-0.5.3/simplyfire/utils/__pycache__/validation.cpython-311.pyc` & `simplyfire-0.5.4/simplyfire/utils/__pycache__/validation.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/abfWriter.py` & `simplyfire-0.5.4/simplyfire/utils/abfWriter.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/calculate.py` & `simplyfire-0.5.4/simplyfire/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/custom_widgets.py` & `simplyfire-0.5.4/simplyfire/utils/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/formatting.py` & `simplyfire-0.5.4/simplyfire/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/plugin_GUI.py` & `simplyfire-0.5.4/simplyfire/utils/plugin_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/plugin_controller.py` & `simplyfire-0.5.4/simplyfire/utils/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/plugin_form.py` & `simplyfire-0.5.4/simplyfire/utils/plugin_form.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/plugin_popup.py` & `simplyfire-0.5.4/simplyfire/utils/plugin_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/plugin_table.py` & `simplyfire-0.5.4/simplyfire/utils/plugin_table.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/recording.py` & `simplyfire-0.5.4/simplyfire/utils/recording.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/scrollable_option_frame.py` & `simplyfire-0.5.4/simplyfire/utils/scrollable_option_frame.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/threader.py` & `simplyfire-0.5.4/simplyfire/utils/threader.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire/utils/validation.py` & `simplyfire-0.5.4/simplyfire/utils/validation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.3/simplyfire.egg-info/PKG-INFO` & `simplyfire-0.5.4/simplyfire.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.5.3
+Version: 0.5.4
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
 Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simplyfire-0.5.3/simplyfire.egg-info/SOURCES.txt` & `simplyfire-0.5.4/simplyfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

