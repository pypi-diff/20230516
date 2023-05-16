# Comparing `tmp/cartagen4py-0.1.8.tar.gz` & `tmp/cartagen4py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartagen4py-0.1.8.tar", last modified: Tue May 16 09:01:45 2023, max compression
+gzip compressed data, was "cartagen4py-0.1.9.tar", last modified: Tue May 16 13:33:58 2023, max compression
```

## Comparing `cartagen4py-0.1.8.tar` & `cartagen4py-0.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      363 2023-05-15 15:01:36.000000 cartagen4py-0.1.8/README.md
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.209889 cartagen4py-0.1.8/cartagen4py/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.8/cartagen4py/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.209889 cartagen4py-0.1.8/cartagen4py/algorithms/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.8/cartagen4py/algorithms/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/amalgamation.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/random_displacement.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14964 2023-05-15 13:52:25.000000 cartagen4py-0.1.8/cartagen4py/algorithms/buildings/squaring.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/algorithms/general/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.8/cartagen4py/algorithms/general/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.8/cartagen4py/algorithms/general/constraint.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/algorithms/lines/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.8/cartagen4py/algorithms/lines/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5305 2023-05-16 08:51:34.000000 cartagen4py-0.1.8/cartagen4py/algorithms/lines/line_simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.8/cartagen4py/algorithms/lines/line_smoothing.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/data_enrichment/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      162 2023-05-16 08:50:46.000000 cartagen4py-0.1.8/cartagen4py/data_enrichment/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.8/cartagen4py/data_enrichment/building_measures.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    13039 2023-05-16 08:57:11.000000 cartagen4py-0.1.8/cartagen4py/data_enrichment/stroke.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.8/cartagen4py/data_enrichment/urban_areas.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/evaluation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.8/cartagen4py/evaluation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.8/cartagen4py/evaluation/constraint_satisfaction.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/processes/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.8/cartagen4py/processes/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/utils/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.8/cartagen4py/utils/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/utils/clustering/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.8/cartagen4py/utils/clustering/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.8/cartagen4py/utils/clustering/dbscan.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.213889 cartagen4py-0.1.8/cartagen4py/utils/geometry/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.8/cartagen4py/utils/geometry/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.8/cartagen4py/utils/geometry/angle.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.8/cartagen4py/utils/geometry/extent.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.8/cartagen4py/utils/geometry/line.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.8/cartagen4py/utils/geometry/segment.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/cartagen4py/utils/math/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.8/cartagen4py/utils/math/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.8/cartagen4py/utils/math/morphology.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.8/cartagen4py/utils/math/vector.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/cartagen4py/utils/partitioning/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.8/cartagen4py/utils/partitioning/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.8/cartagen4py/utils/partitioning/network.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      334 2023-05-15 09:06:20.000000 cartagen4py-0.1.8/cartagen4py/utils/partitioning/quadtree.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/cartagen4py/utils/tessellation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       54 2023-05-16 08:51:12.000000 cartagen4py-0.1.8/cartagen4py/utils/tessellation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3721 2023-05-16 07:42:19.000000 cartagen4py-0.1.8/cartagen4py/utils/tessellation/hexagonal.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.209889 cartagen4py-0.1.8/cartagen4py.egg-info/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-16 09:01:45.000000 cartagen4py-0.1.8/cartagen4py.egg-info/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1650 2023-05-16 09:01:45.000000 cartagen4py-0.1.8/cartagen4py.egg-info/SOURCES.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-16 09:01:45.000000 cartagen4py-0.1.8/cartagen4py.egg-info/dependency_links.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-16 09:01:45.000000 cartagen4py-0.1.8/cartagen4py.egg-info/requires.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-16 09:01:45.000000 cartagen4py-0.1.8/cartagen4py.egg-info/top_level.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/setup.cfg
--rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-16 09:01:35.000000 cartagen4py-0.1.8/setup.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:01:45.217889 cartagen4py-0.1.8/test/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       19 2023-05-15 10:51:15.000000 cartagen4py-0.1.8/test/test-imports.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.447541 cartagen4py-0.1.9/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-16 13:33:58.447541 cartagen4py-0.1.9/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      363 2023-05-15 15:01:36.000000 cartagen4py-0.1.9/README.md
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      183 2023-05-16 13:17:20.000000 cartagen4py-0.1.9/cartagen4py/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py/algorithms/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.9/cartagen4py/algorithms/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-16 09:28:43.000000 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/amalgamation.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/random_displacement.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14964 2023-05-15 13:52:25.000000 cartagen4py-0.1.9/cartagen4py/algorithms/buildings/squaring.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py/algorithms/general/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.9/cartagen4py/algorithms/general/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.9/cartagen4py/algorithms/general/constraint.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py/algorithms/lines/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.9/cartagen4py/algorithms/lines/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5305 2023-05-16 08:51:34.000000 cartagen4py-0.1.9/cartagen4py/algorithms/lines/line_simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.9/cartagen4py/algorithms/lines/line_smoothing.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/data_enrichment/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      162 2023-05-16 08:50:46.000000 cartagen4py-0.1.9/cartagen4py/data_enrichment/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.9/cartagen4py/data_enrichment/building_measures.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    13202 2023-05-16 12:37:53.000000 cartagen4py-0.1.9/cartagen4py/data_enrichment/stroke.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.9/cartagen4py/data_enrichment/urban_areas.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/evaluation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.9/cartagen4py/evaluation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.9/cartagen4py/evaluation/constraint_satisfaction.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/processes/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.9/cartagen4py/processes/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.9/cartagen4py/utils/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/clustering/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.9/cartagen4py/utils/clustering/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.9/cartagen4py/utils/clustering/dbscan.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/geometry/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.9/cartagen4py/utils/geometry/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.9/cartagen4py/utils/geometry/angle.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.9/cartagen4py/utils/geometry/extent.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.9/cartagen4py/utils/geometry/line.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.9/cartagen4py/utils/geometry/segment.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/math/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.9/cartagen4py/utils/math/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.9/cartagen4py/utils/math/morphology.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.9/cartagen4py/utils/math/vector.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/partitioning/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.9/cartagen4py/utils/partitioning/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.9/cartagen4py/utils/partitioning/network.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      334 2023-05-15 09:06:20.000000 cartagen4py-0.1.9/cartagen4py/utils/partitioning/quadtree.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/cartagen4py/utils/tessellation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       54 2023-05-16 08:51:12.000000 cartagen4py-0.1.9/cartagen4py/utils/tessellation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3721 2023-05-16 07:42:19.000000 cartagen4py-0.1.9/cartagen4py/utils/tessellation/hexagonal.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.439541 cartagen4py-0.1.9/cartagen4py.egg-info/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-16 13:33:58.000000 cartagen4py-0.1.9/cartagen4py.egg-info/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1650 2023-05-16 13:33:58.000000 cartagen4py-0.1.9/cartagen4py.egg-info/SOURCES.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-16 13:33:58.000000 cartagen4py-0.1.9/cartagen4py.egg-info/dependency_links.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-16 13:33:58.000000 cartagen4py-0.1.9/cartagen4py.egg-info/requires.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-16 13:33:58.000000 cartagen4py-0.1.9/cartagen4py.egg-info/top_level.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-16 13:33:58.447541 cartagen4py-0.1.9/setup.cfg
+-rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-16 13:33:42.000000 cartagen4py-0.1.9/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 13:33:58.443541 cartagen4py-0.1.9/test/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-05-16 09:12:36.000000 cartagen4py-0.1.9/test/test-imports.py
```

### Comparing `cartagen4py-0.1.8/PKG-INFO` & `cartagen4py-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/buildings/amalgamation.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/buildings/amalgamation.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/buildings/random_displacement.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/buildings/random_displacement.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/buildings/simplification.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/buildings/simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/buildings/squaring.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/buildings/squaring.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/general/constraint.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/general/constraint.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/algorithms/lines/line_simplification.py` & `cartagen4py-0.1.9/cartagen4py/algorithms/lines/line_simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/data_enrichment/building_measures.py` & `cartagen4py-0.1.9/cartagen4py/data_enrichment/building_measures.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/data_enrichment/stroke.py` & `cartagen4py-0.1.9/cartagen4py/data_enrichment/stroke.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import math
 
 import numpy as np
 from shapely.geometry import LineString, Point, MultiLineString
-from shapely import  ops
+from shapely import ops
 import geopandas as gpd
 
 from cartagen4py.utils.geometry.angle import angle_3_pts
 
 class Stroke:
     COUNTER = 0
-    def __init__(self,network,root):
+    def __init__(self, network, root):
         self.network = network
         self.root=root
         self.features = []
         self.features.append(root)
         self.id = Stroke.COUNTER
         Stroke.COUNTER += 1
     
@@ -256,15 +256,14 @@
         liste=""
         for elem in self.features: 
             liste+=str(elem.id)
             liste+=","
         return liste
     
 class StrokeNetwork:
-    
     def __init__(self,features):
             #Initialisation from a list of shapely geometry with the correct attributes
           self.features = features
           self.groupedFeatures = []
           self.id = 0;
           self.strokes = []
           
@@ -292,36 +291,38 @@
                 stroke = Stroke(self, obj)
                 #// build the stroke on the initial side
                 stroke.one_side_stroke(0, attributeNames, deviatAngle, deviatSum);
                 #// build the stroke on the final side
                 stroke.one_side_stroke(-1, attributeNames, deviatAngle, deviatSum);
                 #// add the stroke to the strokes set
                 self.strokes.append(stroke);
-                
-    def save_strokes_shp(self,path):
-        #Save a shapefile of stroke eometry in the desired folder
-        stroke_list=self.strokes
-        array=[]
-        i=0
-        for stroke in stroke_list:
+    
+    def __reconstruct_strokes(self, strokes):
+        array = []
+        for i, stroke in enumerate(strokes):
             listline=[]
             section=""
-            j=0
-            for seg in stroke.features:
+            for j, seg in enumerate(stroke.features):
                 listline+=[seg]
-                j+=1
-                section+=str(seg.id)
-                if j<len(stroke.features):
-                    section+=","
-
+                section += str(seg.id)
+                if j < len(stroke.features):
+                    section += ","
             multi_line = MultiLineString(listline)
             merged_line = ops.linemerge(multi_line)
-            array+=[[i,merged_line,section]]
-            i+=1
+            array += [[i,merged_line,section]]
+        return array
+
+    def save_strokes_shp(self,path):
+        #Save a shapefile of stroke eometry in the desired folder
+        strokes_list = self.strokes
+        array = self.__reconstruct_strokes(strokes_list)
         gdf = gpd.GeoDataFrame(array,  columns = ['id', 'geom',"section"],crs="epsg:2154",geometry="geom")   
         gdf.to_file(path, driver='ESRI Shapefile')
 
+    def get_strokes(self):
+        return self.__reconstruct_strokes(self.strokes)
+
```

### Comparing `cartagen4py-0.1.8/cartagen4py/data_enrichment/urban_areas.py` & `cartagen4py-0.1.9/cartagen4py/data_enrichment/urban_areas.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/geometry/extent.py` & `cartagen4py-0.1.9/cartagen4py/utils/geometry/extent.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/geometry/line.py` & `cartagen4py-0.1.9/cartagen4py/utils/geometry/line.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/geometry/segment.py` & `cartagen4py-0.1.9/cartagen4py/utils/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/math/morphology.py` & `cartagen4py-0.1.9/cartagen4py/utils/math/morphology.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/partitioning/network.py` & `cartagen4py-0.1.9/cartagen4py/utils/partitioning/network.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py/utils/tessellation/hexagonal.py` & `cartagen4py-0.1.9/cartagen4py/utils/tessellation/hexagonal.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/cartagen4py.egg-info/PKG-INFO` & `cartagen4py-0.1.9/cartagen4py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.8/cartagen4py.egg-info/SOURCES.txt` & `cartagen4py-0.1.9/cartagen4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.8/setup.py` & `cartagen4py-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if sys.version_info[:2] < (3, 8):
     error = ('cartagen4py requires Python 3.8 or later (%d.%d detected).' % sys.version_info[:2])
     sys.stderr.write(error + "\n")
     sys.exit(1)
 
 # General informations
 name = 'cartagen4py'
-version = '0.1.8'
+version = '0.1.9'
 description = 'Python package to generalise geographic objects for cartographic purposes'
 url = 'https://github.com/LostInZoom/cartagen4py'
 author = 'Guillaume Touya, Justin Berli'
 author_email = 'guillaume.touya@ign.fr'
 lic = 'CeCILL-C'
 packages = [
     'cartagen4py',
```

