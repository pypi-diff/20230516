# Comparing `tmp/honeybee-grasshopper-core-1.9.0.tar.gz` & `tmp/honeybee-grasshopper-core-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-grasshopper-core-1.9.0.tar", last modified: Sun Jun  7 19:29:41 2020, max compression
+gzip compressed data, was "dist/honeybee-grasshopper-core-1.9.1.tar", last modified: Sun Jul 19 02:05:18 2020, max compression
```

## Comparing `honeybee-grasshopper-core-1.9.0.tar` & `honeybee-grasshopper-core-1.9.1.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/.gitignore
--rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/.releaserc.json
--rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/.travis.yml
--rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/CONTRIBUTING.md
--rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/deploy.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)      331 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/dev-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/
--rw-rw-r--   0 travis    (2000) travis    (2000)      347 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Prefix.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Shade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Subface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4455 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Aperture.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7216 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Apertures by Ratio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3880 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Color Face Attributes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3107 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Color Room Attributes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4792 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2409 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Deconstruct Model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4283 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Deconstruct Object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4371 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Door.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3553 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Dump Objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5096 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Extruded Border Shades.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Facade Parameters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Face.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2760 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by Attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3513 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by BC.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5156 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by Type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Intersect Solids.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6490 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Label Faces.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4174 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Label Rooms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3902 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Load Objects.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8633 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Louver Shades.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Mirror.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Model.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Move.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Object to String.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Planarize Brep.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7545 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Room from Solid.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6911 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Room.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2375 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Attribute.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2102 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Floor Height.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2989 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Orientation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4068 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rotate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3434 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Scale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Set Multiplier.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1662 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Set Story.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4661 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Shade.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3649 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Skylights by Ratio.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10103 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Solve Adjacency.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB String to Object.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7852 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Visualize by Type.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4156 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize All.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize Quick.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3877 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize Wireframe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize by BC.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4489 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Prefix.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4456 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Shade.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4747 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Subface.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4617 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Aperture.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6900 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Apertures by Ratio.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4536 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Color Face Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4836 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Color Room Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5187 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Config.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4601 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Deconstruct Model.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6157 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Deconstruct Object.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Door.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5375 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Dump Objects.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5437 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Extruded Border Shades.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5162 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Facade Parameters.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Face Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4973 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Face.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5123 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by Attribute.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5202 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by BC.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by Type.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4991 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Intersect Solids.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5769 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Label Faces.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Label Rooms.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5014 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Load Objects.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6627 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Louver Shades.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4790 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Mirror.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5668 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Model.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Move.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4013 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Object to String.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Planarize Brep.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room Attributes.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6516 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room from Solid.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6246 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4899 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Attribute.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4508 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Floor Height.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5790 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Orientation.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5230 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rotate.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5818 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Scale.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4664 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Set Multiplier.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3714 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Set Story.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4148 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Shade.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Skylights by Ratio.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6926 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Solve Adjacency.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB String to Object.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     6059 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Visualize by Type.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize All.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     4269 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize Quick.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     3692 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize Wireframe.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)     5421 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize by BC.ghuser
--rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5879 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/pass_tests.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/samples/
--rw-rw-r--   0 travis    (2000) travis    (2000)   489560 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/samples/model_creation_workflows.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)    54451 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/samples/model_serialization.gh
--rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-06-07 19:29:41.000000 honeybee-grasshopper-core-1.9.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-06-07 19:29:00.000000 honeybee-grasshopper-core-1.9.0/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      142 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/.gitignore
+-rw-rw-r--   0 travis    (2000) travis    (2000)      294 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/.releaserc.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)      574 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/.travis.yml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      279 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      445 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/CONTRIBUTING.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35149 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/LICENSE
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1782 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      165 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/deploy.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      332 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/dev-requirements.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      347 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2204 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Prefix.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1839 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Shade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2457 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Subface.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4455 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Aperture.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7216 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Apertures by Ratio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3880 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Color Face Attributes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3107 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Color Room Attributes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4792 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2409 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Deconstruct Model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4283 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Deconstruct Object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4371 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Door.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3553 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Dump Objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5096 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Extruded Border Shades.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1660 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Facade Parameters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5354 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Face.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2760 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by Attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3513 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by BC.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5156 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by Type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2572 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Intersect Solids.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6490 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Label Faces.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4174 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Label Rooms.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3902 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Load Objects.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8633 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Louver Shades.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2529 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Mirror.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2840 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Model.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2544 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Move.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1568 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Object to String.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2169 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Planarize Brep.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7545 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Room from Solid.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6911 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Room.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2375 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Attribute.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2102 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Floor Height.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2989 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Orientation.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4068 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rotate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3434 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Scale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2339 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Set Multiplier.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1662 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Set Story.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4661 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Shade.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3649 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Skylights by Ratio.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10103 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Solve Adjacency.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1989 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB String to Object.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7852 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Visualize by Type.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4156 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize All.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2410 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize Quick.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3877 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize Wireframe.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4340 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize by BC.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       55 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4489 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Prefix.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4456 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Shade.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4747 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Subface.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4617 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Aperture.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6900 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Apertures by Ratio.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4536 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Color Face Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4836 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Color Room Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5187 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Config.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4601 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Deconstruct Model.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6157 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Deconstruct Object.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4364 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Door.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5375 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Dump Objects.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5437 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Extruded Border Shades.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5162 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Facade Parameters.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2402 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Face Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4973 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Face.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5123 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by Attribute.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5202 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by BC.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5903 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by Type.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4991 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Intersect Solids.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5769 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Label Faces.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5235 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Label Rooms.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5014 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Load Objects.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6627 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Louver Shades.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4790 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Mirror.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5668 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Model.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4547 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Move.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4013 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Object to String.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4861 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Planarize Brep.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2951 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room Attributes.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6516 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room from Solid.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6246 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4899 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Attribute.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4508 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Floor Height.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5790 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Orientation.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5230 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rotate.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5839 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Scale.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4664 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Set Multiplier.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3714 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Set Story.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4148 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Shade.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5865 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Skylights by Ratio.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6926 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Solve Adjacency.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3997 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB String to Object.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6059 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Visualize by Type.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5188 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize All.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4269 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize Quick.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3692 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize Wireframe.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5421 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize by BC.ghuser
+-rw-rw-r--   0 travis    (2000) travis    (2000)       46 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2657 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5879 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       26 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       48 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/pass_tests.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/samples/
+-rw-rw-r--   0 travis    (2000) travis    (2000)   490141 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/samples/model_creation_workflows.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)    54462 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/samples/model_serialization.gh
+-rw-rw-r--   0 travis    (2000) travis    (2000)      102 2020-07-19 02:05:18.000000 honeybee-grasshopper-core-1.9.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-07-19 02:04:35.000000 honeybee-grasshopper-core-1.9.1/setup.py
```

### Comparing `honeybee-grasshopper-core-1.9.0/.travis.yml` & `honeybee-grasshopper-core-1.9.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/LICENSE` & `honeybee-grasshopper-core-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/PKG-INFO` & `honeybee-grasshopper-core-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-core
-Version: 1.9.0
+Version: 1.9.1
 Summary: Core Honeybee plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-core
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-core.svg?branch=master)](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-core)
```

### Comparing `honeybee-grasshopper-core-1.9.0/README.md` & `honeybee-grasshopper-core-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Prefix.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Prefix.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Shade.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Add Subface.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Add Subface.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Aperture.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Aperture.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Apertures by Ratio.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Apertures by Ratio.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Color Face Attributes.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Color Face Attributes.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Color Room Attributes.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Color Room Attributes.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Config.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Config.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Deconstruct Model.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Deconstruct Model.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Deconstruct Object.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Deconstruct Object.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Door.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Door.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Dump Objects.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Dump Objects.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Extruded Border Shades.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Extruded Border Shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Facade Parameters.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Facade Parameters.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Face.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Face.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by Attribute.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by Attribute.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by BC.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by BC.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Faces by Type.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Faces by Type.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Intersect Solids.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Intersect Solids.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Label Faces.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Label Faces.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Label Rooms.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Label Rooms.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Load Objects.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Load Objects.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Louver Shades.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Louver Shades.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Mirror.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Mirror.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Model.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Model.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Move.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Move.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Object to String.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Object to String.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Planarize Brep.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Planarize Brep.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Room from Solid.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Room from Solid.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Room.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Room.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Attribute.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Attribute.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Floor Height.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Floor Height.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rooms by Orientation.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rooms by Orientation.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Rotate.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Rotate.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Scale.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Scale.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     
     Returns:
         hb_objs: The input _hb_objs that has been scaled by the input factor.
 """
 
 ghenv.Component.Name = "HB Scale"
 ghenv.Component.NickName = 'Scale'
-ghenv.Component.Message = '0.1.3'
+ghenv.Component.Message = '0.1.4'
 ghenv.Component.Category = 'Honeybee'
 ghenv.Component.SubCategory = '0 :: Create'
 ghenv.Component.AdditionalHelpFromDocStrings = "6"
 
 try:  # import the honeybee core dependencies
     from honeybee.model import Model
 except ImportError as e:
```

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Set Multiplier.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Set Multiplier.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Set Story.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Set Story.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Shade.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Skylights by Ratio.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Skylights by Ratio.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Solve Adjacency.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Solve Adjacency.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB String to Object.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB String to Object.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Visualize by Type.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Visualize by Type.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize All.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize All.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize Quick.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize Quick.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize Wireframe.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize Wireframe.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/src/HB Vizualize by BC.py` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/src/HB Vizualize by BC.py`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Prefix.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Prefix.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Shade.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Shade.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Add Subface.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Add Subface.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Aperture.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Aperture.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Apertures by Ratio.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Apertures by Ratio.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Color Face Attributes.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Color Face Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Color Room Attributes.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Color Room Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Config.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Config.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Deconstruct Model.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Deconstruct Model.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Deconstruct Object.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Deconstruct Object.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Door.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Door.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Dump Objects.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Dump Objects.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Extruded Border Shades.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Extruded Border Shades.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Facade Parameters.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Facade Parameters.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Face Attributes.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Face Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Face.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Face.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by Attribute.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by Attribute.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by BC.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by BC.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Faces by Type.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Faces by Type.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Intersect Solids.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Intersect Solids.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Label Faces.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Label Faces.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Label Rooms.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Label Rooms.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Load Objects.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Load Objects.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Louver Shades.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Louver Shades.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Mirror.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Mirror.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Model.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Model.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Move.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Move.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Object to String.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Object to String.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Planarize Brep.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Planarize Brep.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room Attributes.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room Attributes.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room from Solid.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room from Solid.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Room.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Room.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Attribute.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Attribute.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Floor Height.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Floor Height.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rooms by Orientation.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rooms by Orientation.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Rotate.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Rotate.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Set Multiplier.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Set Multiplier.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Set Story.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Set Story.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Shade.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Shade.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Skylights by Ratio.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Skylights by Ratio.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Solve Adjacency.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Solve Adjacency.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB String to Object.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB String to Object.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Visualize by Type.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Visualize by Type.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize All.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize All.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize Quick.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize Quick.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize Wireframe.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize Wireframe.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core/user_objects/HB Vizualize by BC.ghuser` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core/user_objects/HB Vizualize by BC.ghuser`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/PKG-INFO` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-grasshopper-core
-Version: 1.9.0
+Version: 1.9.1
 Summary: Core Honeybee plugin for Grasshopper.
 Home-page: https://github.com/ladybug-tools/honeybee-grasshopper-core
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: UNKNOWN
 Description: [![Build Status](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-core.svg?branch=master)](https://travis-ci.org/ladybug-tools/honeybee-grasshopper-core)
```

### Comparing `honeybee-grasshopper-core-1.9.0/honeybee_grasshopper_core.egg-info/SOURCES.txt` & `honeybee-grasshopper-core-1.9.1/honeybee_grasshopper_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-grasshopper-core-1.9.0/setup.py` & `honeybee-grasshopper-core-1.9.1/setup.py`

 * *Files identical despite different names*

