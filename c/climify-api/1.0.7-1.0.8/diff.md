# Comparing `tmp/climify_api-1.0.7.tar.gz` & `tmp/climify_api-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "climify_api-1.0.7.tar", last modified: Tue May  2 12:23:42 2023, max compression
+gzip compressed data, was "climify_api-1.0.8.tar", last modified: Tue May 16 10:35:48 2023, max compression
```

## Comparing `climify_api-1.0.7.tar` & `climify_api-1.0.8.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.199093 climify_api-1.0.7/
--rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.7/LICENSE
--rw-rw-rw-   0        0        0      932 2023-05-02 12:23:42.198094 climify_api-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.077757 climify_api-1.0.7/climify_api/
--rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.7/climify_api/ApiController.py
--rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.7/climify_api/REST.py
--rw-rw-rw-   0        0        0      904 2023-05-02 12:23:05.000000 climify_api-1.0.7/climify_api/__init__.py
--rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.7/climify_api/api_client.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.095871 climify_api-1.0.7/climify_api/apis/
--rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.7/climify_api/apis/PathBase.py
--rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.7/climify_api/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.099883 climify_api-1.0.7/climify_api/apis/v1/
--rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.7/climify_api/apis/v1/ApiController.py
--rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.7/climify_api/apis/v1/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.102053 climify_api-1.0.7/climify_api/apis/v1/paths/
--rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.7/climify_api/apis/v1/paths/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.107853 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id/
--rw-rw-rw-   0        0        0       70 2023-03-21 09:44:46.000000 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id/__init__.py
--rw-rw-rw-   0        0        0     3225 2023-04-04 10:10:47.000000 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.112177 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id_devices/
--rw-rw-rw-   0        0        0       85 2023-03-21 09:44:47.000000 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3286 2023-04-04 10:10:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.119074 climify_api-1.0.7/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/
--rw-rw-rw-   0        0        0      115 2023-04-11 09:18:32.000000 climify_api-1.0.7/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/__init__.py
--rw-rw-rw-   0        0        0     4283 2023-04-11 11:58:43.000000 climify_api-1.0.7/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.126593 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id/
--rw-rw-rw-   0        0        0       70 2023-03-21 09:44:49.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id/__init__.py
--rw-rw-rw-   0        0        0     3135 2023-04-04 10:11:09.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.132702 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_change_temperature/
--rw-rw-rw-   0        0        0      101 2023-03-21 09:44:51.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_change_temperature/__init__.py
--rw-rw-rw-   0        0        0     3585 2023-04-04 10:11:23.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_change_temperature/post.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.139844 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_devices/
--rw-rw-rw-   0        0        0       85 2023-03-21 09:44:53.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3218 2023-04-04 10:11:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.149581 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_sensor_values/
--rw-rw-rw-   0        0        0       96 2023-03-21 09:44:54.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_sensor_values/__init__.py
--rw-rw-rw-   0        0        0     7399 2023-05-02 12:19:53.000000 climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_sensor_values/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.156939 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id/
--rw-rw-rw-   0        0        0       60 2023-03-21 09:44:58.000000 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id/__init__.py
--rw-rw-rw-   0        0        0     3028 2023-04-04 10:11:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.169407 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id_devices/
--rw-rw-rw-   0        0        0       75 2023-03-21 09:45:00.000000 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3162 2023-04-04 10:11:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/maps_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.182893 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id/
--rw-rw-rw-   0        0        0       78 2023-03-21 09:45:02.000000 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id/__init__.py
--rw-rw-rw-   0        0        0     3295 2023-04-04 10:11:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.188651 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id_devices/
--rw-rw-rw-   0        0        0       93 2023-03-21 09:45:03.000000 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id_devices/__init__.py
--rw-rw-rw-   0        0        0     3341 2023-04-04 10:11:55.000000 climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id_devices/get.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.192982 climify_api-1.0.7/climify_api/apis/v1/paths/resources/
--rw-rw-rw-   0        0        0       71 2023-03-21 09:45:05.000000 climify_api-1.0.7/climify_api/apis/v1/paths/resources/__init__.py
--rw-rw-rw-   0        0        0     2543 2023-04-04 10:11:47.000000 climify_api-1.0.7/climify_api/apis/v1/paths/resources/get.py
--rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.7/climify_api/auth.py
--rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.7/climify_api/configuration.py
--rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.7/climify_api/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.195984 climify_api-1.0.7/climify_api/models/
--rw-rw-rw-   0        0        0     6779 2023-05-02 09:59:34.000000 climify_api-1.0.7/climify_api/models/__init__.py
--rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.7/climify_api/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-02 12:23:42.091110 climify_api-1.0.7/climify_api.egg-info/
--rw-rw-rw-   0        0        0      932 2023-05-02 12:23:41.000000 climify_api-1.0.7/climify_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1940 2023-05-02 12:23:42.000000 climify_api-1.0.7/climify_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 12:23:41.000000 climify_api-1.0.7/climify_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      159 2023-05-02 12:23:41.000000 climify_api-1.0.7/climify_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-02 12:23:41.000000 climify_api-1.0.7/climify_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2157 2023-05-02 12:22:02.000000 climify_api-1.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 12:23:42.199595 climify_api-1.0.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.492787 climify_api-1.0.8/
+-rw-rw-rw-   0        0        0     1087 2023-03-21 09:22:58.000000 climify_api-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0      932 2023-05-16 10:35:48.492787 climify_api-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       83 2023-03-21 09:16:33.000000 climify_api-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.382752 climify_api-1.0.8/climify_api/
+-rw-rw-rw-   0        0        0       64 2023-04-03 13:09:39.000000 climify_api-1.0.8/climify_api/ApiController.py
+-rw-rw-rw-   0        0        0    10812 2023-04-03 12:26:27.000000 climify_api-1.0.8/climify_api/REST.py
+-rw-rw-rw-   0        0        0      904 2023-05-16 10:35:08.000000 climify_api-1.0.8/climify_api/__init__.py
+-rw-rw-rw-   0        0        0    57575 2023-04-03 15:02:57.000000 climify_api-1.0.8/climify_api/api_client.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.397913 climify_api-1.0.8/climify_api/apis/
+-rw-rw-rw-   0        0        0     3490 2023-04-04 07:12:18.000000 climify_api-1.0.8/climify_api/apis/PathBase.py
+-rw-rw-rw-   0        0        0       78 2023-05-02 09:14:07.000000 climify_api-1.0.8/climify_api/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.405388 climify_api-1.0.8/climify_api/apis/v1/
+-rw-rw-rw-   0        0        0     1244 2023-04-11 09:19:16.000000 climify_api-1.0.8/climify_api/apis/v1/ApiController.py
+-rw-rw-rw-   0        0        0       59 2023-03-21 09:44:43.000000 climify_api-1.0.8/climify_api/apis/v1/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.407388 climify_api-1.0.8/climify_api/apis/v1/paths/
+-rw-rw-rw-   0        0        0      986 2023-04-11 09:18:57.000000 climify_api-1.0.8/climify_api/apis/v1/paths/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.412444 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:46.000000 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id/__init__.py
+-rw-rw-rw-   0        0        0     3225 2023-04-04 10:10:47.000000 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.418342 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:47.000000 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3286 2023-04-04 10:10:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.423109 climify_api-1.0.8/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/
+-rw-rw-rw-   0        0        0      115 2023-04-11 09:18:32.000000 climify_api-1.0.8/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/__init__.py
+-rw-rw-rw-   0        0        0     4283 2023-04-11 11:58:43.000000 climify_api-1.0.8/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.428665 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id/
+-rw-rw-rw-   0        0        0       70 2023-03-21 09:44:49.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id/__init__.py
+-rw-rw-rw-   0        0        0     3135 2023-04-04 10:11:09.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.434825 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_change_temperature/
+-rw-rw-rw-   0        0        0      101 2023-03-21 09:44:51.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_change_temperature/__init__.py
+-rw-rw-rw-   0        0        0     3585 2023-04-04 10:11:23.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_change_temperature/post.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.442119 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_devices/
+-rw-rw-rw-   0        0        0       85 2023-03-21 09:44:53.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3218 2023-04-04 10:11:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.449459 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_sensor_values/
+-rw-rw-rw-   0        0        0       96 2023-03-21 09:44:54.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_sensor_values/__init__.py
+-rw-rw-rw-   0        0        0     7589 2023-05-16 10:29:52.000000 climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_sensor_values/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.457875 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id/
+-rw-rw-rw-   0        0        0       60 2023-03-21 09:44:58.000000 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id/__init__.py
+-rw-rw-rw-   0        0        0     3028 2023-04-04 10:11:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.465595 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id_devices/
+-rw-rw-rw-   0        0        0       75 2023-03-21 09:45:00.000000 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3162 2023-04-04 10:11:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/maps_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.472793 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id/
+-rw-rw-rw-   0        0        0       78 2023-03-21 09:45:02.000000 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id/__init__.py
+-rw-rw-rw-   0        0        0     3295 2023-04-04 10:11:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.481305 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id_devices/
+-rw-rw-rw-   0        0        0       93 2023-03-21 09:45:03.000000 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id_devices/__init__.py
+-rw-rw-rw-   0        0        0     3341 2023-04-04 10:11:55.000000 climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id_devices/get.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.489337 climify_api-1.0.8/climify_api/apis/v1/paths/resources/
+-rw-rw-rw-   0        0        0       71 2023-03-21 09:45:05.000000 climify_api-1.0.8/climify_api/apis/v1/paths/resources/__init__.py
+-rw-rw-rw-   0        0        0     2543 2023-04-04 10:11:47.000000 climify_api-1.0.8/climify_api/apis/v1/paths/resources/get.py
+-rw-rw-rw-   0        0        0     4917 2023-04-03 07:43:48.000000 climify_api-1.0.8/climify_api/auth.py
+-rw-rw-rw-   0        0        0    17565 2023-03-31 14:33:08.000000 climify_api-1.0.8/climify_api/configuration.py
+-rw-rw-rw-   0        0        0     5258 2023-04-04 10:14:01.000000 climify_api-1.0.8/climify_api/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.490948 climify_api-1.0.8/climify_api/models/
+-rw-rw-rw-   0        0        0     6779 2023-05-02 09:59:34.000000 climify_api-1.0.8/climify_api/models/__init__.py
+-rw-rw-rw-   0        0        0   100123 2023-03-31 14:47:44.000000 climify_api-1.0.8/climify_api/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-16 10:35:48.391213 climify_api-1.0.8/climify_api.egg-info/
+-rw-rw-rw-   0        0        0      932 2023-05-16 10:35:48.000000 climify_api-1.0.8/climify_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1940 2023-05-16 10:35:48.000000 climify_api-1.0.8/climify_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 10:35:48.000000 climify_api-1.0.8/climify_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      159 2023-05-16 10:35:48.000000 climify_api-1.0.8/climify_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-16 10:35:48.000000 climify_api-1.0.8/climify_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2157 2023-05-16 10:35:08.000000 climify_api-1.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 10:35:48.493801 climify_api-1.0.8/setup.cfg
```

### Comparing `climify_api-1.0.7/LICENSE` & `climify_api-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/PKG-INFO` & `climify_api-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify_api
-Version: 1.0.7
+Version: 1.0.8
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.7/climify_api/REST.py` & `climify_api-1.0.8/climify_api/REST.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/__init__.py` & `climify_api-1.0.8/climify_api/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Provides a REST endpoints for Climify applications and 3rd party solutions.  # noqa: E501
 
     The version of the OpenAPI document: 1.2.3
     Generated by: https://openapi-generator.tech
 """
 
 __name__ = 'climify_api'
-__version__ = "1.0.7"
+__version__ = "1.0.8"
 
 # import ApiClient
 from climify_api.api_client import ApiClient
 
 # import Configuration
 from climify_api.configuration import Configuration, ClimifyRegion
```

### Comparing `climify_api-1.0.7/climify_api/api_client.py` & `climify_api-1.0.8/climify_api/api_client.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/PathBase.py` & `climify_api-1.0.8/climify_api/apis/PathBase.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/ApiController.py` & `climify_api-1.0.8/climify_api/apis/v1/ApiController.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/__init__.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/buildings_id_devices/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/buildings_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/feedback_forms_id_locations_id_responses/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/locations_id/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/locations_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_change_temperature/post.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_change_temperature/post.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_devices/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/locations_id_sensor_values/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/locations_id_sensor_values/get.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,19 @@
         
             if skip_deserialization:
                 bodies.append(response.data)
                 continue
             
             deserialized_body = parse_raw_as(List[SensorDataExtDto],response.data) if response.data\
                                 else []
+            
+            # Sort observations on time
+            for sensor in deserialized_body:
+                sensor.data = sorted(sensor.data, key=lambda x: x.time, reverse=True)
+
             if asDataFrame:
                 deserialized_body = convert_values_to_dataFrame(deserialized_body)
             
             bodies.append(deserialized_body)
 
         if skip_deserialization:
             response.data = bodies
```

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/maps_id/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/maps_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/maps_id_devices/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/maps_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/organisations_id_devices/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/organisations_id_devices/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/apis/v1/paths/resources/get.py` & `climify_api-1.0.8/climify_api/apis/v1/paths/resources/get.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/auth.py` & `climify_api-1.0.8/climify_api/auth.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/configuration.py` & `climify_api-1.0.8/climify_api/configuration.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/exceptions.py` & `climify_api-1.0.8/climify_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/models/__init__.py` & `climify_api-1.0.8/climify_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api/schemas.py` & `climify_api-1.0.8/climify_api/schemas.py`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/climify_api.egg-info/PKG-INFO` & `climify_api-1.0.8/climify_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: climify-api
-Version: 1.0.7
+Version: 1.0.8
 Summary: A wrapper library for the Climify REST API
 Author-email: Climify Aps <info@climify.com>
 Project-URL: Homepage, https://gitlab.climify.com/climify/python-api-lib
 Project-URL: Bug Tracker, https://gitlab.climify.com/climify/python-api-lib/-/issues
 Keywords: Climify,Environmental engineering
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `climify_api-1.0.7/climify_api.egg-info/SOURCES.txt` & `climify_api-1.0.8/climify_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `climify_api-1.0.7/pyproject.toml` & `climify_api-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
   "setuptools >= 61.0",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "climify_api"
-version = "1.0.7"
+version = "1.0.8"
 keywords=['Climify','Environmental engineering']
 authors = [
   { name="Climify Aps", email="info@climify.com" },
 ]
 description = "A wrapper library for the Climify REST API"
 #long_description = "A wrapper library for the Climify REST API, used to query sensor data and interact with Climify systems programmatically"
 readme = "README.md"
```

