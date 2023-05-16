# Comparing `tmp/spatialpandas-0.4.7.tar.gz` & `tmp/spatialpandas-0.4.8a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/spatialpandas-0.4.7.tar", last modified: Wed Mar 22 15:00:10 2023, max compression
+gzip compressed data, was "spatialpandas-0.4.8a1.tar", last modified: Tue May 16 13:26:08 2023, max compression
```

## Comparing `spatialpandas-0.4.7.tar` & `spatialpandas-0.4.8a1.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/.version
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/_optional_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geodataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/bounds.py
--rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/measures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/basefixed.py
--rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/baselist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/multiline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/multipoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/multipolygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geometry/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/geoseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/io/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17931 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/io/parquet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/spatialindex/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/spatialindex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/spatialindex/hilbert_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/spatialindex/rtree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/_create_testdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_measures.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_orientation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/intersection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/intersection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/intersection/test_point_intersection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/test_cx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/geometry/test_to_geopandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/spatialindex/
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/spatialindex/test_hilbert_curve.py
--rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/spatialindex/test_rtree.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_dask_autoimport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata
--rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/serial_5.0.0.parq
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_data/serial_8.0.0.parq
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_fixedextensionarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_geodataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_listextensionarray.py
--rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/test_parquet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tests/tools/test_sjoin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas/tools/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/tools/sjoin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-03-22 14:37:20.000000 spatialpandas-0.4.7/spatialpandas/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-22 15:00:10.000000 spatialpandas-0.4.7/spatialpandas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7382 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.542909 spatialpandas-0.4.8a1/spatialpandas/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas/.version
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/_optional_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24478 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geodataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/bounds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17743 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28546 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7847 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/basefixed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10828 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/baselist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multiline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multipoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/multipolygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geometry/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/geoseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19063 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/spatialindex/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/spatialindex/rtree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1663 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/_create_testdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.550910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7545 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_measures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_orientation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9338 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/test_point_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_cx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_to_geopandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_hilbert_curve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7000 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_rtree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_dask_autoimport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4157 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.554910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata
+-rw-r--r--   0 runner    (1001) docker     (123)     3420 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet
+-rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_5.0.0.parq
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_8.0.0.parq
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_fixedextensionarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_geodataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_listextensionarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16268 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet_s3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tests/tools/test_sjoin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.558910 spatialpandas-0.4.8a1/spatialpandas/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/tools/sjoin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-16 13:18:14.000000 spatialpandas-0.4.8a1/spatialpandas/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 13:26:08.546910 spatialpandas-0.4.8a1/spatialpandas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-16 13:26:08.000000 spatialpandas-0.4.8a1/spatialpandas.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `spatialpandas-0.4.7/CHANGELOG.md` & `spatialpandas-0.4.8a1/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/LICENSE` & `spatialpandas-0.4.8a1/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/NOTICE` & `spatialpandas-0.4.8a1/NOTICE`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/PKG-INFO` & `spatialpandas-0.4.8a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: spatialpandas
-Version: 0.4.7
+Version: 0.4.8a1
 Summary: Pandas extension arrays for spatial/geometric operations
 Home-page: https://github.com/holoviz/spatialpandas
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: examples
 License-File: LICENSE
 
 <img src="https://github.com/holoviz/spatialpandas/raw/main/doc/_static/logo_horizontal.png" data-canonical-src="https://github.com/holoviz/spatialpandas/raw/main/doc/_static/logo_horizontal.png" width="380"/><br>
```

### Comparing `spatialpandas-0.4.7/README.md` & `spatialpandas-0.4.8a1/README.md`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/setup.py` & `spatialpandas-0.4.8a1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,17 +6,19 @@
     'tests': [
         'codecov',
         'flake8',
         'hilbertcurve',
         'geopandas',
         'hypothesis',
         'keyring',
+        'moto[s3,server]',
         'pytest-cov',
         'pytest',
         'rfc3986',
+        's3fs',
         'scipy',
         'shapely',
         'twine',
     ],
     'examples': [
         'datashader',
         'descartes',
@@ -46,26 +48,25 @@
     ),
     description='Pandas extension arrays for spatial/geometric operations',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/holoviz/spatialpandas',
     maintainer='HoloViz developers',
     maintainer_email='developers@holoviz.org',
-    python_requires='>=3.7',
+    python_requires='>=3.8',
     install_requires=install_requires,
     extras_require=extras_require,
     tests_require=extras_require['tests'],
     license='BSD-2-Clause',
     packages=find_namespace_packages(),
     include_package_data=True,
     classifiers=[
         "License :: OSI Approved :: BSD License",
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
```

### Comparing `spatialpandas-0.4.7/spatialpandas/__init__.py` & `spatialpandas-0.4.8a1/spatialpandas/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/dask.py` & `spatialpandas-0.4.8a1/spatialpandas/dask.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geodataframe.py` & `spatialpandas-0.4.8a1/spatialpandas/geodataframe.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/__init__.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/bounds.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/bounds.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/measures.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/measures.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/_algorithms/orientation.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/_algorithms/orientation.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/base.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/base.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/basefixed.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/basefixed.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/baselist.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/baselist.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/line.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/line.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/multiline.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multiline.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/multipoint.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multipoint.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/multipolygon.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/multipolygon.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/point.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/point.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/polygon.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/polygon.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geometry/ring.py` & `spatialpandas-0.4.8a1/spatialpandas/geometry/ring.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/geoseries.py` & `spatialpandas-0.4.8a1/spatialpandas/geoseries.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/io/parquet.py` & `spatialpandas-0.4.8a1/spatialpandas/io/parquet.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import json
-import pathlib
 from functools import reduce
 from glob import has_magic
 from numbers import Number
 from packaging.version import Version
+from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import fsspec
 import pandas as pd
 import pyarrow as pa
 from dask import delayed
 from dask.dataframe import from_delayed, from_pandas
 from dask.dataframe import read_parquet as dd_read_parquet
 from dask.dataframe import to_parquet as dd_to_parquet  # noqa
 from dask.utils import natural_sort_key
 from pandas.io.parquet import to_parquet as pd_to_parquet
-from pyarrow import parquet as pq
+from pyarrow.parquet import ParquetDataset, ParquetFile, read_metadata
 
 from .. import GeoDataFrame
 from ..dask import DaskGeoDataFrame
 from ..geometry import GeometryDtype
 from ..io.utils import (
     PathType,
     _maybe_prepend_protocol,
@@ -42,44 +42,45 @@
     engine_kwargs = engine_kwargs or {}
     filesystem = validate_coerce_filesystem(path, filesystem, storage_options)
     if not filesystem.exists(path):
         raise ValueError("Path not found: " + path)
 
     if filesystem.isdir(path):
         if LEGACY_PYARROW:
-            basic_kwargs = dict(filesystem=filesystem, validate_schema=False)
+            basic_kwargs = dict(validate_schema=False)
         else:
-            basic_kwargs = dict(filesystem=filesystem, use_legacy_dataset=False)
+            basic_kwargs = dict(use_legacy_dataset=False)
 
-        pqds = pq.ParquetDataset(
+        pqds = ParquetDataset(
             path,
+            filesystem=filesystem,
             **basic_kwargs,
             **engine_kwargs,
         )
 
         if LEGACY_PYARROW:
             common_metadata = pqds.common_metadata
             if common_metadata is None:
                 # Get metadata for first piece
                 piece = pqds.pieces[0]
                 metadata = piece.get_metadata().metadata
             else:
                 metadata = pqds.common_metadata.metadata
         else:
-            filename = pathlib.Path(pqds.files[0]).parent.joinpath("_common_metadata")
+            filename = "/".join([_get_parent_path(pqds.files[0]), "_common_metadata"])
             try:
-                common_metadata = pq.read_metadata(filename)
+                common_metadata = _read_metadata(filename, filesystem=filesystem)
             except FileNotFoundError:
                 # Common metadata doesn't exist, so get metadata for first piece instead
-                filename = pathlib.Path(pqds.files[0])
-                common_metadata = pq.read_metadata(filename)
+                filename = pqds.files[0]
+                common_metadata = _read_metadata(filename, filesystem=filesystem)
             metadata = common_metadata.metadata
     else:
         with filesystem.open(path) as f:
-            pf = pq.ParquetFile(f)
+            pf = ParquetFile(f)
         metadata = pf.metadata.metadata
 
     return json.loads(
         metadata.get(b'pandas', b'{}').decode('utf')
     )
 
 
@@ -124,21 +125,22 @@
     engine_kwargs: Optional[Dict[str, Any]] = None,
     **kwargs: Any,
 ) -> GeoDataFrame:
     engine_kwargs = engine_kwargs or {}
     filesystem = validate_coerce_filesystem(path, filesystem, storage_options)
 
     if LEGACY_PYARROW:
-        basic_kwargs = dict(filesystem=filesystem, validate_schema=False)
+        basic_kwargs = dict(validate_schema=False)
     else:
-        basic_kwargs = dict(filesystem=filesystem, use_legacy_dataset=False)
+        basic_kwargs = dict(use_legacy_dataset=False)
 
     # Load using pyarrow to handle parquet files and directories across filesystems
-    dataset = pq.ParquetDataset(
+    dataset = ParquetDataset(
         path,
+        filesystem=filesystem,
         **basic_kwargs,
         **engine_kwargs,
         **kwargs,
     )
 
     if LEGACY_PYARROW:
         metadata = _load_parquet_pandas_metadata(
@@ -258,52 +260,71 @@
             Whether to build partition level spatial indexes to speed up indexing.
         storage_options: Key/value pairs to be passed on to the file-system backend, if any.
         engine_kwargs: pyarrow.parquet engine-related keyword arguments.
     Returns:
     DaskGeoDataFrame
     """
     # Normalize path to a list
-    if isinstance(path, (str, pathlib.Path)):
-        paths = [str(path)]
+    if isinstance(path, (str, Path)):
+        paths = [path]
     else:
         paths = list(path)
         if not paths:
             raise ValueError('Empty path specification')
 
     # Infer filesystem
     filesystem = validate_coerce_filesystem(
         paths[0],
         filesystem,
         storage_options,
     )
 
-    # Expand glob
-    if len(paths) == 1 and has_magic(paths[0]):
-        paths = filesystem.glob(paths[0])
-        paths = _maybe_prepend_protocol(paths, filesystem)
+    files = []
+    for p in paths:
+        if hasattr(p, "as_posix"):
+            p = p.as_posix()
+        if has_magic(p):
+            # Expand glob paths
+            _files = _expand_path(p, filesystem)
+            files.extend(_files)
+        elif not filesystem.exists(p):
+            raise FileNotFoundError(p)
+        else:
+            files.append(p)
 
     # Perform read parquet
     result = _perform_read_parquet_dask(
-        paths,
-        columns,
-        filesystem,
+        files,
+        columns=columns,
+        filesystem=filesystem,
         load_divisions=load_divisions,
         geometry=geometry,
         bounds=bounds,
         categories=categories,
         storage_options=storage_options,
         engine_kwargs=engine_kwargs,
     )
 
     if build_sindex:
         result = result.build_sindex()
 
     return result
 
 
+def _expand_path(paths, filesystem):
+    # Expand glob paths
+    files = filesystem.expand_path(paths)
+    if isinstance(files, str):
+        files = [files]
+    # Filter out metadata files
+    files = [_ for _ in files if "_metadata" not in _.split("/")[-1]]
+    files = _maybe_prepend_protocol(files, filesystem)
+    return files
+
+
 def _perform_read_parquet_dask(
     paths,
     columns,
     filesystem,
     load_divisions,
     geometry=None,
     bounds=None,
@@ -314,25 +335,31 @@
     engine_kwargs = engine_kwargs or {}
     filesystem = validate_coerce_filesystem(
         paths[0],
         filesystem,
         storage_options,
     )
     if LEGACY_PYARROW:
-        basic_kwargs = dict(filesystem=filesystem, validate_schema=False)
+        basic_kwargs = dict(validate_schema=False)
     else:
-        basic_kwargs = dict(filesystem=filesystem, use_legacy_dataset=False)
+        basic_kwargs = dict(use_legacy_dataset=False)
 
-    datasets = [
-        pa.parquet.ParquetDataset(
+    datasets = []
+    for path in paths:
+        if filesystem.isdir(path):
+            path = f"{path}/**.parquet"
+        if has_magic(path):
+            path = _expand_path(path, filesystem)
+        d = ParquetDataset(
             path,
+            filesystem=filesystem,
             **basic_kwargs,
             **engine_kwargs,
-        ) for path in paths
-    ]
+        )
+        datasets.append(d)
 
     # Create delayed partition for each piece
     pieces = []
     for dataset in datasets:
         # Perform natural sort on pieces so that "part.10" comes after "part.2"
         fragments = getattr(dataset, "fragments", None)
         if fragments is None:
@@ -360,15 +387,18 @@
         div_mins = reduce(lambda a, b: a + b, div_mins_list, [])
         div_maxes = reduce(lambda a, b: a + b, div_maxes_list, [])
     else:
         div_mins = None
         div_maxes = None
 
     # load partition bounds
-    partition_bounds_list = [_load_partition_bounds(dataset) for dataset in datasets]
+    partition_bounds_list = [
+        _load_partition_bounds(dataset, filesystem=filesystem)
+        for dataset in datasets
+    ]
     if not any([b is None for b in partition_bounds_list]):
         partition_bounds = {}
         # We have partition bounds for all datasets
         for partition_bounds_el in partition_bounds_list:
             for col, col_bounds in partition_bounds_el.items():
                 col_bounds_list = partition_bounds.get(col, [])
                 col_bounds_list.append(col_bounds)
@@ -397,15 +427,14 @@
     meta = dd_read_parquet(
         files[0],
         columns=cols_no_index,
         filesystem=filesystem,
         engine='pyarrow',
         categories=categories,
         ignore_metadata_file=True,
-        storage_options=storage_options,
         **engine_kwargs,
     )._meta
 
     meta = GeoDataFrame(meta)
 
     # Handle geometry in meta
     if geometry:
@@ -474,23 +503,36 @@
     # Set partition bounds
     if partition_bounds:
         result._partition_bounds = partition_bounds
 
     return result
 
 
-def _load_partition_bounds(pqds):
+def _get_parent_path(path):
+    if isinstance(path, Iterable) and not isinstance(path, str):
+        path = path[0]
+    parent = str(path).rsplit("/", 1)[0]
+    return parent if parent else "/"
+
+
+def _read_metadata(filename, filesystem):
+    with filesystem.open(filename, "rb") as f:
+        common_metadata = read_metadata(f)
+    return common_metadata
+
+
+def _load_partition_bounds(pqds, filesystem=None):
     partition_bounds = None
 
     if LEGACY_PYARROW:
         common_metadata = pqds.common_metadata
     else:
-        filename = pathlib.Path(pqds.files[0]).parent.joinpath("_common_metadata")
+        filename = "/".join([_get_parent_path(pqds.files[0]), "_common_metadata"])
         try:
-            common_metadata = pq.read_metadata(filename)
+            common_metadata = _read_metadata(filename, filesystem=filesystem)
         except FileNotFoundError:
             common_metadata = None
 
     if common_metadata is not None and b'spatialpandas' in common_metadata.metadata:
         spatial_metadata = json.loads(
             common_metadata.metadata[b'spatialpandas'].decode('utf')
         )
```

### Comparing `spatialpandas-0.4.7/spatialpandas/io/utils.py` & `spatialpandas-0.4.8a1/spatialpandas/io/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -47,9 +47,10 @@
     paths: Iterable[PathType],
     filesystem: fsspec.AbstractFileSystem,
 ) -> Iterable[PathType]:
     protocol = filesystem.protocol if isinstance(
         filesystem.protocol, str) else filesystem.protocol[0]
     if protocol not in ("file", "abstract"):
         # Add back prefix (e.g. s3://)
-        paths = ["{proto}://{p}".format(proto=protocol, p=p) for p in paths]
+        p = f"{protocol}://"
+        paths = [f"{p}{_}" if not _.startswith(p) else _ for _ in paths]
     return paths
```

### Comparing `spatialpandas-0.4.7/spatialpandas/spatialindex/hilbert_curve.py` & `spatialpandas-0.4.8a1/spatialpandas/spatialindex/hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/spatialindex/rtree.py` & `spatialpandas-0.4.8a1/spatialpandas/spatialindex/rtree.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/_create_testdata.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/_create_testdata.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_measures.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_measures.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/algorithms/test_orientation.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/algorithms/test_orientation.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/intersection/test_point_intersection.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/intersection/test_point_intersection.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/strategies.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/strategies.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/test_construction.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_construction.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/test_cx.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_cx.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/test_geometry.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_geometry.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/geometry/test_to_geopandas.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/geometry/test_to_geopandas.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/spatialindex/test_hilbert_curve.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_hilbert_curve.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/spatialindex/test_rtree.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/spatialindex/test_rtree.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_5.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_8.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_5.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_common_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/_metadata`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.0.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/dask_repart_8.0.0.parq/part.1.parquet`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/serial_5.0.0.parq` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_5.0.0.parq`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_data/serial_8.0.0.parq` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_data/serial_8.0.0.parq`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_fixedextensionarray.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_fixedextensionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,17 +216,23 @@
 
     @pytest.mark.skip(
         reason="Searchsorted seems not implemented for custom extension arrays"
     )
     def test_searchsorted(self):
         pass
 
-    @pytest.mark.skip(
-        reason="__setitem__ not supported"
-    )
+    @pytest.mark.skip(reason="__setitem__ not supported")
+    def test_fillna_copy_frame(self, data):
+        pass
+
+    @pytest.mark.skip(reason="__setitem__ not supported")
+    def test_fillna_copy_series(self, data):
+        pass
+
+    @pytest.mark.skip(reason="__setitem__ not supported")
     def test_shift_0_periods(self, data):
         pass
 
     @pytest.mark.skip(
         reason="value_counts not yet supported"
     )
     def test_value_counts_with_normalize(self, data):
```

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_geodataframe.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_geodataframe.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_listextensionarray.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_listextensionarray.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,17 +216,23 @@
 
     @pytest.mark.skip(
         reason="Searchsorted seems not implemented for custom extension arrays"
     )
     def test_searchsorted(self):
         pass
 
-    @pytest.mark.skip(
-        reason="__setitem__ not supported"
-    )
+    @pytest.mark.skip(reason="__setitem__ not supported")
+    def test_fillna_copy_frame(self, data):
+        pass
+
+    @pytest.mark.skip(reason="__setitem__ not supported")
+    def test_fillna_copy_series(self, data):
+        pass
+
+    @pytest.mark.skip(reason="__setitem__ not supported")
     def test_shift_0_periods(self, data):
         pass
 
     @pytest.mark.skip(
         reason="value_counts not yet supported"
     )
     def test_value_counts_with_normalize(self, data):
```

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/test_parquet.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/test_parquet.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tests/tools/test_sjoin.py` & `spatialpandas-0.4.8a1/spatialpandas/tests/tools/test_sjoin.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/tools/sjoin.py` & `spatialpandas-0.4.8a1/spatialpandas/tools/sjoin.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas/utils.py` & `spatialpandas-0.4.8a1/spatialpandas/utils.py`

 * *Files identical despite different names*

### Comparing `spatialpandas-0.4.7/spatialpandas.egg-info/PKG-INFO` & `spatialpandas-0.4.8a1/spatialpandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: spatialpandas
-Version: 0.4.7
+Version: 0.4.8a1
 Summary: Pandas extension arrays for spatial/geometric operations
 Home-page: https://github.com/holoviz/spatialpandas
 Maintainer: HoloViz developers
 Maintainer-email: developers@holoviz.org
 License: BSD-2-Clause
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: examples
 License-File: LICENSE
 
 <img src="https://github.com/holoviz/spatialpandas/raw/main/doc/_static/logo_horizontal.png" data-canonical-src="https://github.com/holoviz/spatialpandas/raw/main/doc/_static/logo_horizontal.png" width="380"/><br>
```

### Comparing `spatialpandas-0.4.7/spatialpandas.egg-info/SOURCES.txt` & `spatialpandas-0.4.8a1/spatialpandas.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 spatialpandas/tests/__init__.py
 spatialpandas/tests/_create_testdata.py
 spatialpandas/tests/test_dask_autoimport.py
 spatialpandas/tests/test_fixedextensionarray.py
 spatialpandas/tests/test_geodataframe.py
 spatialpandas/tests/test_listextensionarray.py
 spatialpandas/tests/test_parquet.py
+spatialpandas/tests/test_parquet_s3.py
 spatialpandas/tests/geometry/__init__.py
 spatialpandas/tests/geometry/strategies.py
 spatialpandas/tests/geometry/test_construction.py
 spatialpandas/tests/geometry/test_cx.py
 spatialpandas/tests/geometry/test_geometry.py
 spatialpandas/tests/geometry/test_to_geopandas.py
 spatialpandas/tests/geometry/algorithms/__init__.py
```

