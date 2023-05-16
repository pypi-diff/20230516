# Comparing `tmp/ovos-PHAL-plugin-notification-widgets-1.0.1a1.tar.gz` & `tmp/ovos-PHAL-plugin-notification-widgets-1.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-notification-widgets-1.0.1a1.tar", last modified: Thu Jan 12 22:47:52 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-notification-widgets-1.0.1a2.tar", last modified: Tue Apr  4 22:32:20 2023, max compression
```

## Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1.tar` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 22:47:52.209423 ovos-PHAL-plugin-notification-widgets-1.0.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-12 22:47:41.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-01-12 22:47:52.209423 ovos-PHAL-plugin-notification-widgets-1.0.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-01-12 22:47:41.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 22:47:52.209423 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-01-12 22:47:41.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-01-12 22:47:44.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 22:47:52.209423 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-01-12 22:47:51.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-01-12 22:47:52.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 22:47:51.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-01-12 22:47:51.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-12 22:47:51.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 22:47:51.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 22:47:41.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 22:47:52.209423 ovos-PHAL-plugin-notification-widgets-1.0.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-01-12 22:47:41.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.158981 ovos-PHAL-plugin-notification-widgets-1.0.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 22:32:07.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-04 22:32:20.158981 ovos-PHAL-plugin-notification-widgets-1.0.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-04 22:32:07.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.158981 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     9534 2023-04-04 22:32:07.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 22:32:14.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.158981 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:19.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:32:20.158981 ovos-PHAL-plugin-notification-widgets-1.0.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3039 2023-04-04 22:32:07.000000 ovos-PHAL-plugin-notification-widgets-1.0.1a2/setup.py
```

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/LICENSE` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/PKG-INFO` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-notification-widgets
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-notification-widgets
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/README.md` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets/__init__.py` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/PKG-INFO` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-notification-widgets
-Version: 1.0.1a1
+Version: 1.0.1a2
 Summary: Notifications and Widgets plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-notification-widgets
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/ovos_PHAL_plugin_notification_widgets.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/ovos_PHAL_plugin_notification_widgets.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-notification-widgets-1.0.1a1/setup.py` & `ovos-PHAL-plugin-notification-widgets-1.0.1a2/setup.py`

 * *Files identical despite different names*

