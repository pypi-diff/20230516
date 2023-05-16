# Comparing `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.0a2.tar.gz` & `tmp/ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.0a2.tar", last modified: Thu Feb 23 22:49:31 2023, max compression
+gzip compressed data, was "ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar", last modified: Tue May 16 20:15:12 2023, max compression
```

## Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2.tar` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:49:31.801286 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-23 22:49:24.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-23 22:49:31.801286 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11013 2023-02-23 22:49:24.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:49:31.801286 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/
--rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-02-23 22:49:24.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-23 22:49:24.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-02-23 22:49:26.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:49:31.801286 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:49:31.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 22:49:31.801286 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-02-23 22:49:24.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11092 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.203867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)    18286 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 20:15:07.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:15:12.203867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-16 20:15:12.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-16 20:15:11.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 20:15:12.207867 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2992 2023-05-16 20:15:03.000000 ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.py
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/LICENSE` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.0a2
+Version: 0.0.1a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/README.md` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # OVOS PHAL PLUGIN WALLPAPER MANAGER
 This PHAL plugin provides a central wallpaper management interface for homescreens and other desktops
 
+Platform support provided by https://github.com/OpenVoiceOS/wallpaper_changer
+
 ### What is the Wallpaper Management Interface ?
 The wallpaper management interface provides functionality for providing a central interface for homescreen and desktop wallpaper management, this interface is responsible for providing a list of available wallpapers and also provides functionality for setting a wallpaper from the list of available wallpapers. This interface supports different types of wallpaper providers, this can be a local provider that provides wallpapers from the local filesystem or a remote provider that provides wallpapers from a remote url. 
 
 ### Install
 `pip install ovos-PHAL-plugin-wallpaper-manager`
 
 ## Event & API Details and Usage:
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/__init__.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager/downloadedProvider.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-wallpaper-manager
-Version: 0.0.0a2
+Version: 0.0.1a1
 Summary: A plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-wallpaper-manager
 Author: Aiix
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/ovos_PHAL_plugin_wallpaper_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-wallpaper-manager-0.0.0a2/setup.py` & `ovos-PHAL-plugin-wallpaper-manager-0.0.1a1/setup.py`

 * *Files identical despite different names*

