# Comparing `tmp/fluxoperator-0.0.23.tar.gz` & `tmp/fluxoperator-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.23.tar", last modified: Tue May 16 17:21:47 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.24.tar", last modified: Tue May 16 20:42:54 2023, max compression
```

## Comparing `fluxoperator-0.0.23.tar` & `fluxoperator-0.0.24.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.613923 fluxoperator-0.0.23/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6639 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5986 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.613923 fluxoperator-0.0.23/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.23/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-10 23:12:41.000000 fluxoperator-0.0.23/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-10 23:12:41.000000 fluxoperator-0.0.23/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13483 2023-05-16 20:42:46.000000 fluxoperator-0.0.24/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6639 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5986 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.138285 fluxoperator-0.0.24/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-16 20:42:54.000000 fluxoperator-0.0.24/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-16 20:42:53.000000 fluxoperator-0.0.24/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-16 20:42:54.000000 fluxoperator-0.0.24/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-16 20:42:46.000000 fluxoperator-0.0.24/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:42:54.142285 fluxoperator-0.0.24/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 20:18:09.000000 fluxoperator-0.0.24/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-05-16 20:15:38.000000 fluxoperator-0.0.24/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.23/PKG-INFO` & `fluxoperator-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.23
+Version: 0.0.24
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.23/fluxoperator/__init__.py` & `fluxoperator-0.0.24/fluxoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/api_client.py` & `fluxoperator-0.0.24/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/client.py` & `fluxoperator-0.0.24/fluxoperator/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -229,35 +229,53 @@
 
         self.c = client.Configuration.get_default_copy()
         self.c.assert_hostname = False
         client.Configuration.set_default(self.c)
         self._core_v1 = core_v1_api.CoreV1Api()
         return self._core_v1
 
-    def stream_output(self, filename, name=None, namespace=None, pod=None, stdout=True, timestamps=False):
+    def stream_output(
+        self,
+        filename,
+        name=None,
+        namespace=None,
+        pod=None,
+        stdout=True,
+        return_output=True,
+        timestamps=False,
+    ):
         """
         Stream output, optionally printing also to stdout.
+
+        Also return the output to the user.
         """
         namespace = namespace or self.namespace
         pod = pod or self.get_broker_pod(name=name, namespace=namespace).metadata.name
         watcher = watch.Watch()
 
-        # Stream output to file (should we return output too?)
+        # Stream output to file and return it if desired!
+        lines = []
         with open(filename, "w") as fd:
             for line in watcher.stream(
                 self.core_v1.read_namespaced_pod_log,
                 name=pod,
                 namespace=namespace,
                 timestamps=timestamps,
                 follow=True,
             ):
                 # Lines end with /r and we need to strip and add a newline
                 fd.write(line.strip() + "\n")
                 if stdout:
                     print(line)
+                if return_output:
+                    lines.append(line)
+
+        # I can imagine cases where we wouldn't want to keep it
+        if return_output:
+            return lines
 
     def kubectl_exec(self, command, pod=None, quiet=False, namespace=None, name=None):
         """
         Issue a command with kubectl exec
 
         A pod is required. If not provided, we retrieve (and wait for)
         the broker pod to be ready. If you are doing multiple commands
@@ -298,15 +316,15 @@
             # If name is present, filter down to pods with that prefix
             if name is not None:
                 pods = self._filter_pods(pods, name)
             return pods
 
         # Not found - it was deleted
         except kubernetes.client.exceptions.ApiException:
-             return V1PodList(items=[])
+            return V1PodList(items=[])
         except:
             time.sleep(2)
             return self.get_pods(namespace, name)
 
     def _filter_pods(self, pods, name):
         """
         Filter a set of pods (associated with a job) to a name prefix.
@@ -375,26 +393,28 @@
 
         ready = set()
         while len(ready) != size:
             logger.debug(f"{len(ready)} pods are ready, out of {size}")
             pod_list = self.get_pods(name=name, namespace=namespace)
 
             for pod in pod_list.items:
-                logger.debug(f"{pod.metadata.name} is in phase {pod.status.phase}")
+                print(f"{pod.metadata.name} is in phase {pod.status.phase}")
 
                 # Don't include the cert generator pod
                 if "cert-generator" in pod.metadata.name:
                     continue
 
                 # Ignore services pod
-                if pod.metadata.name.endswith('-services'):
+                if pod.metadata.name.endswith("-services"):
                     continue
                 if pod.status.phase not in states:
                     time.sleep(retry_seconds)
-                elif pod.status.phase not in ["Terminating", "Succeeded"]:
+                    continue
+
+                if pod.status.phase not in ["Terminating"]:
                     ready.add(pod.metadata.name)
 
         if not quiet:
             states = '" or "'.join(states)
             print(f'All pods are in states "{states}"')
         return pod_list
```

### Comparing `fluxoperator-0.0.23/fluxoperator/configuration.py` & `fluxoperator-0.0.24/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/decorator.py` & `fluxoperator-0.0.24/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/exceptions.py` & `fluxoperator-0.0.24/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/__init__.py` & `fluxoperator-0.0.24/fluxoperator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/commands.py` & `fluxoperator-0.0.24/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.24/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.24/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.24/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.24/fluxoperator/models/flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.24/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.24/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.24/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.24/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.24/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/models/security_context.py` & `fluxoperator-0.0.24/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/resource/network.py` & `fluxoperator-0.0.24/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/resource/pods.py` & `fluxoperator-0.0.24/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator/rest.py` & `fluxoperator-0.0.24/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.24/fluxoperator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.23
+Version: 0.0.24
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.23/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.24/fluxoperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/setup.py` & `fluxoperator-0.0.24/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.23",
+        version="0.0.24",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.23/test/test_commands.py` & `fluxoperator-0.0.24/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_container_resources.py` & `fluxoperator-0.0.24/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_container_volume.py` & `fluxoperator-0.0.24/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_flux_restful.py` & `fluxoperator-0.0.24/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_flux_spec.py` & `fluxoperator-0.0.24/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_flux_user.py` & `fluxoperator-0.0.24/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_life_cycle.py` & `fluxoperator-0.0.24/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_logging_spec.py` & `fluxoperator-0.0.24/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster.py` & `fluxoperator-0.0.24/test/test_mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.24/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_container.py` & `fluxoperator-0.0.24/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.24/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_list.py` & `fluxoperator-0.0.24/test/test_mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.24/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_status.py` & `fluxoperator-0.0.24/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_user.py` & `fluxoperator-0.0.24/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.24/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_pod_spec.py` & `fluxoperator-0.0.24/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.23/test/test_security_context.py` & `fluxoperator-0.0.24/test/test_security_context.py`

 * *Files identical despite different names*

