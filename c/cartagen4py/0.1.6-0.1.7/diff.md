# Comparing `tmp/cartagen4py-0.1.6.tar.gz` & `tmp/cartagen4py-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cartagen4py-0.1.6.tar", last modified: Mon May 15 09:06:42 2023, max compression
+gzip compressed data, was "cartagen4py-0.1.7.tar", last modified: Mon May 15 13:43:38 2023, max compression
```

## Comparing `cartagen4py-0.1.6.tar` & `cartagen4py-0.1.7.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/README.md
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.6/cartagen4py/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.6/cartagen4py/algorithms/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/amalgamation.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/random_displacement.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14748 2023-05-15 08:35:50.000000 cartagen4py-0.1.6/cartagen4py/algorithms/buildings/squaring.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/general/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.6/cartagen4py/algorithms/general/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.6/cartagen4py/algorithms/general/constraint.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/algorithms/lines/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5310 2023-05-12 11:58:09.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_simplification.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_smoothing.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py/data_enrichment/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      113 2023-05-12 12:24:09.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/building_measures.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.6/cartagen4py/data_enrichment/urban_areas.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/evaluation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/evaluation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/evaluation/constraint_satisfaction.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/processes/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.6/cartagen4py/processes/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.6/cartagen4py/utils/__init__.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/clustering/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.6/cartagen4py/utils/clustering/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.6/cartagen4py/utils/clustering/dbscan.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/geometry/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/angle.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/extent.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/line.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.6/cartagen4py/utils/geometry/segment.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/math/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.6/cartagen4py/utils/math/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.6/cartagen4py/utils/math/morphology.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.6/cartagen4py/utils/math/vector.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/partitioning/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/network.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      334 2023-05-15 09:06:20.000000 cartagen4py-0.1.6/cartagen4py/utils/partitioning/quadtree.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/cartagen4py/utils/tessellation/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       59 2023-05-15 08:50:31.000000 cartagen4py-0.1.6/cartagen4py/utils/tessellation/__init__.py
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3747 2023-03-15 09:37:20.000000 cartagen4py-0.1.6/cartagen4py/utils/tessellation/hexagonal_tess.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.816951 cartagen4py-0.1.6/cartagen4py.egg-info/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/PKG-INFO
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1617 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/SOURCES.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/dependency_links.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/requires.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-15 09:06:42.000000 cartagen4py-0.1.6/cartagen4py.egg-info/top_level.txt
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/setup.cfg
--rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-15 09:06:40.000000 cartagen4py-0.1.6/setup.py
-drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 09:06:42.820951 cartagen4py-0.1.6/test/
--rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 08:55:39.000000 cartagen4py-0.1.6/test/test-imports.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      229 2023-03-01 13:47:49.000000 cartagen4py-0.1.7/README.md
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.991925 cartagen4py-0.1.7/cartagen4py/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      179 2023-05-15 08:33:30.000000 cartagen4py-0.1.7/cartagen4py/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.991925 cartagen4py-0.1.7/cartagen4py/algorithms/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      134 2023-05-15 08:34:07.000000 cartagen4py-0.1.7/cartagen4py/algorithms/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      244 2023-05-15 08:34:43.000000 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4482 2023-05-15 08:35:40.000000 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/amalgamation.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     7441 2023-05-15 08:35:18.000000 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/random_displacement.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     8000 2023-05-15 08:35:47.000000 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    14966 2023-05-15 13:42:57.000000 cartagen4py-0.1.7/cartagen4py/algorithms/buildings/squaring.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/algorithms/general/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       55 2023-05-12 12:21:40.000000 cartagen4py-0.1.7/cartagen4py/algorithms/general/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)    27075 2023-05-12 11:58:26.000000 cartagen4py-0.1.7/cartagen4py/algorithms/general/constraint.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/algorithms/lines/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      120 2023-05-12 12:23:23.000000 cartagen4py-0.1.7/cartagen4py/algorithms/lines/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     5310 2023-05-12 11:58:09.000000 cartagen4py-0.1.7/cartagen4py/algorithms/lines/line_simplification.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      394 2023-03-15 09:37:20.000000 cartagen4py-0.1.7/cartagen4py/algorithms/lines/line_smoothing.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/data_enrichment/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      113 2023-05-12 12:24:09.000000 cartagen4py-0.1.7/cartagen4py/data_enrichment/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1570 2023-05-12 12:24:49.000000 cartagen4py-0.1.7/cartagen4py/data_enrichment/building_measures.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1018 2023-05-12 11:58:54.000000 cartagen4py-0.1.7/cartagen4py/data_enrichment/urban_areas.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/evaluation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.7/cartagen4py/evaluation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      238 2023-03-01 13:47:49.000000 cartagen4py-0.1.7/cartagen4py/evaluation/constraint_satisfaction.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/processes/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-01 13:47:49.000000 cartagen4py-0.1.7/cartagen4py/processes/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/utils/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      210 2023-05-15 08:50:08.000000 cartagen4py-0.1.7/cartagen4py/utils/__init__.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/utils/clustering/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       49 2023-05-15 08:52:08.000000 cartagen4py-0.1.7/cartagen4py/utils/clustering/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        0 2023-03-30 13:41:05.000000 cartagen4py-0.1.7/cartagen4py/utils/clustering/dbscan.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.995925 cartagen4py-0.1.7/cartagen4py/utils/geometry/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      189 2023-05-15 08:51:46.000000 cartagen4py-0.1.7/cartagen4py/utils/geometry/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      386 2023-03-15 09:37:20.000000 cartagen4py-0.1.7/cartagen4py/utils/geometry/angle.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1327 2023-03-21 13:10:50.000000 cartagen4py-0.1.7/cartagen4py/utils/geometry/extent.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1195 2023-03-30 13:41:05.000000 cartagen4py-0.1.7/cartagen4py/utils/geometry/line.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3167 2023-05-12 11:54:30.000000 cartagen4py-0.1.7/cartagen4py/utils/geometry/segment.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/cartagen4py/utils/math/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       91 2023-05-15 08:51:15.000000 cartagen4py-0.1.7/cartagen4py/utils/math/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     4304 2023-04-21 08:51:00.000000 cartagen4py-0.1.7/cartagen4py/utils/math/morphology.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      474 2023-05-12 11:28:23.000000 cartagen4py-0.1.7/cartagen4py/utils/math/vector.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/cartagen4py/utils/partitioning/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      106 2023-05-15 08:50:53.000000 cartagen4py-0.1.7/cartagen4py/utils/partitioning/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     2183 2023-05-12 11:55:23.000000 cartagen4py-0.1.7/cartagen4py/utils/partitioning/network.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      334 2023-05-15 09:06:20.000000 cartagen4py-0.1.7/cartagen4py/utils/partitioning/quadtree.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/cartagen4py/utils/tessellation/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       59 2023-05-15 08:50:31.000000 cartagen4py-0.1.7/cartagen4py/utils/tessellation/__init__.py
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     3747 2023-03-15 09:37:20.000000 cartagen4py-0.1.7/cartagen4py/utils/tessellation/hexagonal_tess.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.991925 cartagen4py-0.1.7/cartagen4py.egg-info/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)      794 2023-05-15 13:43:37.000000 cartagen4py-0.1.7/cartagen4py.egg-info/PKG-INFO
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)     1617 2023-05-15 13:43:37.000000 cartagen4py-0.1.7/cartagen4py.egg-info/SOURCES.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)        1 2023-05-15 13:43:37.000000 cartagen4py-0.1.7/cartagen4py.egg-info/dependency_links.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       24 2023-05-15 13:43:37.000000 cartagen4py-0.1.7/cartagen4py.egg-info/requires.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       12 2023-05-15 13:43:37.000000 cartagen4py-0.1.7/cartagen4py.egg-info/top_level.txt
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       38 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/setup.cfg
+-rwxr-xr-x   0 justinberli  (1000) justinberli  (1000)     2053 2023-05-15 13:43:35.000000 cartagen4py-0.1.7/setup.py
+drwxr-xr-x   0 justinberli  (1000) justinberli  (1000)        0 2023-05-15 13:43:37.999925 cartagen4py-0.1.7/test/
+-rw-r--r--   0 justinberli  (1000) justinberli  (1000)       19 2023-05-15 10:51:15.000000 cartagen4py-0.1.7/test/test-imports.py
```

### Comparing `cartagen4py-0.1.6/PKG-INFO` & `cartagen4py-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/amalgamation.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/buildings/amalgamation.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/random_displacement.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/buildings/random_displacement.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/simplification.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/buildings/simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/buildings/squaring.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/buildings/squaring.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # This is an implementation of the least squares based squaring algorithm proposed by Lokhat & Touya (https://hal.science/hal-02147792)
 import numpy as np
 
 class Squarer:
     """Initialize squaring object, with default weights and tolerance set in the constructor
     """
-    def __init__(self, max_iter=1000, norm_tol=0.05,rtol=10, ftol=0.11, hrtol=7, pfixe=5, p90=100, p0=50, p45=10, switch_new=False):
+    def __init__(
+            self, max_iteration=1000, norm_tolerance=0.05,
+            right_tolerance=10, flat_tolerance=10, half_right_tolerance=7,
+            fixed_weight=5, right_weight=100, flat_weight=50, half_right_weight=10, switch_new=False
+        ):
+
         self.SWITCH_NEW = switch_new
-        self.MAX_ITER = max_iter
-        self.NORM_DIFF_TOL = norm_tol
-        self.rightTol = rtol # 10 90° angles tolerance
-        self.flatTol = ftol # 0.11 flat angles tolerance
-        self.semiRightTol = hrtol # 7 45/135° angles tolerance
-        self.poidsPtfFixe = pfixe #5
-        self.poids90 = p90 #100
-        self.poids0 = p0 #50
-        self.poids45 = p45 #10
+        self.MAX_ITERATION = max_iteration
+        self.NORM_TOLERANCE = norm_tolerance
+        self.right_tolerance = right_tolerance # 10 90° angles tolerance
+        self.flat_tolerance = flat_tolerance # 0.11 flat angles tolerance
+        self.half_right_tolerance = half_right_tolerance # 7 45/135° angles tolerance
+        self.fixed_weight = fixed_weight #5
+        self.right_weight = right_weight #100
+        self.flat_weight = flat_weight #50
+        self.half_right_weight = half_right_weight #10
 
         self.point_shapes = {}
         self.__lines_pindex = []
         self.indicesRight, self.indicesFlat, self.indicesHrAig, self.indicesHrObt = [], [], [], []
 
     # returns a list of coordinates from a shapely linestring, multilinestring or polygon 
     def __get_coords(self, shape):
@@ -107,29 +112,30 @@
         else:
             v1 = np.array([p[0] - pr[0], p[1] - pr[1]])
         v2 = np.array([s[0] - p[0], s[1] - p[1]])
         return v1, v2
 
     def __idx_angles_remarquables(self, unik_points):
         #unik_points = list(self.point_shapes)
-        rTol = np.cos((np.pi / 2) - self.rightTol * np.pi / 180)
-        hrTol1 = np.cos((np.pi / 4) - self.semiRightTol * np.pi / 180)
-        hrTol2 = np.cos((np.pi / 4) + self.semiRightTol * np.pi / 180)
+        rTol = np.cos((np.pi / 2) - self.right_tolerance * np.pi / 180)
+        fTol = np.deg2rad(self.flat_tolerance)
+        hrTol1 = np.cos((np.pi / 4) - self.half_right_tolerance * np.pi / 180)
+        hrTol2 = np.cos((np.pi / 4) + self.half_right_tolerance * np.pi / 180)
         for idx_p in range(len(unik_points)):
             triplets = self.__get_angle_triplets(idx_p, unik_points)
             for t in triplets:
                 v1, v2 = self.__get_vecs_around(t, unik_points)
                 n1, n2 = np.linalg.norm(v1), np.linalg.norm(v2)
                 v1n = v1 / n1 if n1 != 0. else np.array([0.,0.]) #n1
                 v2n = v2 / n2 if n2 != 0. else np.array([0.,0.]) #n2
                 dot = v1n.dot(v2n)
                 cross = np.cross(v1n, v2n).item(0)
                 if (np.abs(dot) <= rTol):
                     self.indicesRight.append(t)
-                elif (cross <= self.flatTol):
+                elif (cross <= fTol):
                     self.indicesFlat.append(t)
                 #elif (dot <= hrTol1 and dot >= hrTol2):
                 #    self.indicesHrAig.append(t)
                 #elif (dot >= -hrTol1 and dot <= -hrTol2):
                 #    self.indicesHrObt.append(t)
         print(f'potential angles -- R: {len(self.indicesRight)} - F: {len(self.indicesFlat)}')
         #print(f'potential angles -- R: {len(self.indicesRight)} - F: {len(self.indicesFlat)} - HRa: {len(self.indicesHrAig)} - HRo: {len(self.indicesHrObt)}')
@@ -163,25 +169,19 @@
         for i, p in enumerate(points):
             S[2*i] = p[0]
             S[2*i+1] = p[1]
         offset = 2 * nb_points
         for i, t in enumerate(self.indicesRight):
             v1, v2 = self.__get_vecs_around(t, points)
             d = v1.dot(v2)
-            # print(v1)
-            # print(v2)
-            # print(d)
             S[offset + i] = d
         offset = 2 * nb_points + len(self.indicesRight)
         for i, t in enumerate(self.indicesFlat):
             v1, v2 = self.__get_vecs_around(t, points)
             d = np.cross(v1, v2).item(0)
-            print(v1)
-            print(v2)
-            print(d)
             S[offset + i] = d
         offset = 2 * nb_points + len(self.indicesRight) + len(self.indicesFlat)
         #for i, t in enumerate(self.indicesHrAig):
         #    v1, v2 = self.__get_vecs_around(t, points)
         #    d = v1.dot(v2) 
         #    S[offset + i] = d
         #offset = 2 * nb_points + len(self.indicesRight) + len(self.indicesFlat) + len(self.indicesHrAig)
@@ -193,18 +193,18 @@
 
     # Weight Matrix
     # n = 2 * nb_points + indicesRight.size() + indicesFlat.size() + indicesHrAig.size() + indicesHrObt.size()
     def __get_P(self):
         nb_points = len(self.point_shapes)
         nb_rights, nb_flats =  len(self.indicesRight), len(self.indicesFlat)
         #nb_half_rights = len(self.indicesHrAig) + len(self.indicesHrObt)
-        wfix = np.full(2*nb_points, self.poidsPtfFixe)
-        wRight = np.full(nb_rights, self.poids90)
-        wFlat = np.full(nb_flats, self.poids0)
-        #wHr = np.full(nb_half_rights, self.poids45)
+        wfix = np.full(2*nb_points, self.fixed_weight)
+        wRight = np.full(nb_rights, self.right_weight)
+        wFlat = np.full(nb_flats, self.flat_weight)
+        #wHr = np.full(nb_half_rights, self.half_right_weight)
         self.P = np.diag(np.concatenate((wfix, wRight, wFlat)))
 
     ## new vectors
     def __partial_derivatives_dotp(self, points, indices):
         nb_points = len(points)
         nb_indices = len(indices)
         m = np.zeros((nb_indices, 2*nb_points))
@@ -294,19 +294,19 @@
     
     def square(self, shapes):
         """squares a collection of shapely multilinestrings or polygons
         returns a numpy array of the points after the least square process
         """
         points = self.__prepare_square(shapes)
         nb_points = len(points)
-        for i in range(self.MAX_ITER):
+        for i in range(self.MAX_ITERATION):
             dx = self.__compute_dx(points)
             points += dx.reshape((nb_points, 2))
             print(i, np.linalg.norm(dx, ord=np.inf))
-            if np.linalg.norm(dx, ord=np.inf) < self.NORM_DIFF_TOL:
+            if np.linalg.norm(dx, ord=np.inf) < self.NORM_TOLERANCE:
                 break
         self.nb_iters = i
         return points
 
 
     # rebuild shapes with updated points from least square process
     def get_shapes_from_new_points(self, original_shapes, new_points):
```

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/general/constraint.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/general/constraint.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/algorithms/lines/line_simplification.py` & `cartagen4py-0.1.7/cartagen4py/algorithms/lines/line_simplification.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/data_enrichment/building_measures.py` & `cartagen4py-0.1.7/cartagen4py/data_enrichment/building_measures.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/data_enrichment/urban_areas.py` & `cartagen4py-0.1.7/cartagen4py/data_enrichment/urban_areas.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/geometry/extent.py` & `cartagen4py-0.1.7/cartagen4py/utils/geometry/extent.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/geometry/line.py` & `cartagen4py-0.1.7/cartagen4py/utils/geometry/line.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/geometry/segment.py` & `cartagen4py-0.1.7/cartagen4py/utils/geometry/segment.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/math/morphology.py` & `cartagen4py-0.1.7/cartagen4py/utils/math/morphology.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/partitioning/network.py` & `cartagen4py-0.1.7/cartagen4py/utils/partitioning/network.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py/utils/tessellation/hexagonal_tess.py` & `cartagen4py-0.1.7/cartagen4py/utils/tessellation/hexagonal_tess.py`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/cartagen4py.egg-info/PKG-INFO` & `cartagen4py-0.1.7/cartagen4py.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cartagen4py
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python package to generalise geographic objects for cartographic purposes
 Home-page: https://github.com/LostInZoom/cartagen4py
 Author: Guillaume Touya, Justin Berli
 Author-email: guillaume.touya@ign.fr
 License: CeCILL-C
 Keywords: Generalization,Cartography,cartographic generalization
 Platform: Linux
```

### Comparing `cartagen4py-0.1.6/cartagen4py.egg-info/SOURCES.txt` & `cartagen4py-0.1.7/cartagen4py.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cartagen4py-0.1.6/setup.py` & `cartagen4py-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if sys.version_info[:2] < (3, 8):
     error = ('cartagen4py requires Python 3.8 or later (%d.%d detected).' % sys.version_info[:2])
     sys.stderr.write(error + "\n")
     sys.exit(1)
 
 # General informations
 name = 'cartagen4py'
-version = '0.1.6'
+version = '0.1.7'
 description = 'Python package to generalise geographic objects for cartographic purposes'
 url = 'https://github.com/LostInZoom/cartagen4py'
 author = 'Guillaume Touya, Justin Berli'
 author_email = 'guillaume.touya@ign.fr'
 lic = 'CeCILL-C'
 packages = [
     'cartagen4py',
```

