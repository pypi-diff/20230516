# Comparing `tmp/PyFlyt-0.7.1.tar.gz` & `tmp/PyFlyt-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyFlyt-0.7.1.tar", last modified: Mon May 15 15:53:26 2023, max compression
+gzip compressed data, was "PyFlyt-0.7.2.tar", last modified: Tue May 16 17:32:35 2023, max compression
```

## Comparing `PyFlyt-0.7.1.tar` & `PyFlyt-0.7.2.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.7.1/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PKG-INFO
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.556448 PyFlyt-0.7.1/PyFlyt/
--rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.560449 PyFlyt-0.7.1/PyFlyt/core/
--rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.7.1/PyFlyt/core/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.564448 PyFlyt-0.7.1/PyFlyt/core/abstractions/
--rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_controller.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_drone.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/base_wind_field.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/boosters.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     4454 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/boring_bodies.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/camera.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/gimbals.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    15316 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/lifting_surfaces.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/motors.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/core/abstractions/pid.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    17975 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/aviary.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/core/drones/
--rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.7.1/PyFlyt/core/drones/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9440 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/core/drones/fixedwing.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    18407 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/drones/quadx.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    11574 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/drones/rocket.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/core/load_objs.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/core/wind/
--rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/core/wind/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.568448 PyFlyt-0.7.1/PyFlyt/gym_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/__init__.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.572449 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/
--rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-11 16:33:17.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-27 15:02:04.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/gym_envs/waypoint_handler.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.576449 PyFlyt-0.7.1/PyFlyt/models/
--rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.7.1/PyFlyt/models/landing_pad.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.7.1/PyFlyt/models/race_gate.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.7.1/PyFlyt/models/target.urdf
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.556448 PyFlyt-0.7.1/PyFlyt/models/vehicles/
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.576449 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/
--rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2.dae
--rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/
--rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/
--rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/
--rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.urdf
--rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.yaml
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.560449 PyFlyt-0.7.1/PyFlyt.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)     4098 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       49 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-15 15:53:26.000000 PyFlyt-0.7.1/PyFlyt.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)     1171 2023-05-15 15:52:13.000000 PyFlyt-0.7.1/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 15:14:17.000000 PyFlyt-0.7.1/readme.md
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-02 11:06:46.000000 PyFlyt-0.7.1/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-15 15:53:26.580448 PyFlyt-0.7.1/tests/
--rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-15 11:28:20.000000 PyFlyt-0.7.1/tests/test_core.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-03-21 13:48:00.000000 PyFlyt-0.7.1/tests/test_gym_envs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1036 2022-06-30 13:35:00.000000 PyFlyt-0.7.2/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PKG-INFO
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.519900 PyFlyt-0.7.2/PyFlyt/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       85 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/PyFlyt/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.523900 PyFlyt-0.7.2/PyFlyt/core/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      178 2023-03-07 16:22:47.000000 PyFlyt-0.7.2/PyFlyt/core/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.523900 PyFlyt-0.7.2/PyFlyt/core/abstractions/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      396 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      601 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/base_controller.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    12406 2023-05-16 17:24:04.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/base_drone.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2840 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/base_wind_field.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11845 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/boosters.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4955 2023-05-16 17:21:09.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/boring_bodies.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7695 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/camera.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7376 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/gimbals.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15799 2023-05-16 17:21:22.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/lifting_surfaces.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6757 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/motors.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1832 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/PyFlyt/core/abstractions/pid.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    19052 2023-05-16 17:31:41.000000 PyFlyt-0.7.2/PyFlyt/core/aviary.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/core/drones/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      132 2023-04-11 16:33:17.000000 PyFlyt-0.7.2/PyFlyt/core/drones/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9686 2023-05-16 17:13:33.000000 PyFlyt-0.7.2/PyFlyt/core/drones/fixedwing.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    18406 2023-05-16 17:12:54.000000 PyFlyt-0.7.2/PyFlyt/core/drones/quadx.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11914 2023-05-16 17:14:09.000000 PyFlyt-0.7.2/PyFlyt/core/drones/rocket.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2254 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/PyFlyt/core/load_objs.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/core/wind/
+-rw-rw-r--   0 jet       (1000) jet       (1000)       46 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/core/wind/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/gym_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      798 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/__init__.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/gym_envs/fixedwing_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9211 2023-04-07 18:11:27.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6228 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8945 2023-04-07 18:11:27.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10073 2023-03-21 13:48:00.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3973 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6877 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/gym_envs/rocket_envs/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    11585 2023-04-11 16:33:17.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     9736 2023-04-27 15:02:04.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     6306 2023-04-07 18:11:27.000000 PyFlyt-0.7.2/PyFlyt/gym_envs/waypoint_handler.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.527901 PyFlyt-0.7.2/PyFlyt/models/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      441 2023-02-28 12:51:18.000000 PyFlyt-0.7.2/PyFlyt/models/landing_pad.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2533 2022-06-30 13:35:00.000000 PyFlyt-0.7.2/PyFlyt/models/race_gate.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      452 2023-02-28 12:51:18.000000 PyFlyt-0.7.2/PyFlyt/models/target.urdf
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.519900 PyFlyt-0.7.2/PyFlyt/models/vehicles/
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/
+-rw-rw-r--   0 jet       (1000) jet       (1000)   529735 2022-11-22 14:06:54.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2.dae
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2929 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1262 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PyFlyt/models/vehicles/fixedwing/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4711 2023-03-21 13:48:00.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2558 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PyFlyt/models/vehicles/primitive_drone/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     3850 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1257 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PyFlyt/models/vehicles/quadplane/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5907 2023-02-07 01:25:05.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2618 2023-02-07 01:25:05.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/PyFlyt/models/vehicles/rocket/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     7191 2023-04-07 18:11:27.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/rocket/rocket.urdf
+-rw-rw-r--   0 jet       (1000) jet       (1000)      976 2023-04-07 18:11:27.000000 PyFlyt-0.7.2/PyFlyt/models/vehicles/rocket/rocket.yaml
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.523900 PyFlyt-0.7.2/PyFlyt.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4179 2023-05-16 17:32:35.000000 PyFlyt-0.7.2/PyFlyt.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1968 2023-05-16 17:32:35.000000 PyFlyt-0.7.2/PyFlyt.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-16 17:32:35.000000 PyFlyt-0.7.2/PyFlyt.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       49 2023-05-16 17:32:35.000000 PyFlyt-0.7.2/PyFlyt.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        7 2023-05-16 17:32:35.000000 PyFlyt-0.7.2/PyFlyt.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1242 2023-05-16 17:32:26.000000 PyFlyt-0.7.2/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2283 2023-04-27 15:14:17.000000 PyFlyt-0.7.2/readme.md
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)      462 2023-03-02 11:06:46.000000 PyFlyt-0.7.2/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-16 17:32:35.531902 PyFlyt-0.7.2/tests/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     8603 2023-05-15 11:28:20.000000 PyFlyt-0.7.2/tests/test_core.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5300 2023-03-21 13:48:00.000000 PyFlyt-0.7.2/tests/test_gym_envs.py
```

### Comparing `PyFlyt-0.7.1/LICENSE.txt` & `PyFlyt-0.7.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PKG-INFO` & `PyFlyt-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.1
+Version: 0.7.2
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,14 +20,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/jjshoots/PyFlyt
+Project-URL: Documentation, https://jjshoots.github.io/PyFlyt/documentation.html
 Project-URL: Bug Report, https://github.com/jjshoots/PyFlyt/issues
 Keywords: Reinforcement Learning,UAVs,drones,Quadcopter,AI,RL,Gymnasium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_controller.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/base_controller.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_drone.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/base_drone.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/base_wind_field.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/base_wind_field.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/boosters.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/boosters.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/boring_bodies.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/boring_bodies.py`

 * *Files 10% similar despite different names*

```diff
@@ -90,14 +90,25 @@
         if self.p.wind_field is not None:
             body_positions = np.array([item[0] for item in link_states])
             body_velocities -= self.p.wind_field(self.p.elapsed_time, body_positions)
 
         # rotate all velocities to be in local frame
         body_velocities = np.matmul(rotation_matrix, body_velocities.T).T
 
+        if rotation_matrix.shape == (len(self.body_ids), 3, 3):
+            body_velocities = np.matmul(
+                rotation_matrix, np.expand_dims(body_velocities, -1)
+            ).squeeze(-1)
+        elif rotation_matrix.shape == (3, 3):
+            body_velocities = np.matmul(rotation_matrix, body_velocities.T).T
+        else:
+            raise ValueError(
+                f"Only accept (num_bodies, 3, 3) or (3, 3) array for `rotation_matrix`, got {rotation_matrix.shape}."
+            )
+
         # update the variable
         self.local_body_velocities = body_velocities
 
     def physics_update(self):
         """Applies a force to the boring bodies depending on their local surface velocities."""
         forces = (
             -np.sign(self.local_body_velocities)
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/camera.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/camera.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/gimbals.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/gimbals.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/lifting_surfaces.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/lifting_surfaces.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
             surface.physics_update(actuation)
 
     def state_update(self, rotation_matrix: np.ndarray):
         """Updates all local surface velocities of the lifting surface, place under `update_state`.
 
         Args:
-            rotation_matrix (np.ndarray): (3, 3) rotation_matrix of the main body
+            rotation_matrix (np.ndarray): (3, 3) OR (num_surfaces, 3, 3) array rotation_matrix
         """
         # get all the states for all the surfaces
         link_states = self.p.getLinkStates(
             self.uav_id, self.surface_ids, computeLinkVelocity=True
         )
 
         # get all the velocities
@@ -82,16 +82,25 @@
         # query for wind if available and add to surface velocities
         if self.p.wind_field is not None:
             surface_positions = np.array([item[0] for item in link_states])
             surface_velocities -= self.p.wind_field(
                 self.p.elapsed_time, surface_positions
             )
 
-        # convert all to local velocities
-        surface_velocities = np.matmul(rotation_matrix, surface_velocities.T).T
+        # convert all to local velocities, depending on rotation matrix style
+        if rotation_matrix.shape == (len(self.surfaces), 3, 3):
+            surface_velocities = np.matmul(
+                rotation_matrix, np.expand_dims(surface_velocities, -1)
+            ).squeeze(-1)
+        elif rotation_matrix.shape == (3, 3):
+            surface_velocities = np.matmul(rotation_matrix, surface_velocities.T).T
+        else:
+            raise ValueError(
+                f"Only accept (num_surfaces, 3, 3) or (3, 3) array for `rotation_matrix`, got {rotation_matrix.shape}."
+            )
 
         # update the velocities of all surfaces
         for surface, velocity in zip(self.surfaces, surface_velocities):
             surface.state_update(velocity)
 
 
 class LiftingSurface:
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/motors.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/motors.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/abstractions/pid.py` & `PyFlyt-0.7.2/PyFlyt/core/abstractions/pid.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/core/aviary.py` & `PyFlyt-0.7.2/PyFlyt/core/aviary.py`

 * *Files 4% similar despite different names*

```diff
@@ -270,37 +270,57 @@
         assert callable(wind_field), "`wind_field` function must be callable."
         WindFieldClass._check_wind_field_validity(wind_field)
         self.wind_field = wind_field
 
     def state(self, index: DroneIndex) -> np.ndarray:
         """Returns the state for the indexed drone.
 
+        This is a (4, 3) array, where:
+            - `state[0, :]` represents body frame angular velocity
+            - `state[1, :]` represents ground frame angular position
+            - `state[2, :]` represents body frame linear velocity
+            - `state[3, :]` represents ground frame linear position
+
         Args:
             index (DRONE_INDEX): index
 
         Returns:
             np.ndarray: state
         """
         return self.drones[index].state
 
     def aux_state(self, index: DroneIndex) -> np.ndarray:
         """Returns the auxiliary state for the indexed drone.
 
+        This is typically an (n, ) vector, representing various attributes such as:
+            - booster thrust settings
+            - fuel remaining
+            - control surfaces deflection magnitude
+            - etc...
+
         Args:
             index (DRONE_INDEX): index
 
         Returns:
             np.ndarray: auxiliary state
         """
         return self.drones[index].aux_state
 
     @property
     def all_states(self) -> list[np.ndarray]:
         """Returns a list of states for all drones in the environment.
 
+        This is a `num_drones` list of (4, 3) arrays, where each element in the list corresponds to the i-th drone state.
+
+        Similar to the `state` property, the states contain information corresponding to:
+            - `state[0, :]` represents body frame angular velocity
+            - `state[1, :]` represents ground frame angular position
+            - `state[2, :]` represents body frame linear velocity
+            - `state[3, :]` represents ground frame linear position
+
         This function is not very optimized, if you want the state of a single drone, do `state(i)`.
 
         Returns:
             np.ndarray: list of states
         """
         states = []
         for drone in self.drones:
@@ -308,14 +328,16 @@
 
         return states
 
     @property
     def all_aux_states(self) -> list[np.ndarray]:
         """Returns a list of auxiliary states for all drones in the environment.
 
+        This is a `num_drones` list of auxiliary states.
+
         This function is not very optimized, if you want the aux state of a single drone, do `aux_state(i)`.
 
         Returns:
             np.ndarray: list of auxiliary states
         """
         aux_states = []
         for drone in self.drones:
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/drones/fixedwing.py` & `PyFlyt-0.7.2/PyFlyt/core/drones/fixedwing.py`

 * *Files 3% similar despite different names*

```diff
@@ -191,14 +191,25 @@
 
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.p.resetBaseVelocity(self.Id, self.starting_velocity, [0, 0, 0])
         self.disable_artificial_damping()
         self.lifting_surfaces.reset()
         self.motors.reset()
 
+    def set_mode(self, mode):
+        """Sets the current flight mode of the vehicle.
+
+        flight modes:
+            - 0: Pitch, Roll, Yaw, Thrust
+
+        Args:
+            mode (int): flight mode
+        """
+        super().set_mode(mode)
+
     def update_control(self):
         """Runs through controllers."""
         # the default mode
         if self.mode == 0:
             self.cmd = self.setpoint
             return
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/drones/quadx.py` & `PyFlyt-0.7.2/PyFlyt/core/drones/quadx.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,15 +228,14 @@
             - u, v, w = local linear velocities
             - x, y, z = linear positions
             - vx, vy, vz = ground linear velocities
             - T = thrust
 
         Args:
             mode (int): flight mode
-
         """
         if (mode < -1 or mode > 7) and mode not in self.registered_controllers.keys():
             raise ValueError(
                 f"`mode` must be between -1 and 7 or be registered in {self.registered_controllers.keys()=}, got {mode}."
             )
 
         self.mode = mode
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/drones/rocket.py` & `PyFlyt-0.7.2/PyFlyt/core/drones/rocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -222,14 +222,25 @@
         self.p.resetBasePositionAndOrientation(self.Id, self.start_pos, self.start_orn)
         self.disable_artificial_damping()
         self.bodies.reset()
         self.lifting_surfaces.reset()
         self.booster_gimbal.reset()
         self.boosters.reset(starting_fuel_ratio=self.starting_fuel_ratio)
 
+    def set_mode(self, mode):
+        """Sets the current flight mode of the vehicle.
+
+        flight modes:
+            - 0: finlet x deflection, finlet y deflection, finlet yaw, ignition, throttle, booster gimbal axis 1, booster gimbal axis 2
+
+        Args:
+            mode (int): flight mode
+        """
+        super().set_mode(mode)
+
     def update_control(self):
         """Runs through controllers."""
         # the default mode
         if self.mode == 0:
             # finlet mapping
             finlet_cmd = self.finlet_map @ np.expand_dims(self.setpoint[:3], axis=-1)
             finlet_cmd = np.clip(finlet_cmd, -1.0, 1.0)
```

### Comparing `PyFlyt-0.7.1/PyFlyt/core/load_objs.py` & `PyFlyt-0.7.2/PyFlyt/core/load_objs.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/__init__.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/fixedwing_envs/fixedwing_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_gates_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_hover_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/quadx_envs/quadx_waypoints_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/rocket_envs/rocket_base_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/rocket_envs/rocket_landing_env.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/gym_envs/waypoint_handler.py` & `PyFlyt-0.7.2/PyFlyt/gym_envs/waypoint_handler.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/race_gate.urdf` & `PyFlyt-0.7.2/PyFlyt/models/race_gate.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2.dae` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2.dae`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.urdf` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2x.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/cf2x/cf2x.yaml` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/cf2x/cf2x.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/fixedwing/fixedwing.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/fixedwing/fixedwing.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/primitive_drone/primitive_drone.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.urdf` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/quadplane/quadplane.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/quadplane/quadplane.yaml` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/quadplane/quadplane.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.urdf` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/rocket/rocket.urdf`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt/models/vehicles/rocket/rocket.yaml` & `PyFlyt-0.7.2/PyFlyt/models/vehicles/rocket/rocket.yaml`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/PyFlyt.egg-info/PKG-INFO` & `PyFlyt-0.7.2/PyFlyt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFlyt
-Version: 0.7.1
+Version: 0.7.2
 Summary: UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research.
 Author-email: Jet <taijunjet@hotmail.com>
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -20,14 +20,15 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Repository, https://github.com/jjshoots/PyFlyt
+Project-URL: Documentation, https://jjshoots.github.io/PyFlyt/documentation.html
 Project-URL: Bug Report, https://github.com/jjshoots/PyFlyt/issues
 Keywords: Reinforcement Learning,UAVs,drones,Quadcopter,AI,RL,Gymnasium
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `PyFlyt-0.7.1/PyFlyt.egg-info/SOURCES.txt` & `PyFlyt-0.7.2/PyFlyt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/pyproject.toml` & `PyFlyt-0.7.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "PyFlyt"
-version = "0.7.1"
+version = "0.7.2"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "UAV Flight Simulator Gymnasium Environments for Reinforcement Learning Research."
 readme = "readme.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -24,14 +24,15 @@
 include-package-data = true
 
 [tool.setuptools.packages.find]
 include = ["PyFlyt", "PyFlyt.*"]
 
 [project.urls]
 Repository = "https://github.com/jjshoots/PyFlyt"
+Documentation = "https://jjshoots.github.io/PyFlyt/documentation.html"
 "Bug Report" = "https://github.com/jjshoots/PyFlyt/issues"
 
 #######################################################################################
 # linters
 #######################################################################################
 [tool.pyright]
 reportMissingImports = "none"
```

### Comparing `PyFlyt-0.7.1/readme.md` & `PyFlyt-0.7.2/readme.md`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/tests/test_core.py` & `PyFlyt-0.7.2/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `PyFlyt-0.7.1/tests/test_gym_envs.py` & `PyFlyt-0.7.2/tests/test_gym_envs.py`

 * *Files identical despite different names*

