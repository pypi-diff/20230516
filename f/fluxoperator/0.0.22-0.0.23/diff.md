# Comparing `tmp/fluxoperator-0.0.22.tar.gz` & `tmp/fluxoperator-0.0.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.22.tar", last modified: Fri May  5 19:00:14 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.23.tar", last modified: Tue May 16 17:21:47 2023, max compression
```

## Comparing `fluxoperator-0.0.22.tar` & `fluxoperator-0.0.23.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-02 21:28:30.000000 fluxoperator-0.0.22/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.628271 fluxoperator-0.0.22/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5816 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5811 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.628271 fluxoperator-0.0.22/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-05 19:00:13.000000 fluxoperator-0.0.22/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.22/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_flux_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8167 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17751 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1364 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.613923 fluxoperator-0.0.23/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6639 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5986 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.613923 fluxoperator-0.0.23/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.609923 fluxoperator-0.0.23/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.23/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-16 17:21:47.000000 fluxoperator-0.0.23/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-16 17:21:47.617923 fluxoperator-0.0.23/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-14 21:11:51.000000 fluxoperator-0.0.23/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-10 21:19:30.000000 fluxoperator-0.0.23/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8175 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1370 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-10 23:12:41.000000 fluxoperator-0.0.23/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17767 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-10 23:12:41.000000 fluxoperator-0.0.23/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1539 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1396 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1990 2023-05-11 01:21:46.000000 fluxoperator-0.0.23/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.23/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.22/PKG-INFO` & `fluxoperator-0.0.23/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.22
+Version: 0.0.23
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.22/fluxoperator/__init__.py` & `fluxoperator-0.0.23/fluxoperator/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/api_client.py` & `fluxoperator-0.0.23/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/client.py` & `fluxoperator-0.0.23/fluxoperator/client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/configuration.py` & `fluxoperator-0.0.23/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/decorator.py` & `fluxoperator-0.0.23/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/exceptions.py` & `fluxoperator-0.0.23/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/__init__.py` & `fluxoperator-0.0.23/fluxoperator/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/commands.py` & `fluxoperator-0.0.23/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.23/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.23/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.23/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/flux_spec.py` & `fluxoperator-0.0.23/fluxoperator/models/flux_spec.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,37 +30,42 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'connect_timeout': 'str',
+        'install_root': 'str',
         'log_level': 'int',
         'option_flags': 'str'
     }
 
     attribute_map = {
         'connect_timeout': 'connectTimeout',
+        'install_root': 'installRoot',
         'log_level': 'logLevel',
         'option_flags': 'optionFlags'
     }
 
-    def __init__(self, connect_timeout='5s', log_level=6, option_flags='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, connect_timeout='5s', install_root='/usr', log_level=6, option_flags='', local_vars_configuration=None):  # noqa: E501
         """FluxSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._connect_timeout = None
+        self._install_root = None
         self._log_level = None
         self._option_flags = None
         self.discriminator = None
 
         if connect_timeout is not None:
             self.connect_timeout = connect_timeout
+        if install_root is not None:
+            self.install_root = install_root
         if log_level is not None:
             self.log_level = log_level
         if option_flags is not None:
             self.option_flags = option_flags
 
     @property
     def connect_timeout(self):
@@ -82,14 +87,37 @@
         :param connect_timeout: The connect_timeout of this FluxSpec.  # noqa: E501
         :type connect_timeout: str
         """
 
         self._connect_timeout = connect_timeout
 
     @property
+    def install_root(self):
+        """Gets the install_root of this FluxSpec.  # noqa: E501
+
+        Install root location  # noqa: E501
+
+        :return: The install_root of this FluxSpec.  # noqa: E501
+        :rtype: str
+        """
+        return self._install_root
+
+    @install_root.setter
+    def install_root(self, install_root):
+        """Sets the install_root of this FluxSpec.
+
+        Install root location  # noqa: E501
+
+        :param install_root: The install_root of this FluxSpec.  # noqa: E501
+        :type install_root: str
+        """
+
+        self._install_root = install_root
+
+    @property
     def log_level(self):
         """Gets the log_level of this FluxSpec.  # noqa: E501
 
         Log level to use for flux logging (only in non TestMode)  # noqa: E501
 
         :return: The log_level of this FluxSpec.  # noqa: E501
         :rtype: int
```

### Comparing `fluxoperator-0.0.22/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.23/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.23/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.23/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_status.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,38 +31,38 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'conditions': 'list[V1Condition]',
         'jobid': 'str',
-        'size': 'int'
+        'maximum_size': 'int'
     }
 
     attribute_map = {
         'conditions': 'conditions',
         'jobid': 'jobid',
-        'size': 'size'
+        'maximum_size': 'maximumSize'
     }
 
-    def __init__(self, conditions=None, jobid='', size=0, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, conditions=None, jobid='', maximum_size=0, local_vars_configuration=None):  # noqa: E501
         """MiniClusterStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._conditions = None
         self._jobid = None
-        self._size = None
+        self._maximum_size = None
         self.discriminator = None
 
         if conditions is not None:
             self.conditions = conditions
         self.jobid = jobid
-        self.size = size
+        self.maximum_size = maximum_size
 
     @property
     def conditions(self):
         """Gets the conditions of this MiniClusterStatus.  # noqa: E501
 
         conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
@@ -105,37 +105,37 @@
         """
         if self.local_vars_configuration.client_side_validation and jobid is None:  # noqa: E501
             raise ValueError("Invalid value for `jobid`, must not be `None`")  # noqa: E501
 
         self._jobid = jobid
 
     @property
-    def size(self):
-        """Gets the size of this MiniClusterStatus.  # noqa: E501
+    def maximum_size(self):
+        """Gets the maximum_size of this MiniClusterStatus.  # noqa: E501
 
         We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
 
-        :return: The size of this MiniClusterStatus.  # noqa: E501
+        :return: The maximum_size of this MiniClusterStatus.  # noqa: E501
         :rtype: int
         """
-        return self._size
+        return self._maximum_size
 
-    @size.setter
-    def size(self, size):
-        """Sets the size of this MiniClusterStatus.
+    @maximum_size.setter
+    def maximum_size(self, maximum_size):
+        """Sets the maximum_size of this MiniClusterStatus.
 
         We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
 
-        :param size: The size of this MiniClusterStatus.  # noqa: E501
-        :type size: int
+        :param maximum_size: The maximum_size of this MiniClusterStatus.  # noqa: E501
+        :type maximum_size: int
         """
-        if self.local_vars_configuration.client_side_validation and size is None:  # noqa: E501
-            raise ValueError("Invalid value for `size`, must not be `None`")  # noqa: E501
+        if self.local_vars_configuration.client_side_validation and maximum_size is None:  # noqa: E501
+            raise ValueError("Invalid value for `maximum_size`, must not be `None`")  # noqa: E501
 
-        self._size = size
+        self._maximum_size = maximum_size
 
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
```

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.23/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.23/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/models/security_context.py` & `fluxoperator-0.0.23/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/resource/network.py` & `fluxoperator-0.0.23/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/resource/pods.py` & `fluxoperator-0.0.23/fluxoperator/resource/pods.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator/rest.py` & `fluxoperator-0.0.23/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.23/fluxoperator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.22
+Version: 0.0.23
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
```

### Comparing `fluxoperator-0.0.22/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.23/fluxoperator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/setup.py` & `fluxoperator-0.0.23/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.22",
+        version="0.0.23",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.22/test/test_commands.py` & `fluxoperator-0.0.23/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_container_resources.py` & `fluxoperator-0.0.23/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_container_volume.py` & `fluxoperator-0.0.23/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_flux_restful.py` & `fluxoperator-0.0.23/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_flux_spec.py` & `fluxoperator-0.0.23/test/test_flux_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_flux_user.py` & `fluxoperator-0.0.23/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_life_cycle.py` & `fluxoperator-0.0.23/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_logging_spec.py` & `fluxoperator-0.0.23/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster.py` & `fluxoperator-0.0.23/test/test_mini_cluster.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                             volume_handle = '', )
                         }, ), 
                 status = fluxoperator.models.mini_cluster_status.MiniClusterStatus(
                     conditions = [
                         None
                         ], 
                     jobid = '', 
-                    size = 56, )
+                    maximum_size = 56, )
             )
         else :
             return MiniCluster(
         )
 
     def testMiniCluster(self):
         """Test MiniCluster"""
```

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.23/test/test_mini_cluster_user.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_archive import MiniClusterArchive  # noqa: E501
+from fluxoperator.models.mini_cluster_user import MiniClusterUser  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
-class TestMiniClusterArchive(unittest.TestCase):
-    """MiniClusterArchive unit test stubs"""
+class TestMiniClusterUser(unittest.TestCase):
+    """MiniClusterUser unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test MiniClusterArchive
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
-        # model = fluxoperator.models.mini_cluster_archive.MiniClusterArchive()  # noqa: E501
-        if include_optional:
-            return MiniClusterArchive(path="")
-        else:
-            return MiniClusterArchive()
+        """Test MiniClusterUser
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
+        # model = fluxoperator.models.mini_cluster_user.MiniClusterUser()  # noqa: E501
+        if include_optional :
+            return MiniClusterUser(
+                name = '', 
+                password = ''
+            )
+        else :
+            return MiniClusterUser(
+                name = '',
+        )
 
-    def testMiniClusterArchive(self):
-        """Test MiniClusterArchive"""
+    def testMiniClusterUser(self):
+        """Test MiniClusterUser"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_container.py` & `fluxoperator-0.0.23/test/test_mini_cluster_container.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.23/test/test_mini_cluster_existing_volume.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,44 +12,44 @@
 
 from __future__ import absolute_import
 
 import unittest
 import datetime
 
 import fluxoperator
-from fluxoperator.models.mini_cluster_existing_volume import (
-    MiniClusterExistingVolume,
-)  # noqa: E501
+from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
 class TestMiniClusterExistingVolume(unittest.TestCase):
     """MiniClusterExistingVolume unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterExistingVolume
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
         # model = fluxoperator.models.mini_cluster_existing_volume.MiniClusterExistingVolume()  # noqa: E501
-        if include_optional:
-            return MiniClusterExistingVolume(claim_name="", path="", read_only=True)
-        else:
+        if include_optional :
             return MiniClusterExistingVolume(
-                claim_name="",
-                path="",
+                claim_name = '', 
+                path = '', 
+                read_only = True
             )
+        else :
+            return MiniClusterExistingVolume(
+                claim_name = '',
+                path = '',
+        )
 
     def testMiniClusterExistingVolume(self):
         """Test MiniClusterExistingVolume"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_list.py` & `fluxoperator-0.0.23/test/test_mini_cluster_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
                                     volume_handle = '', )
                                 }, ), 
                         status = fluxoperator.models.mini_cluster_status.MiniClusterStatus(
                             conditions = [
                                 None
                                 ], 
                             jobid = '', 
-                            size = 56, ), )
+                            maximum_size = 56, ), )
                     ], 
                 kind = '', 
                 metadata = None
             )
         else :
             return MiniClusterList(
                 items = [
@@ -330,15 +330,15 @@
                                     volume_handle = '', )
                                 }, ), 
                         status = fluxoperator.models.mini_cluster_status.MiniClusterStatus(
                             conditions = [
                                 None
                                 ], 
                             jobid = '', 
-                            size = 56, ), )
+                            maximum_size = 56, ), )
                     ],
         )
 
     def testMiniClusterList(self):
         """Test MiniClusterList"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
```

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_spec.py` & `fluxoperator-0.0.23/test/test_mini_cluster_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_mini_cluster_status.py` & `fluxoperator-0.0.23/test/test_mini_cluster_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,38 +15,43 @@
 import unittest
 import datetime
 
 import fluxoperator
 from fluxoperator.models.mini_cluster_status import MiniClusterStatus  # noqa: E501
 from fluxoperator.rest import ApiException
 
-
 class TestMiniClusterStatus(unittest.TestCase):
     """MiniClusterStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
         """Test MiniClusterStatus
-        include_option is a boolean, when False only required
-        params are included, when True both required and
-        optional params are included"""
+            include_option is a boolean, when False only required
+            params are included, when True both required and
+            optional params are included """
         # model = fluxoperator.models.mini_cluster_status.MiniClusterStatus()  # noqa: E501
-        if include_optional:
-            return MiniClusterStatus(conditions=[None], jobid="")
-        else:
+        if include_optional :
             return MiniClusterStatus(
-                jobid="",
+                conditions = [
+                    None
+                    ], 
+                jobid = '', 
+                maximum_size = 56
             )
+        else :
+            return MiniClusterStatus(
+                jobid = '',
+                maximum_size = 56,
+        )
 
     def testMiniClusterStatus(self):
         """Test MiniClusterStatus"""
         inst_req_only = self.make_instance(include_optional=False)
         inst_req_and_optional = self.make_instance(include_optional=True)
 
-
-if __name__ == "__main__":
+if __name__ == '__main__':
     unittest.main()
```

### Comparing `fluxoperator-0.0.22/test/test_pod_spec.py` & `fluxoperator-0.0.23/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.22/test/test_security_context.py` & `fluxoperator-0.0.23/test/test_security_context.py`

 * *Files identical despite different names*

