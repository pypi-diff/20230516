# Comparing `tmp/simplyfire-0.5.1.tar.gz` & `tmp/simplyfire-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplyfire-0.5.1.tar", last modified: Mon May  1 23:29:11 2023, max compression
+gzip compressed data, was "simplyfire-0.5.2.tar", last modified: Tue May 16 01:29:21 2023, max compression
```

## Comparing `simplyfire-0.5.1.tar` & `simplyfire-0.5.2.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.767148 simplyfire-0.5.1/
--rw-rw-rw-   0        0        0    33092 2023-05-01 23:06:43.000000 simplyfire-0.5.1/LICENSE
--rw-rw-rw-   0        0        0       66 2023-05-01 23:06:43.000000 simplyfire-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1947 2023-05-01 23:29:11.767148 simplyfire-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1286 2023-05-01 23:06:43.000000 simplyfire-0.5.1/README.md
--rw-rw-rw-   0        0        0      108 2023-05-01 23:06:43.000000 simplyfire-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0      170 2023-05-01 23:29:11.768199 simplyfire-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2564 2023-05-01 23:27:17.000000 simplyfire-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.558971 simplyfire-0.5.1/simplyfire/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/__init__.py
--rw-rw-rw-   0        0        0     2236 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/__main__.py
--rw-rw-rw-   0        0        0    15816 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/app.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.582279 simplyfire-0.5.1/simplyfire/backend/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/__init__.py
--rw-rw-rw-   0        0        0    16487 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/interface.py
--rw-rw-rw-   0        0        0    22220 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/interpreter.py
--rw-rw-rw-   0        0        0     4163 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/backend/plugin_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.597229 simplyfire-0.5.1/simplyfire/img/
--rw-rw-rw-   0        0        0      239 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/arrow.png
--rw-rw-rw-   0        0        0   123774 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/loading.gif
--rw-rw-rw-   0        0        0   108307 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/logo.ico
--rw-rw-rw-   0        0        0   106769 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/logo_bw.ico
--rw-rw-rw-   0        0        0      255 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/pan_up.png
--rw-rw-rw-   0        0        0      553 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/x_zoom_in.png
--rw-rw-rw-   0        0        0      482 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/x_zoom_out.png
--rw-rw-rw-   0        0        0      528 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/y_zoom_in.png
--rw-rw-rw-   0        0        0      506 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/y_zoom_out.png
--rw-rw-rw-   0        0        0      597 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/img/zoom_in_y.png
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.630742 simplyfire-0.5.1/simplyfire/layout/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/__init__.py
--rw-rw-rw-   0        0        0    28853 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/batch_popup.py
--rw-rw-rw-   0        0        0    12580 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/graph_panel.py
--rw-rw-rw-   0        0        0     4461 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/log_display.py
--rw-rw-rw-   0        0        0     8569 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/menubar.py
--rw-rw-rw-   0        0        0     5979 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/plugin_tab.py
--rw-rw-rw-   0        0        0     2635 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/results_display.py
--rw-rw-rw-   0        0        0    12488 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/setting_tab.py
--rw-rw-rw-   0        0        0    16937 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/layout/trace_display.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.537614 simplyfire-0.5.1/simplyfire/plugins/
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.640733 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/
--rw-rw-rw-   0        0        0    15742 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/comparison_GUI.py
--rw-rw-rw-   0        0        0      200 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/comparison_plot/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.649784 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/
--rw-rw-rw-   0        0        0    15452 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_GUI.py
--rw-rw-rw-   0        0        0     2721 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_analysis.py
--rw-rw-rw-   0        0        0      232 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/evoked_basic/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.660456 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/
--rw-rw-rw-   0        0        0    89249 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_GUI.py
--rw-rw-rw-   0        0        0    61353 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_analysis.py
--rw-rw-rw-   0        0        0      236 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/mini_analysis/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.666001 simplyfire-0.5.1/simplyfire/plugins/navigation/
--rw-rw-rw-   0        0        0     8946 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/navigation/navigation.py
--rw-rw-rw-   0        0        0      172 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/navigation/plugin.yaml
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.673936 simplyfire-0.5.1/simplyfire/plugins/process_recording/
--rw-rw-rw-   0        0        0      254 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/plugin.yaml
--rw-rw-rw-   0        0        0    20784 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/process_GUI.py
--rw-rw-rw-   0        0        0     5259 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/process_recording/process_recording.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.679919 simplyfire-0.5.1/simplyfire/plugins/style/
--rw-rw-rw-   0        0        0      199 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/style/plugin.yaml
--rw-rw-rw-   0        0        0     5451 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/style/style_tab.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.685856 simplyfire-0.5.1/simplyfire/plugins/sweeps/
--rw-rw-rw-   0        0        0      201 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/sweeps/plugin.yaml
--rw-rw-rw-   0        0        0    14881 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/plugins/sweeps/sweeps_GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.700600 simplyfire-0.5.1/simplyfire/setting/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/__init__.py
--rw-rw-rw-   0        0        0     6453 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/config.py
--rw-rw-rw-   0        0        0     3517 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/setting/default_config.yaml
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.702678 simplyfire-0.5.1/simplyfire/temp/
--rw-rw-rw-   0        0        0      218 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/temp/README.md
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/temp/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.763200 simplyfire-0.5.1/simplyfire/utils/
--rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/__init__.py
--rw-rw-rw-   0        0        0     6411 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/abfWriter.py
--rw-rw-rw-   0        0        0     6620 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/calculate.py
--rw-rw-rw-   0        0        0    23659 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/custom_widgets.py
--rw-rw-rw-   0        0        0     3311 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/formatting.py
--rw-rw-rw-   0        0        0     2932 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_GUI.py
--rw-rw-rw-   0        0        0     8664 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_controller.py
--rw-rw-rw-   0        0        0     7778 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_form.py
--rw-rw-rw-   0        0        0     1900 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_popup.py
--rw-rw-rw-   0        0        0     8023 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/plugin_table.py
--rw-rw-rw-   0        0        0    19411 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/recording.py
--rw-rw-rw-   0        0        0    11690 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/scrollable_option_frame.py
--rw-rw-rw-   0        0        0     2651 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/threader.py
--rw-rw-rw-   0        0        0     3932 2023-05-01 23:06:43.000000 simplyfire-0.5.1/simplyfire/utils/validation.py
-drwxrwxrwx   0        0        0        0 2023-05-01 23:29:11.568961 simplyfire-0.5.1/simplyfire.egg-info/
--rw-rw-rw-   0        0        0     1947 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2459 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-01 23:21:50.000000 simplyfire-0.5.1/simplyfire.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       94 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 23:29:11.000000 simplyfire-0.5.1/simplyfire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.594778 simplyfire-0.5.2/
+-rw-rw-rw-   0        0        0    33092 2023-05-01 23:06:43.000000 simplyfire-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0       66 2023-05-01 23:06:43.000000 simplyfire-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1947 2023-05-16 01:29:21.594778 simplyfire-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1286 2023-05-01 23:06:43.000000 simplyfire-0.5.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-01 23:06:43.000000 simplyfire-0.5.2/pyproject.toml
+-rw-rw-rw-   0        0        0      170 2023-05-16 01:29:21.598774 simplyfire-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     2564 2023-05-16 01:28:56.000000 simplyfire-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.478905 simplyfire-0.5.2/simplyfire/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/__init__.py
+-rw-rw-rw-   0        0        0     2236 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/__main__.py
+-rw-rw-rw-   0        0        0    15816 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/app.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.522781 simplyfire-0.5.2/simplyfire/backend/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/backend/__init__.py
+-rw-rw-rw-   0        0        0    16487 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/backend/interface.py
+-rw-rw-rw-   0        0        0    22220 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/backend/interpreter.py
+-rw-rw-rw-   0        0        0     4163 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/backend/plugin_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.538778 simplyfire-0.5.2/simplyfire/img/
+-rw-rw-rw-   0        0        0      239 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/arrow.png
+-rw-rw-rw-   0        0        0   123774 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/loading.gif
+-rw-rw-rw-   0        0        0   108307 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/logo.ico
+-rw-rw-rw-   0        0        0   106769 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/logo_bw.ico
+-rw-rw-rw-   0        0        0      255 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/pan_up.png
+-rw-rw-rw-   0        0        0      553 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/x_zoom_in.png
+-rw-rw-rw-   0        0        0      482 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/x_zoom_out.png
+-rw-rw-rw-   0        0        0      528 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/y_zoom_in.png
+-rw-rw-rw-   0        0        0      506 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/y_zoom_out.png
+-rw-rw-rw-   0        0        0      597 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/img/zoom_in_y.png
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.554892 simplyfire-0.5.2/simplyfire/layout/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/__init__.py
+-rw-rw-rw-   0        0        0    28853 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/batch_popup.py
+-rw-rw-rw-   0        0        0    12580 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/graph_panel.py
+-rw-rw-rw-   0        0        0     4461 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/log_display.py
+-rw-rw-rw-   0        0        0     8569 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/menubar.py
+-rw-rw-rw-   0        0        0     5979 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/plugin_tab.py
+-rw-rw-rw-   0        0        0     2635 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/results_display.py
+-rw-rw-rw-   0        0        0    12488 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/setting_tab.py
+-rw-rw-rw-   0        0        0    16937 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/layout/trace_display.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.466763 simplyfire-0.5.2/simplyfire/plugins/
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.558776 simplyfire-0.5.2/simplyfire/plugins/comparison_plot/
+-rw-rw-rw-   0        0        0    15742 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/comparison_plot/comparison_GUI.py
+-rw-rw-rw-   0        0        0      200 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/comparison_plot/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.562784 simplyfire-0.5.2/simplyfire/plugins/evoked_basic/
+-rw-rw-rw-   0        0        0    15452 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/evoked_basic/evoked_GUI.py
+-rw-rw-rw-   0        0        0     2721 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/evoked_basic/evoked_analysis.py
+-rw-rw-rw-   0        0        0      232 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/evoked_basic/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.566774 simplyfire-0.5.2/simplyfire/plugins/mini_analysis/
+-rw-rw-rw-   0        0        0    89249 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/mini_analysis/mini_GUI.py
+-rw-rw-rw-   0        0        0    61353 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/mini_analysis/mini_analysis.py
+-rw-rw-rw-   0        0        0      236 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/mini_analysis/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.566774 simplyfire-0.5.2/simplyfire/plugins/navigation/
+-rw-rw-rw-   0        0        0     8946 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/navigation/navigation.py
+-rw-rw-rw-   0        0        0      172 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/navigation/plugin.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.570886 simplyfire-0.5.2/simplyfire/plugins/process_recording/
+-rw-rw-rw-   0        0        0      254 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/process_recording/plugin.yaml
+-rw-rw-rw-   0        0        0    20784 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/process_recording/process_GUI.py
+-rw-rw-rw-   0        0        0     5259 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/process_recording/process_recording.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.574842 simplyfire-0.5.2/simplyfire/plugins/style/
+-rw-rw-rw-   0        0        0      199 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/style/plugin.yaml
+-rw-rw-rw-   0        0        0     5451 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/style/style_tab.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.574842 simplyfire-0.5.2/simplyfire/plugins/sweeps/
+-rw-rw-rw-   0        0        0      201 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/sweeps/plugin.yaml
+-rw-rw-rw-   0        0        0    14881 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/plugins/sweeps/sweeps_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.578873 simplyfire-0.5.2/simplyfire/setting/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/setting/__init__.py
+-rw-rw-rw-   0        0        0     6453 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/setting/config.py
+-rw-rw-rw-   0        0        0     3517 2023-05-16 01:25:36.000000 simplyfire-0.5.2/simplyfire/setting/default_config.yaml
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.582882 simplyfire-0.5.2/simplyfire/temp/
+-rw-rw-rw-   0        0        0      218 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/temp/README.md
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/temp/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.594778 simplyfire-0.5.2/simplyfire/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/__init__.py
+-rw-rw-rw-   0        0        0     6411 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/abfWriter.py
+-rw-rw-rw-   0        0        0     6620 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/calculate.py
+-rw-rw-rw-   0        0        0    23659 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/custom_widgets.py
+-rw-rw-rw-   0        0        0     3311 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/formatting.py
+-rw-rw-rw-   0        0        0     2932 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/plugin_GUI.py
+-rw-rw-rw-   0        0        0     8664 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/plugin_controller.py
+-rw-rw-rw-   0        0        0     7778 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/plugin_form.py
+-rw-rw-rw-   0        0        0     1900 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/plugin_popup.py
+-rw-rw-rw-   0        0        0     8023 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/plugin_table.py
+-rw-rw-rw-   0        0        0    19411 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/recording.py
+-rw-rw-rw-   0        0        0    11690 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/scrollable_option_frame.py
+-rw-rw-rw-   0        0        0     2651 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/threader.py
+-rw-rw-rw-   0        0        0     3932 2023-05-01 23:06:43.000000 simplyfire-0.5.2/simplyfire/utils/validation.py
+drwxrwxrwx   0        0        0        0 2023-05-16 01:29:21.514889 simplyfire-0.5.2/simplyfire.egg-info/
+-rw-rw-rw-   0        0        0     1947 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2459 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-01 23:21:50.000000 simplyfire-0.5.2/simplyfire.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       94 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 01:29:21.000000 simplyfire-0.5.2/simplyfire.egg-info/top_level.txt
```

### Comparing `simplyfire-0.5.1/LICENSE` & `simplyfire-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/PKG-INFO` & `simplyfire-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.5.1
+Version: 0.5.2
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
 Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simplyfire-0.5.1/README.md` & `simplyfire-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/setup.py` & `simplyfire-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 """
 from setuptools import setup, find_packages
 with open('README.md') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='simplyfire',
-    version='0.5.1',
+    version='0.5.2',
     author='Megumi Mori, Andrew Rosko',
     description='Customizable electrophysiology analysis software',
     long_description=readme,
     long_description_content_type='text/markdown',
     url="https://simplyfire.readthedocs.io/",
     pakage_dir={'simplyfire':'simplyfire'},
     packages = find_packages(),
```

### Comparing `simplyfire-0.5.1/simplyfire/__main__.py` & `simplyfire-0.5.2/simplyfire/__main__.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/app.py` & `simplyfire-0.5.2/simplyfire/app.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/backend/interface.py` & `simplyfire-0.5.2/simplyfire/backend/interface.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/backend/interpreter.py` & `simplyfire-0.5.2/simplyfire/backend/interpreter.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/backend/plugin_manager.py` & `simplyfire-0.5.2/simplyfire/backend/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/loading.gif` & `simplyfire-0.5.2/simplyfire/img/loading.gif`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/logo.ico` & `simplyfire-0.5.2/simplyfire/img/logo.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/logo_bw.ico` & `simplyfire-0.5.2/simplyfire/img/logo_bw.ico`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/x_zoom_in.png` & `simplyfire-0.5.2/simplyfire/img/x_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/y_zoom_in.png` & `simplyfire-0.5.2/simplyfire/img/y_zoom_in.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/img/zoom_in_y.png` & `simplyfire-0.5.2/simplyfire/img/zoom_in_y.png`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/batch_popup.py` & `simplyfire-0.5.2/simplyfire/layout/batch_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/graph_panel.py` & `simplyfire-0.5.2/simplyfire/layout/graph_panel.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/log_display.py` & `simplyfire-0.5.2/simplyfire/layout/log_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/menubar.py` & `simplyfire-0.5.2/simplyfire/layout/menubar.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/plugin_tab.py` & `simplyfire-0.5.2/simplyfire/layout/plugin_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/results_display.py` & `simplyfire-0.5.2/simplyfire/layout/results_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/setting_tab.py` & `simplyfire-0.5.2/simplyfire/layout/setting_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/layout/trace_display.py` & `simplyfire-0.5.2/simplyfire/layout/trace_display.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/comparison_plot/comparison_GUI.py` & `simplyfire-0.5.2/simplyfire/plugins/comparison_plot/comparison_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_GUI.py` & `simplyfire-0.5.2/simplyfire/plugins/evoked_basic/evoked_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/evoked_basic/evoked_analysis.py` & `simplyfire-0.5.2/simplyfire/plugins/evoked_basic/evoked_analysis.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_GUI.py` & `simplyfire-0.5.2/simplyfire/plugins/mini_analysis/mini_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/mini_analysis/mini_analysis.py` & `simplyfire-0.5.2/simplyfire/plugins/mini_analysis/mini_analysis.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/navigation/navigation.py` & `simplyfire-0.5.2/simplyfire/plugins/navigation/navigation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/process_recording/process_GUI.py` & `simplyfire-0.5.2/simplyfire/plugins/process_recording/process_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/process_recording/process_recording.py` & `simplyfire-0.5.2/simplyfire/plugins/process_recording/process_recording.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/style/style_tab.py` & `simplyfire-0.5.2/simplyfire/plugins/style/style_tab.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/plugins/sweeps/sweeps_GUI.py` & `simplyfire-0.5.2/simplyfire/plugins/sweeps/sweeps_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/setting/config.py` & `simplyfire-0.5.2/simplyfire/setting/config.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/setting/default_config.yaml` & `simplyfire-0.5.2/simplyfire/setting/default_config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # The key_map dict is used to map most of the core key-bindings.
 # Key names follow the tkinter convention.
 # Until a key-mapper feature is added (planned for future releases),
 # the keys can be edited here.
 #################################################################
 
 # version
-version : '0.4.2'
+version : '0.5.2'
 
 #aesthetics
 geometry : '900x600'
 zoomed : 0
 
 relative_cp_width : 0.25
 cp_width : 270
```

### Comparing `simplyfire-0.5.1/simplyfire/utils/abfWriter.py` & `simplyfire-0.5.2/simplyfire/utils/abfWriter.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/calculate.py` & `simplyfire-0.5.2/simplyfire/utils/calculate.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/custom_widgets.py` & `simplyfire-0.5.2/simplyfire/utils/custom_widgets.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/formatting.py` & `simplyfire-0.5.2/simplyfire/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/plugin_GUI.py` & `simplyfire-0.5.2/simplyfire/utils/plugin_GUI.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/plugin_controller.py` & `simplyfire-0.5.2/simplyfire/utils/plugin_controller.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/plugin_form.py` & `simplyfire-0.5.2/simplyfire/utils/plugin_form.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/plugin_popup.py` & `simplyfire-0.5.2/simplyfire/utils/plugin_popup.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/plugin_table.py` & `simplyfire-0.5.2/simplyfire/utils/plugin_table.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/recording.py` & `simplyfire-0.5.2/simplyfire/utils/recording.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/scrollable_option_frame.py` & `simplyfire-0.5.2/simplyfire/utils/scrollable_option_frame.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/threader.py` & `simplyfire-0.5.2/simplyfire/utils/threader.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire/utils/validation.py` & `simplyfire-0.5.2/simplyfire/utils/validation.py`

 * *Files identical despite different names*

### Comparing `simplyfire-0.5.1/simplyfire.egg-info/PKG-INFO` & `simplyfire-0.5.2/simplyfire.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplyfire
-Version: 0.5.1
+Version: 0.5.2
 Summary: Customizable electrophysiology analysis software
 Home-page: https://simplyfire.readthedocs.io/
 Author: Megumi Mori, Andrew Rosko
 License: GNU General Public License v3
 Keywords: neuroscience,analysis,electrophysiology,gui-application
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `simplyfire-0.5.1/simplyfire.egg-info/SOURCES.txt` & `simplyfire-0.5.2/simplyfire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

