# Comparing `tmp/ovos-PHAL-plugin-configuration-provider-1.0.0a3.tar.gz` & `tmp/ovos-PHAL-plugin-configuration-provider-1.0.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-PHAL-plugin-configuration-provider-1.0.0a3.tar", last modified: Sun Oct 16 00:54:28 2022, max compression
+gzip compressed data, was "ovos-PHAL-plugin-configuration-provider-1.0.1a1.tar", last modified: Tue Apr  4 22:32:20 2023, max compression
```

## Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3.tar` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 00:54:28.378547 ovos-PHAL-plugin-configuration-provider-1.0.0a3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-16 00:54:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-16 00:54:28.378547 ovos-PHAL-plugin-configuration-provider-1.0.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-10-16 00:54:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 00:54:28.374547 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider/
--rw-r--r--   0 runner    (1001) docker     (121)    11111 2022-10-16 00:54:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-10-16 00:54:23.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-16 00:54:28.378547 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      128 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-16 00:54:28.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-16 00:54:28.378547 ovos-PHAL-plugin-configuration-provider-1.0.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3048 2022-10-16 00:54:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.370077 ovos-PHAL-plugin-configuration-provider-1.0.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-04 22:32:10.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-04 22:32:20.370077 ovos-PHAL-plugin-configuration-provider-1.0.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-04-04 22:32:10.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.370077 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 2023-04-04 22:32:10.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-04 22:32:14.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:32:20.370077 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:32:20.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:32:20.370077 ovos-PHAL-plugin-configuration-provider-1.0.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-04-04 22:32:10.000000 ovos-PHAL-plugin-configuration-provider-1.0.1a1/setup.py
```

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/LICENSE` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/PKG-INFO` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-configuration-provider
-Version: 1.0.0a3
+Version: 1.0.1a1
 Summary: Configuration provider plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-configuration-provider
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/README.md` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/README.md`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider/__init__.py` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/PKG-INFO` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-PHAL-plugin-configuration-provider
-Version: 1.0.0a3
+Version: 1.0.1a1
 Summary: Configuration provider plugin for OpenVoiceOS hardware abstraction layer
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-configuration-provider
 Author: AIIX
 Author-email: aix.m@outlook.com
 License: Apache-2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/ovos_PHAL_plugin_configuration_provider.egg-info/SOURCES.txt` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/ovos_PHAL_plugin_configuration_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-PHAL-plugin-configuration-provider-1.0.0a3/setup.py` & `ovos-PHAL-plugin-configuration-provider-1.0.1a1/setup.py`

 * *Files identical despite different names*

