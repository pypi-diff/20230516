# Comparing `tmp/ovos-PHAL-plugin-color-scheme-manager-1.0.0a5.tar.gz` & `tmp/ovos-PHAL-plugin-color-scheme-manager-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-color-scheme-manager-1.0.0a5.tar", last modified: Thu Nov 10 00:11:05 2022, max compression
+gzip compressed data, was "ovos-PHAL-plugin-color-scheme-manager-1.0.1a1.tar", last modified: Tue Apr  4 22:32:16 2023, max compression
```

## Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5.tar` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 00:11:05.434986 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-10 00:10:56.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-10 00:11:05.434986 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-11-10 00:10:56.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 00:11:05.434986 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager/
--rw-r--r--   0 runner    (1001) docker     (121)     3237 2022-11-10 00:10:56.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-11-10 00:10:59.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 00:11:05.434986 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      115 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       64 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 00:11:05.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-10 00:11:05.434986 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     3023 2022-11-10 00:10:56.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:16.242550 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 22:32:08.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-04 22:32:16.238550 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-04 22:32:08.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:16.238550 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-04 22:32:08.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 22:32:11.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:16.238550 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:16.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:32:16.242550 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-04-04 22:32:08.000000 ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/setup.py
```

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/LICENSE` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/PKG-INFO` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-color-scheme-manager
-Version: 1.0.0a5
+Version: 1.0.1a1
 Summary: Color scheme manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-color-scheme-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/README.md` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager/__init__.py` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-color-scheme-manager
-Version: 1.0.0a5
+Version: 1.0.1a1
 Summary: Color scheme manager plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-color-scheme-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/ovos_PHAL_plugin_color_scheme_manager.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/ovos_PHAL_plugin_color_scheme_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-color-scheme-manager-1.0.0a5/setup.py` & `ovos-PHAL-plugin-color-scheme-manager-1.0.1a1/setup.py`

 * *Files identical despite different names*

