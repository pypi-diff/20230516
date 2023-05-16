# Comparing `tmp/ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2.tar.gz` & `tmp/ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2.tar", last modified: Tue Apr  4 23:10:22 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3.tar", last modified: Tue May 16 16:59:29 2023, max compression
```

## Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2.tar` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:10:22.877892 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 23:10:15.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 23:10:22.877892 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-04 23:10:15.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:10:22.877892 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi/
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-04-04 23:10:15.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 23:10:17.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 23:10:22.877892 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 23:10:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 23:10:22.877892 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-04 23:10:15.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:59:29.641620 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 16:59:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-16 16:59:29.641620 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-05-16 16:59:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:59:29.637621 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi/
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-05-16 16:59:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 16:59:25.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 16:59:29.641620 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 16:59:29.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 16:59:29.641620 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-05-16 16:59:22.000000 ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/setup.py
```

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/LICENSE` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/PKG-INFO` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-brightness-control-rpi
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-brightness-control
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/README.md` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,13 @@
-# OVOS PHAL BRIGHTNESS CONTROL PLUGIN FOR RPI
+# DEPRECATED - OVOS PHAL BRIGHTNESS CONTROL PLUGIN FOR RPI
 
+
+This repository is no longer maintained by OpenVoiceOS, use https://github.com/OpenVoiceOS/ovos-gui-plugin-shell-companion instead
+
+___________________________
 This plugin provides a brightness control interface for the Raspberry PI, it supports DSI and **HDMI screens
 
 ** HDMI Screens: Screens supported and detected by DDCUTILS only
 
 # Requirements
 - Requires ddcutils for HDMI: https://github.com/rockowitz/ddcutil (install location: "/usr/bin/ddcutil")
 - Requires vcgencmd for DSI: https://github.com/raspberrypi/userland (install location: "/opt/vc/bin/vcgencmd")
```

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi/__init__.py` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/PKG-INFO` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-brightness-control-rpi
-Version: 1.0.1a2
+Version: 1.0.1a3
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-brightness-control
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/ovos_PHAL_plugin_brightness_control_rpi.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/ovos_PHAL_plugin_brightness_control_rpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a2/setup.py` & `ovos-PHAL-plugin-brightness-control-rpi-1.0.1a3/setup.py`

 * *Files identical despite different names*

