# Comparing `tmp/honeybee-doe2-0.0.4.tar.gz` & `tmp/honeybee-doe2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-doe2-0.0.4.tar", last modified: Mon May 15 23:02:15 2023, max compression
+gzip compressed data, was "dist/honeybee-doe2-0.0.5.tar", last modified: Tue May 16 02:06:32 2023, max compression
```

## Comparing `honeybee-doe2-0.0.4.tar` & `honeybee-doe2-0.0.5.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-15 23:00:57.000000 honeybee-doe2-0.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/_extend_honeybee_doe2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/cli/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/geometry/polygon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/aperture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/constructions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/exposedfloor.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/groundcontact.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/hvac.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/compliance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/glass_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/run_period.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/sitebldg.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/materials.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/roof.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/story.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/properties/wall.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/utils/doe_formatters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/utils/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/utils/vector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/honeybee_doe2/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-15 23:02:14.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:02:14.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-15 23:02:14.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 23:02:14.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 23:02:14.000000 honeybee-doe2-0.0.4/honeybee_doe2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-15 23:02:15.000000 honeybee-doe2-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-15 23:00:58.000000 honeybee-doe2-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-16 02:05:06.000000 honeybee-doe2-0.0.5/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/_extend_honeybee_doe2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/cli/translate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/geometry/polygon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3871 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/constructions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/exposedfloor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/groundcontact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/hvac.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6982 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/glass_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1382 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/run_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/sitebldg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/materials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/roof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/story.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/properties/wall.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/doe_formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/utils/vector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/honeybee_doe2/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-16 02:06:31.000000 honeybee-doe2-0.0.5/honeybee_doe2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 02:06:32.000000 honeybee-doe2-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 02:05:07.000000 honeybee-doe2-0.0.5/setup.py
```

### Comparing `honeybee-doe2-0.0.4/LICENSE` & `honeybee-doe2-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/PKG-INFO` & `honeybee-doe2-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.0.4/README.md` & `honeybee-doe2-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/_extend_honeybee_doe2.py` & `honeybee-doe2-0.0.5/honeybee_doe2/_extend_honeybee_doe2.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/cli/translate.py` & `honeybee-doe2-0.0.5/honeybee_doe2/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/geometry/polygon.py` & `honeybee-doe2-0.0.5/honeybee_doe2/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/aperture.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/constructions.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/constructions.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/exposedfloor.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/exposedfloor.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/face.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/face.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/groundcontact.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/groundcontact.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/hvac.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/hvac.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/blocks.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/blocks.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/compliance.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/compliance.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/glass_types.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/glass_types.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/run_period.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/run_period.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/inputils/sitebldg.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/inputils/sitebldg.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/materials.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/materials.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/model.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/model.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/roof.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/roof.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/room.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/room.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/story.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/story.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/properties/wall.py` & `honeybee-doe2-0.0.5/honeybee_doe2/properties/wall.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/utils/doe_formatters.py` & `honeybee-doe2-0.0.5/honeybee_doe2/utils/doe_formatters.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/utils/geometry.py` & `honeybee-doe2-0.0.5/honeybee_doe2/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2/writer.py` & `honeybee-doe2-0.0.5/honeybee_doe2/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2.egg-info/PKG-INFO` & `honeybee-doe2-0.0.5/honeybee_doe2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-doe2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Honeybee extension for translating HBJSON files to INP files for eQuest
 Home-page: https://github.com/ladybug-tools/honeybee-doe2
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `honeybee-doe2-0.0.4/honeybee_doe2.egg-info/SOURCES.txt` & `honeybee-doe2-0.0.5/honeybee_doe2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-doe2-0.0.4/setup.py` & `honeybee-doe2-0.0.5/setup.py`

 * *Files identical despite different names*

