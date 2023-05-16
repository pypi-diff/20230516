# Comparing `tmp/geomapi-0.3.0.tar.gz` & `tmp/geomapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geomapi-0.3.0.tar", last modified: Mon Apr 17 15:38:30 2023, max compression
+gzip compressed data, was "geomapi-0.3.1.tar", last modified: Tue May 16 14:34:17 2023, max compression
```

## Comparing `geomapi-0.3.0.tar` & `geomapi-0.3.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.033697 geomapi-0.3.0/
--rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-04-17 15:37:01.000000 geomapi-0.3.0/LICENSE
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-17 15:38:30.033697 geomapi-0.3.0/PKG-INFO
--rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-04-17 15:37:01.000000 geomapi-0.3.0/README.md
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/developmenttests/
--rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-04-17 15:37:01.000000 geomapi-0.3.0/developmenttests/QualityCompare.py
--rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-04-17 15:37:01.000000 geomapi-0.3.0/developmenttests/QualityCompare_gui.py
--rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-04-17 15:37:12.000000 geomapi-0.3.0/developmenttests/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/context.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/ifc_to_nodes.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-04-17 15:37:02.000000 geomapi-0.3.0/developmenttests/import_e57.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/geomapi/
--rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/nodes/
--rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    34991 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/imagenode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/linesetnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/node.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/orthonode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/nodes/sessionnode.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/
--rw-rw-rw-   0 root         (0) daemon       (1)    45354 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/alignmenttools/
--rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/match.py
--rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/alignmenttools/params.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/completiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/completiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/inspectiontools/
--rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/inspectiontools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/machinelearningtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/machinelearningtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/progresstools/
--rw-rw-rw-   0 root         (0) daemon       (1)    35729 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/progresstools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/tools/validationtools/
--rw-rw-rw-   0 root         (0) daemon       (1)    23868 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/tools/validationtools/__init__.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.029697 geomapi-0.3.0/geomapi/utils/
--rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)   108378 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-04-17 15:37:02.000000 geomapi-0.3.0/geomapi/utils/imageutils.py
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.025697 geomapi-0.3.0/geomapi.egg-info/
--rw-r--r--   0 root         (0) daemon       (1)     1508 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) daemon       (1)     1539 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) daemon       (1)        1 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) daemon       (1)      194 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/requires.txt
--rw-r--r--   0 root         (0) daemon       (1)       30 2023-04-17 15:38:30.000000 geomapi-0.3.0/geomapi.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-04-17 15:37:02.000000 geomapi-0.3.0/pyproject.toml
--rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-04-17 15:38:30.033697 geomapi-0.3.0/setup.cfg
-drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-04-17 15:38:30.033697 geomapi-0.3.0/test/
--rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/__init__.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_alignmenttools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_bimnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_completiontools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geometrynode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    24257 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geometryutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_geospatialutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_imageutils.py
--rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_imgnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_meshnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_node.py
--rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_pointcloudnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_progresstools.py
--rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_sessionnode.py
--rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_tools.py
--rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-04-17 15:37:02.000000 geomapi-0.3.0/test/test_utils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.636665 geomapi-0.3.1/
+-rw-rw-rw-   0 root         (0) daemon       (1)     1133 2023-05-16 14:32:42.000000 geomapi-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-05-16 14:34:17.636665 geomapi-0.3.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) daemon       (1)      890 2023-05-16 14:32:42.000000 geomapi-0.3.1/README.md
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/developmenttests/
+-rw-rw-rw-   0 root         (0) daemon       (1)    42245 2023-05-16 14:32:42.000000 geomapi-0.3.1/developmenttests/QualityCompare.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     5108 2023-05-16 14:32:42.000000 geomapi-0.3.1/developmenttests/QualityCompare_gui.py
+-rw-rw-rw-   0 root         (0) daemon       (1)        0 2023-05-16 14:32:53.000000 geomapi-0.3.1/developmenttests/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      119 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/context.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2241 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/ifc_to_nodes.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4911 2023-05-16 14:32:43.000000 geomapi-0.3.1/developmenttests/import_e57.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/geomapi/
+-rw-rw-rw-   0 root         (0) daemon       (1)       64 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/nodes/
+-rw-rw-rw-   0 root         (0) daemon       (1)      372 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12147 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    16209 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    35014 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/imagenode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9033 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/linesetnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     7742 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    22483 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2101 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/orthonode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17538 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27142 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/nodes/sessionnode.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    45777 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/alignmenttools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     2975 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    17867 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/match.py
+-rw-rw-rw-   0 root         (0) daemon       (1)      604 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/alignmenttools/params.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/completiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)     5455 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/completiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/inspectiontools/
+-rw-rw-rw-   0 root         (0) daemon       (1)      306 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/inspectiontools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/machinelearningtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    13233 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/machinelearningtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/progresstools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    41267 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/progresstools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/tools/validationtools/
+-rw-rw-rw-   0 root         (0) daemon       (1)    30354 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/tools/validationtools/__init__.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.632665 geomapi-0.3.1/geomapi/utils/
+-rw-rw-rw-   0 root         (0) daemon       (1)    38758 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)   119403 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     6335 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    26061 2023-05-16 14:32:43.000000 geomapi-0.3.1/geomapi/utils/imageutils.py
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.628665 geomapi-0.3.1/geomapi.egg-info/
+-rw-r--r--   0 root         (0) daemon       (1)     1508 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) daemon       (1)     1539 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) daemon       (1)        1 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) daemon       (1)      194 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) daemon       (1)       30 2023-05-16 14:34:17.000000 geomapi-0.3.1/geomapi.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) daemon       (1)       80 2023-05-16 14:32:43.000000 geomapi-0.3.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) daemon       (1)      921 2023-05-16 14:34:17.636665 geomapi-0.3.1/setup.cfg
+drwxr-sr-x   0 root         (0) daemon       (1)        0 2023-05-16 14:34:17.636665 geomapi-0.3.1/test/
+-rw-rw-rw-   0 root         (0) daemon       (1)      128 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/__init__.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1787 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_alignmenttools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    18912 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_bimnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2023 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_completiontools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    14578 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geometrynode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    24158 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geometryutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     1112 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_geospatialutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     2392 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_imageutils.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    13030 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_imgnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12504 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_meshnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15672 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_node.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    12842 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_pointcloudnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     4270 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_progresstools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)     9408 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_sessionnode.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    15091 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_tools.py
+-rw-rw-rw-   0 root         (0) daemon       (1)    27056 2023-05-16 14:32:43.000000 geomapi-0.3.1/test/test_utils.py
```

### Comparing `geomapi-0.3.0/LICENSE` & `geomapi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/PKG-INFO` & `geomapi-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.3.0/README.md` & `geomapi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/developmenttests/QualityCompare.py` & `geomapi-0.3.1/developmenttests/QualityCompare.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/developmenttests/QualityCompare_gui.py` & `geomapi-0.3.1/developmenttests/QualityCompare_gui.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/developmenttests/ifc_to_nodes.py` & `geomapi-0.3.1/developmenttests/ifc_to_nodes.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/developmenttests/import_e57.py` & `geomapi-0.3.1/developmenttests/import_e57.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/bimnode.py` & `geomapi-0.3.1/geomapi/nodes/bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/geometrynode.py` & `geomapi-0.3.1/geomapi/nodes/geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/imagenode.py` & `geomapi-0.3.1/geomapi/nodes/imagenode.py`

 * *Files 1% similar despite different names*

```diff
@@ -760,22 +760,25 @@
         u=+points[:,1]-self.imageWidth/2
         v=+points[:,0]-self.imageHeight/2    
         camera_coordinates=np.vstack((u,v,np.ones(n)))
         
         #transform to world coordinates
         camera_coordinates=np.vstack((camera_coordinates[0:2,:],np.full(n, f).T,np.ones((n,1)).T))
         world_coordinates=m @ camera_coordinates
-        world_coordinates=gmu.normalize_vectors(world_coordinates[0:3,:].T)
+        
+        #normalize direction
+        displacement=world_coordinates[0:3,:].T-t
+        direction=gmu.normalize_vectors(displacement)
   
         if depths is not None:
-            world_coordinates=world_coordinates * depths[:, np.newaxis]
+            direction=direction * depths[:, np.newaxis]
   
         
-        #create rays [camera.center, direction(world_coordinates)]
-        rays=np.hstack((np.full((n,3), t),world_coordinates))         
+        #create rays [camera.center, direction]
+        rays=np.hstack((np.full((n,3), t),direction))         
         return rays 
     
     # def create_rays(self,imagePoints:np.array)->o3d.core.Tensor:
     #     """Generate a grid a rays from the camera location to a given set of imagePoints.\n
                 
     #     **NOTE**: This function targets a subselection of imagePoints, use o3d.t.geometry.RaycastingScene.create_rays_pinhole if you want a dense raytracing for the full image.
```

### Comparing `geomapi-0.3.0/geomapi/nodes/linesetnode.py` & `geomapi-0.3.1/geomapi/nodes/linesetnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/meshnode.py` & `geomapi-0.3.1/geomapi/nodes/meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/node.py` & `geomapi-0.3.1/geomapi/nodes/node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/orthonode.py` & `geomapi-0.3.1/geomapi/nodes/orthonode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/pointcloudnode.py` & `geomapi-0.3.1/geomapi/nodes/pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/nodes/sessionnode.py` & `geomapi-0.3.1/geomapi/nodes/sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/__init__.py` & `geomapi-0.3.1/geomapi/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,25 +92,29 @@
     mytree = ET.parse(xmlPath)
     root = mytree.getroot()  
 
     #get reference
     chunk=root.find('chunk')
     globalTransform=gmu.get_cartesian_transform(rotation=ut.literal_to_array(chunk.find('transform').find('rotation').text),
                                                 translation= ut.literal_to_array(chunk.find('transform').find('translation').text))
-    globalScale = np.identity(4)*float(chunk.find('transform').find('scale').text)
-    globalScale[-1,-1]=1  
+    # globalScale = np.identity(4)*float(chunk.find('transform').find('scale').text)
+    # globalScale[-1,-1]=1  
+    #! test
+    globalScale=float(chunk.find('transform').find('scale').text)
 
     #get components -> in some xml files, there are no components.
     components=[]
     for component in root.iter('component'):       
         try:
             transform=component.find('transform')
             region=component.find('region')
-            scale = np.identity(4)*float(transform.find('scale').text)
-            scale[-1,-1]=1
+            # scale = np.identity(4)*float(transform.find('scale').text)
+            # scale[-1,-1]=1
+            #! test
+            scale=float(transform.find('scale').text)
             components.append({'componentid':  int(component.get('id')),        
                             'refTransform': gmu.get_cartesian_transform(rotation=ut.literal_to_array(transform.find('rotation').text),
                                                 translation= ut.literal_to_array(transform.find('translation').text)),
                             'scale': scale,
                             'center': gmu.get_cartesian_transform( translation=ut.literal_to_array(region.find('center').text)),
                             'size': ut.literal_to_array(region.find('size').text),
                             'R': ut.literal_to_array(region.find('R').text)})     
@@ -156,15 +160,22 @@
             else:
                 refTransform=globalTransform
                 scale=globalScale
                 
             #get transform
             transform=np.reshape(ut.literal_to_array(cam.find('transform').text),(4,4))
             #apply scale and reference transformation
-            transform=refTransform  @ scale  @ transform
+            
+            #! test
+            transform=gmu.get_cartesian_transform(rotation=transform[0:3,0:3],
+                                        translation=transform[0:3,3]*scale)
+            
+            
+            transform=refTransform  @ transform
+            #transform=refTransform  @ scale  @ transform
 
             #get sensor information
             sensorid=int(cam.get('sensor_id'))      
             sensorInformation= next(s for s in sensors if s is not None and s.get('sensorid')==sensorid)
 
             #create image node 
             import uuid
```

### Comparing `geomapi-0.3.0/geomapi/tools/alignmenttools/__init__.py` & `geomapi-0.3.1/geomapi/tools/alignmenttools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/alignmenttools/match.py` & `geomapi-0.3.1/geomapi/tools/alignmenttools/match.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/alignmenttools/params.py` & `geomapi-0.3.1/geomapi/tools/alignmenttools/params.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/completiontools/__init__.py` & `geomapi-0.3.1/geomapi/tools/completiontools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/machinelearningtools/__init__.py` & `geomapi-0.3.1/geomapi/tools/machinelearningtools/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/tools/progresstools/__init__.py` & `geomapi-0.3.1/geomapi/tools/progresstools/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import geomapi.utils.geometryutils as gmu
 import geomapi.utils.imageutils as iu
 from typing import List,Tuple
 from colour import Color
 from geomapi.nodes import ImageNode
 import copy 
 import os
+import laspy
+import pandas as pd
 
 def create_voxel_block_grid_and_raytrace(pcd,imageNode):
     """THIS CURRENTLY DOESNT WORK BUT IS A PLACEHOLDER.
 
     Args:
         pcd (_type_): _description_
         imageNode (_type_): _description_
@@ -74,14 +76,125 @@
 
     # axs[1, 1].imshow(sum_colors.cpu().numpy())
     # axs[1, 1].set_title('color via indexing')
 
     # plt.tight_layout()
     # plt.show()
 
+def subdivide_pcd_per_box (pcd,size:List[float]=None, parts:List[int]=None)->Tuple[List[int],List[int]]:
+    """Subdivide a point cloud according to a set of boxes (either by size of number of parts).
+    
+    .. image:: ../../../docs/pics/subselection1.PNG
+
+    Args:
+        pcd (las,dataframe or open3d): Point Cloud (only points are used)
+        size (list[float], optional): X, Y and Z size of the subdivided boxes in meter e.g. [10,10,5].
+        parts (list[int], optional): X, Y and Z number of parts to divide the box in e.g. [7,7,1].
+
+    Returns:
+        Tuple[List[int],List[int]]: pathLists with names formatted as 'pcd_{a}_{b}_{c}_{d}' that correspond to xyz order, idxLists with indices per box.
+    """
+    # conver to o3d.geometry.point cloud if necessary
+    if 'laspy.lasdata' in str(type(pcd)):
+        pointcloud=o3d.geometry.PointCloud()
+        pointcloud.points=o3d.utility.Vector3dVector(pcd.xyz)
+        pcd=pointcloud
+    elif 'pandas.DataFrame' in str(type(pcd)):
+        pointcloud=o3d.geometry.PointCloud()
+        pointcloud.points=o3d.utility.Vector3dVector(pcd.iloc[0:2].to_numpy())
+        pcd=pointcloud
+        
+    # create box
+    box=pcd.get_axis_aligned_bounding_box()
+
+    # subdivide box into boxes
+    boxes,names=gmu.divide_box_in_boxes(box,size=size) if size is not None else gmu.divide_box_in_boxes(box,parts=parts)
+
+    # select indices per boxes
+    pathLists=[]
+    idxLists=[]
+    for box,name in zip(boxes,names):
+        pathLists.append(f'pcd_{name[0]}_{name[1]}_{name[2]}')
+        idxLists.append(box.get_point_indices_within_bounding_box(pcd.points))
+    return idxLists,pathLists
+
+def subdivide_pcd_per_octree(pcd,maxDepth:int=4,lowEnd=0,highEnd=2000000)-> Tuple[List[int],List[int]]:
+    """Create an octree of various point clouds and subdivide it according to a voxel octree. For each depth level, the data is divided 8-fold.
+    This function returns the indices per voxel if that node has a number of points between lowEnd and highEnd.
+
+    Args:
+        pcd (las,dataframe or open3d): Point Cloud (only points are used)
+        maxDepth (int, optional): depth of the octree. Defaults to 4.
+        lowEnd (int, optional): minimum number of points in a node for it to be added to the export. Defaults to 0.
+        highEnd (int, optional): maximum number of points in a node for it to be added to the export. If this is surpassed, its children will be assessed. Defaults to 2000000.
+
+    Returns:
+        Tuple[List[int],List[int]]: pathLists with names formatted as 'pcd_{a}_{b}_{c}_{d}' that correspond to the depth ,idxLists with indices per valid node
+    """
+    #validate inputs
+    assert maxDepth >0 and maxDepth <=4, f'maxDepth  should be >0 and <=4 (deeper branchin does not make sense and is not implemented)'
+    
+    # conver to o3d.geometry.point cloud if necessary
+    if 'laspy.lasdata' in str(type(pcd)):
+        pointcloud=o3d.geometry.PointCloud()
+        pointcloud.points=o3d.utility.Vector3dVector(pcd.xyz)
+        pcd=pointcloud
+    elif 'pandas.DataFrame' in str(type(pcd)):
+        pointcloud=o3d.geometry.PointCloud()
+        pointcloud.points=o3d.utility.Vector3dVector(pcd.iloc[0:2].to_numpy())
+        pcd=pointcloud
+    
+    #create octree
+    octree = o3d.geometry.Octree(max_depth=4)
+    octree.convert_from_point_cloud(pcd, size_expand=0.01)
+    
+    #iterate over point cloud node children (maxDepth 4) and return the indices if len(node.indices) are between lowEnd and highEnd
+    a=-1
+    pathLists=[]
+    idxLists=[]
+    # first level
+    for node in octree.root_node.children[0:1]: # depth1
+        a+=1
+        if (getattr(node,'indices',None) is not None and 
+            len(node.indices)> lowEnd and 
+            len(node.indices)< highEnd):
+            pathLists.append(f'pcd_{a}')
+            idxLists.append(node.indices)
+        else:
+            # second level
+            b=-1
+            for childnode in getattr(node,'children',[]): #depth 2
+                b+=1
+                if (getattr(childnode,'indices',None) is not None and 
+                    len(childnode.indices)> lowEnd and 
+                    len(childnode.indices)< highEnd):
+                    pathLists.append(f'pcd_{a}_{b}')
+                    idxLists.append(childnode.indices)
+                else:
+                    #third level
+                    c=-1
+                    for grandchildnode in getattr(childnode,'children',[]): #depth 3
+                        c+=1
+                        if (getattr(grandchildnode,'indices',None) is not None and 
+                            len(grandchildnode.indices)> lowEnd and 
+                            len(grandchildnode.indices)< highEnd):
+                            pathLists.append(f'pcd_{a}_{b}_{c}')
+                            idxLists.append(grandchildnode.indices)
+                        else:
+                            #fourth level
+                            d=-1
+                            for grandgrandchildnode in getattr(grandchildnode,'children',[]): #depth 4
+                                d+=1
+                                if (getattr(grandgrandchildnode,'indices',None) is not None and 
+                                    len(grandgrandchildnode.indices)> lowEnd and 
+                                    len(grandgrandchildnode.indices)< highEnd):
+                                    pathLists.append(f'pcd_{a}_{b}_{c}_{d}')
+                                    idxLists.append(grandgrandchildnode.indices)
+    return idxLists,pathLists
+
 def pcd_to_octree(pcd:o3d.geometry.PointCloud, maDepth:int=7,colorUse:int=0)->o3d.geometry.Octree:
     """Create octree of point cloud and optionally color it consistently.
 
     Args:
         pcd (o3d.geometry.PointCloud): 
         colorUse (int, optional): If 0, the colors per leafNode will be averaged. If 1, the dominant color per LeafNode will be retained (this is quite slow). Defaults to 0.
```

### Comparing `geomapi-0.3.0/geomapi/tools/validationtools/__init__.py` & `geomapi-0.3.1/geomapi/tools/validationtools/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 """
 validationtools - a Python library for validating objects.
 """
 import csv
 import os
 import os.path
-from typing import List
+from typing import List, Tuple
 
 from sklearn.neighbors import NearestNeighbors 
-import laspy 
 
 import geomapi.utils as ut
 import geomapi.utils.geometryutils as gmu
 import matplotlib.pyplot as plt
 import numpy as np
 import open3d as o3d
 import xlsxwriter
 from colour import Color
 from geomapi.nodes import *
-
-# def compute_nearest_neighbor_in_bim(las:laspy.LasData,ref_clouds:List[] resolution:float = 0.1, )
-
-#     compute_nearest_neighbors(reference_points:np.array, query_points:np.array,n:int=1)
+import ezdxf
 
 
 def get_boundingbox_of_list_of_geometries(geometries:List[o3d.geometry.PointCloud]) -> np.array:
     """Determines the global boundingbox of a group of Node containing geometries.
 
     Args:
         geometries (List[Nodes]):  list of Nodes containing a resource of which the boundingbox must be determined"
@@ -538,7 +534,209 @@
                     BIMNode.get_resource()
                 if LOA[2] == 'LOA10':
                     BIMNode.resource.paint_uniform_color([1,0.76,0])
                 if LOA[2] == 'LOA20':
                     BIMNode.resource.paint_uniform_color([1,1,0])
                 if LOA[2] == 'LOA30':
                     BIMNode.resource.paint_uniform_color([0,1,0])
+
+def divide_line_in_sections(linesets,resolution:float=0.1)->np.ndarray:
+
+    #convert to list
+    linesets=ut.item_to_list(linesets)
+
+    for lineset in linesets:
+        #sample every line
+        for line in lineset.lines:
+            start=lineset.points(line.points[0])
+            end=lineset.points(line.points[1])
+            vector=end-start #create line function using start end
+            length=0
+            #compute points on the vector at fixed intervals given the resolution on 
+    
+    return points
+
+
+
+
+def cad_show_lines(dxf_path:str):
+
+    doc = ezdxf.readfile(dxf_path)
+
+    # Extract all line entities from the DXF file
+    msp = doc.modelspace()
+    lines = msp.query("LINE")
+
+    # Plot all the lines using Matplotlib
+    for line in lines:
+        x1, y1, _ = line.dxf.start
+        x2, y2, _ = line.dxf.end
+        plt.plot([x1, x2], [y1, y2])
+
+    plt.show()
+
+def dxf_extract_ezdxf_lines(dxf_path:str) -> List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]:
+    """Import a DXF and extract all line assets.  
+
+    Args:
+        dxf_path (str): path to dxf
+
+    Returns:
+        List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]: (start, end, color, layer, thickness)
+
+    """
+    #open dxf file
+    dwg = ezdxf.readfile(dxf_path)
+    modelspace = dwg.modelspace()
+    
+    #parse lines
+    lines = []
+    for entity in modelspace:
+        if entity.dxftype() == 'LINE': #! make bigger linesets
+            start = entity.dxf.start
+            end = entity.dxf.end
+            color = entity.dxf.color
+            layer = entity.dxf.layer
+            thickness = entity.dxf.lineweight
+            lines.append((start, end, color, layer, thickness))
+    
+    return lines
+
+def create_lineset(line, points:np.ndarray):
+    pcd = o3d.geometry.PointCloud()
+    pcd.points = o3d.utility.Vector3dVector(np.array(points))
+    colors = [line[2]] * len(points) #! this is sketchy
+    pcd.colors = o3d.utility.Vector3dVector(np.array(colors) / 255.0)
+    
+    lineset = o3d.geometry.LineSet.create_from_point_cloud_correspondences(pcd, pcd, [(i, i+1) for i in range(len(points)-1)])
+    lineset.paint_uniform_color(np.array(line[2]) / 255.0)
+    lineset.line_width = line[4]
+    
+    return lineset
+
+def sample_pcd_from_linesets(linesets:List[o3d.geometry.LineSet],step_size:float=0.1)-> List[o3d.geometry.PointCloud]:
+    """Sample a point cloud from a set of o3d.geometry.LineSet elements (color is inherited)
+
+    Args:
+        linesets (List[o3d.geometry.LineSet]): linesets to sample. 
+        step_size(float,optional):spacing between points. Defaults to 0.1m.
+
+    Returns:
+        List[o3d.geometry.PointCloud]: point_clouds
+    """
+    point_clouds=[]
+    for lineset in linesets:
+
+        # Get line segments from the LineSet
+        pointArray=np.asarray(lineset.points)
+        points = []
+
+        for line in np.asarray(lineset.lines):
+            #get start and end
+            start_point = pointArray[line[0]]
+            end_point = pointArray[line[1]]
+            #get direction and length
+            direction = end_point - start_point
+            length = np.linalg.norm(direction)
+            #compute number of points
+            num_points = int(length / step_size)
+            if num_points > 0:
+                step = direction / num_points
+                points.extend([start_point + i * step for i in range(num_points + 1)])
+
+        # Convert the sampled points to an o3d PointCloud
+        point_cloud = o3d.geometry.PointCloud()
+        point_cloud.points = o3d.utility.Vector3dVector(points)
+        color=lineset.colors[0]
+        point_cloud.paint_uniform_color(color)
+        point_clouds.append(point_cloud)
+        
+    return point_clouds
+
+def create_unique_mapping(array:np.ndarray)->Tuple[np.ndarray,np.ndarray]:
+    """Create a unique mapping of an array
+
+    Args:
+        array (np.ndarray): first column of the array will be used for the sorting.
+
+    Returns:
+        Tuple[np.ndarray,np.ndarray]: unique_values, mapping (shape of input array)
+    """
+    #get first array #! this is a bit flawed and supposes that every x-value is unique
+    a=array[:,0]
+    unique_values=np.unique(array,axis=0)
+    
+    # build dictionary
+    fwd = np.argsort(a)
+    asorted = a[fwd]
+    keys = np.unique(asorted) 
+    lower = np.searchsorted(asorted, keys)
+    higher = np.append(lower[1:], len(asorted))
+
+    inv = {key: fwd[lower_i:higher_i]
+            for key, lower_i, higher_i
+            in zip(keys, lower, higher)}
+    
+    # remap values to 0,1,2,....
+    mapping=np.zeros(array.shape[0])
+    i=0
+    for _,value in inv.items():
+            for v in value:
+                    mapping[v]=i
+            i+=1
+    
+    return unique_values,mapping
+
+def ezdxf_lines_to_open3d_linesets(ezdxf_lines:List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]) -> List[o3d.geometry.LineSet]: #
+    """Convert ezdxf lines to open3D linesets. Create 1 lineset per layer.
+
+    Args:
+        ezdxf_lines (List[Tuple[ezdxf.math.vector.Vector,ezdxf.math.vector.Vector,int,str,float]]): (start, end, color, layer, thickness)
+
+    Returns:
+        List[o3d.geometry.LineSet]
+    """  
+    # get layers (str)
+    layers=list(set([line[3] for line in ezdxf_lines]))
+
+    #Convert linesets
+    linesets = []  
+    for layer in layers:
+
+        # get lines in layer
+        lines=[line for line in ezdxf_lines if line[3]==layer]
+        
+        # get start and endpoints       
+        array=np.empty((len(lines)*2,3))
+        for i,line in enumerate(lines): 
+            array[2*i,:]= np.array(line[0])
+            array[2*i+1,:]= np.array(line[1])
+        
+        #get mapping    
+        unique_values,mapping = create_unique_mapping(array)
+
+        #get points and lines and create lineset
+        line_set = o3d.geometry.LineSet() 
+        lineArray=np.reshape(mapping,(len(lines),2))
+        line_set.points = o3d.utility.Vector3dVector(unique_values)  
+        line_set.lines = o3d.utility.Vector2iVector(lineArray)
+        
+        #colorize per color 
+        color=next(line[2] for line in ezdxf_lines if line[3]==layer)/256
+        line_set.paint_uniform_color(np.repeat(color,3))
+        linesets.append(line_set)
+
+    return linesets
+
+def compute_distance_between_open3d_lines(lines:List[o3d.geometry.LineSet],resolution:float=0.1) -> List[float]:
+    """Compute distance between lines at periodic intervals
+
+    Args:
+        lines (List[o3d.geometry.LineSet]): _description_
+        resolution (float, optional): _description_. Defaults to 0.1.
+
+    Returns:
+        List[float]: _description_
+    """
+    distances=[0]
+    return distances
+
```

### Comparing `geomapi-0.3.0/geomapi/utils/__init__.py` & `geomapi-0.3.1/geomapi/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/utils/geometryutils.py` & `geomapi-0.3.1/geomapi/utils/geometryutils.py`

 * *Files 3% similar despite different names*

```diff
@@ -173,27 +173,27 @@
     meshList=[]
     for m in meshes:
         area=m.get_surface_area()
         count=int(area/(resolution*resolution))
         meshList.append(m.sample_points_uniformly(number_of_points=count))
     return meshList
 
-def pcd_get_normals(pcd:o3d.geometry.PointCloud)->np.array:
+def pcd_get_normals(pcd:o3d.geometry.PointCloud)->np.ndarray:
     """Compute open3d point cloud normals if not already present.\n
 
     Args:
         pcd (o3d.geometry.PointCloud)
 
     Returns:
         np.array:
     """
     pcd.estimate_normals() if not pcd.has_normals() else None
     return np.asarray(pcd.normals)
 
-def get_points_and_normals(pcd,transform:np.array=None,getNormals=False)-> Tuple[np.array,np.array]:
+def get_points_and_normals(pcd,transform:np.ndarray=None,getNormals=False)-> Tuple[np.ndarray,np.ndarray]:
     """Extract points from different point cloud formats. Optionally extract or generate normals and apply a rigid body transformation.
 
     Args:
         1. pcd (_type_): point cloud \n
         2. transform (np.array[4,4], optional): Rigid body transformation. Defaults to None.\n
         3. getNormals (bool, optional): Defaults to False.\n
 
@@ -213,20 +213,20 @@
     elif 'DataFrame' in str(type(pcd)):
         pass
         # TODO: implement dataframe query_points and query points
     else:
         raise ValueError('type(pcd) == o3d.geometry.PointCloud, laspy point cloud or pandas dataframe')
     return points,normals
 
-def compute_nearest_neighbor_with_normal_filtering(query_points:np.array,
-                                                    query_normals:np.array, 
-                                                    reference_points:np.array,
-                                                    reference_normals:np.array, 
+def compute_nearest_neighbor_with_normal_filtering(query_points:np.ndarray,
+                                                    query_normals:np.ndarray, 
+                                                    reference_points:np.ndarray,
+                                                    reference_normals:np.ndarray, 
                                                     n:int=5,
-                                                    distanceThreshold=None)->Tuple[np.array,np.array]:
+                                                    distanceThreshold=None)->Tuple[np.ndarray,np.ndarray]:
     """Compute index and distance to nearest neighboring point in the reference dataset.\n
     For the normal fultering, the n closest neighbors are considered of which the correspodence with the best matching normal is retained. \n
 
     **NOTE**:  The index of outliers is set to -1 if distanceTreshold is not None.\n
     
     Args:
         1. query_points (np.array[n,3]): points to evaluate.\n
@@ -255,15 +255,15 @@
     if distanceThreshold is not None:
         assert distanceThreshold>0 ,f'distanceTreshold should be positive, got {distanceThreshold}'
         indices=np.where(distances>distanceThreshold,-1,indices)
         distances=np.where(distances>distanceThreshold,-1,distances)  
         
     return indices,distances
 
-def compute_nearest_neighbors(query_points:np.array,reference_points:np.array, n:int=1)->Tuple[np.array,np.array]:
+def compute_nearest_neighbors(query_points:np.ndarray,reference_points:np.ndarray, n:int=1)->Tuple[np.ndarray,np.ndarray]:
     """Compute nearest neighbors (indices and distances) from querry to reference points.
 
     Args:
         
         1. query_points (np.arrayn): points to calculate the distance from.\n 
         2. reference_points (np.array): points used as a reference.\n        
         3. n (int, optional): number of neighbors. Defaults to 1.\n
@@ -286,15 +286,15 @@
     Returns:
         Tuple(o3d.geometry.PointCloud,o3d.geometry.PointCloud): The points close enough and the points too far away.
     """
     dists = sourcePcd.compute_point_cloud_distance(testPcd)
     ind = np.where(np.asarray(dists) < maxDistance)[0]
     return (sourcePcd.select_by_index(ind), sourcePcd.select_by_index(ind, True))
 
-def get_indices_in_hull(points : np.array, hull :np.array) -> List[int]:
+def get_indices_in_hull(points : np.ndarray, hull :np.ndarray) -> List[int]:
     """Get the indices of all the points that are inside the hull.\n
 
     Args:
         1. points (numpy.array): should be a `NxK` coordinates of `N` points in `K` dimensions.\n
         2. hull (np.array): is either a scipy.spatial.Delaunay object or the `MxK` array of the 
         coordinates of `M` points in `K`dimensions for which Delaunay triangulation will be computed
 
@@ -354,15 +354,15 @@
         open3d.geometry.LineSet: the lineset from the mesh.
     """
     assert len(color)==3 
     ls = o3d.geometry.LineSet.create_from_triangle_mesh(geometry)
     ls.paint_uniform_color(color)
     return ls
 
-def rays_to_points(rays:np.array,distances:np.array=np.array([1.0])) -> Tuple[np.array,np.array]:
+def rays_to_points(rays:np.ndarray,distances:np.ndarray=np.array([1.0])) -> Tuple[np.ndarray,np.ndarray]:
     """Converts a set of rays to start-and endpoints.\n
 
     Args:
         1.rays (np.array[n,6] or o3d.core.Tensor): ray consisting of a startpoint np.array[n,0:3] and a direction np.array[n,3:6].\n
         2.distances (np.array[n], optional): scalar or array with distances of the ray. Defaults to 1.0m.\n
 
     Returns:
@@ -462,15 +462,15 @@
 
         #add to list
         colorImages.append(colorImage)    
         depthImages.append(depthImage)
 
     return colorImages,depthImages
 
-def rays_to_lineset(rays:np.array,distances=None)->o3d.geometry.LineSet:
+def rays_to_lineset(rays:np.ndarray,distances=None)->o3d.geometry.LineSet:
     """Convert an array or o3d.tensor to a lineset that can be visualized in open3d.\n
     
     .. image:: ../../../docs/pics/Raycasting_3.PNG
 
     Args:
         1.rays (np.array[n,6] or o3d.core.Tensor): ray consisting of a startpoint np.array[n,0:3] and a direction np.array[n,3:6]\n
         2.distances (float or np.array[n],Optional): distance/distances over which to cast each ray. Defaults to 1.0m. 
@@ -528,15 +528,26 @@
         (is_collision, names ) = collisionManager.in_collision_single(myTrimesh, transform=None, return_names=True, return_data=False)    
         if is_collision:
             list=[int(name) for name in names]
             return list
     else:
         raise ValueError('condition not met: type(sourceMesh) is o3d.geometry.TriangleMesh and len(sourceMesh.triangles) >0')
 
-def find_nearest(array,value):
+def find_nearest(array:np.ndarray,value:float)->float:
+    """Find value closest to the input value.    
+    
+    **NOTE**: This function will be depreciated 
+    
+    Args:
+        array (np.ndarray): array to evaluate
+        value (float): value to match
+
+    Returns:
+        float: closest value to input vatlue
+    """
     idx = np.searchsorted(array, value, side="left")
     if idx > 0 and (idx == len(array) or math.fabs(value - array[idx-1]) < math.fabs(value - array[idx])):
         return array[idx-1]
     else:
         return array[idx]
 
 def divide_pcd_per_height(heights:List[float], pointCloud:o3d.geometry.PointCloud)->List[o3d.geometry.PointCloud]:
@@ -626,15 +637,15 @@
         pointcloud.colors = o3d.utility.Vector3dVector(tuple[1])
     if tuple[2] is not None:
         pointcloud.normals = o3d.utility.Vector3dVector(tuple[2])
     if len(tuple)==5 and 'ndarray' in str(type(tuple[3])) :
         pointcloud.transform(tuple[3])  
     return pointcloud
 
-def e57_get_cartesian_transform(header:dict)->np.array:
+def e57_get_cartesian_transform(header:dict)->np.ndarray:
     """Returns cartesianTransform (np.array(4x4)) from a e57 header.\n
 
     Args:
         header (dict): retrieved from pye57 e57.get_header(e57Index)
 
     Returns:
         cartesianTransform (np.array(4x4))
@@ -686,15 +697,15 @@
     labelList=np.unique(labels)    
     for l in range(0,labelList[-1]):
         indices = np.where(labels == l)[0]
         pcds.append(pcd.select_by_index(indices))
     return ut.item_to_list(pcds)
 
 def describe_element(name:str, df):
-    """ Takes the columns of a  dataframe and builds a ply-like description.\n
+    """ Takes the columns of a dataframe and builds a ply-like description.\n
     
     Args:
         1. name: str\n
         2. df: pandas DataFrame\n
         
     Returns:
         element: list[str]
@@ -758,14 +769,160 @@
         with open(filename, 'ab') as ply:
             if points is not None:
                 points.to_records(index=False).tofile(ply)
             if mesh is not None:
                 mesh.to_records(index=False).tofile(ply)
     return True
 
+def color_by_intensity(pcd:o3d.geometry.PointCloud, intensities:np.array) -> o3d.geometry.PointCloud:
+    """ Colorize a o3d.geometry.PointCloud with a numpy array of intesities.
+    The intensties are assumed to have a maximum value of 65535.
+    
+    Args:
+        1. pcd (o3d.geometry.PointCloud): Point Cloud to colorize.
+        2. intensities (ndarray): (mx1) values [0-65535].
+        
+    Returns
+        o3d.geometry.PointCloud     
+    """
+    assert intensities.shape[0] == np.asarray(pcd.points).shape[0], f'length intensities ({intensities.shape[0]}) differs from pcd ({np.asarray(pcd.points).shape[0]})'
+    
+    # If the intensity array is RGB encoded, first normalize it using opencv to 16-bit precision
+    intensities_norm = cv2.normalize(intensities, dst=None, alpha=0, beta=65535, norm_type=cv2.NORM_MINMAX)
+
+    # Using numpy.column_stack() provide equal values to RGB values and then assign to 'colors' property 
+    # of the point cloud.
+    # Since Open3D point cloud's 'colors' property is float64 array of shape (num_points, 3), range [0, 1],
+    # we have to normalize the intensity array by dividing it by 65535
+    colors = np.column_stack((intensities_norm, intensities_norm, intensities_norm)) / 65535
+
+    # Now colors array is grayscale array (r = g = b)
+    pcd.colors = o3d.utility.Vector3dVector(colors)
+    return pcd
+
+def array_subsample(array:np.ndarray,percentage:float=0.1)->np.ndarray:
+    """subsample rows of np.array
+
+    Args:
+        array (np.ndarray): 
+        percentage (float, optional): downsampling percentage. Defaults to 0.1.
+
+    Returns:
+        np.ndarray: output array
+    """
+    #create mask of True and False
+    size=math.ceil(array.shape[0]*percentage)
+    choice = np.random.choice(range(array.shape[0]), size=(size,), replace=False)    
+    ind = np.zeros(array.shape[0], dtype=bool)
+    ind[choice] = True
+    
+    #mask the array
+    return array[ind,:] 
+
+def las_subsample(las: laspy.LasData,percentage:float=0.1) -> laspy.LasData:
+    """Subsample a las file given a percentage [0-1].
+    
+    The order is assumed to be ['X','Y','Z','red','green','blue','intensity','classification']
+    
+    **NOTE**: if a classification is present, its maximum value must be <32 (unit4) else the values are remapped
+    
+    Args:
+        1.las ( laspy.LasData): las file
+        2.percentage (float, optional): percentage to downsample [0-1].
+
+    Returns:
+        laspy.lasdata: output las file 
+    """
+    #get all las arrays
+    array,names=las_get_data(las)
+    
+    #subsample array
+    array=array_subsample(array,percentage)
+        
+    #create a new las header
+    header = laspy.LasHeader(point_format=3, version="1.2")
+    header.offsets = np.min(array[:,0:3], axis=0)
+    header.scales = np.array([0.1, 0.1, 0.1])
+    new_las = laspy.LasData(header)
+    
+    #fill in las from array    
+    new_las.x = array[:, 0]
+    new_las.y = array[:, 1]
+    new_las.z = array[:, 2]
+    array=array[:,3:]
+    
+    #add rgb if present
+    if any(n for n in names if n in ['red','green','blue']):
+        new_las.red=array[:, 0]
+        new_las.green=array[:, 1]
+        new_las.blue=array[:, 2]
+        array=array[:,3:]
+    
+    #add intensity if present
+    if any(n for n in names if n in ['intensity']):
+        new_las.intensity=array[:, 0]
+        array=array[:,1:]
+    
+    #add classification if present (max 31)
+    if any(n for n in names if n in ['classification']):        
+        new_las.classification=array[:, 0] if array[:, 0].max()<=31 else array[:, 0]-array[:, 0].min()
+        array=array[:,1:]
+    
+    #create extra dims for scalar fields
+    names= [n for n in names if n not in ['X','Y','Z','red','green','blue','intensity','classification']]
+    dtypes=['float32' for n in names]
+    new_las=las_add_extra_dimensions(new_las,array,names=names,dtypes=dtypes)    
+    
+    return new_las
+
+def dataframe_to_las(dataframe: pd.DataFrame,xyz:List[int]=[0,1,2],rgb:List[int]=None,dtypes:List[str]=None) -> laspy.lasdata:
+    """Convert a dataframe representing a point cloud to a las point cloud file.
+    View laspy dimension and type formatting at https://laspy.readthedocs.io/en/latest/lessbasic.html.\n
+    
+    E.g.: las=dataframe_to_las(dataframe,rgb=[3,4,5])    
+
+    Args:
+        1.dataframe (pd.DataFrame): data frame with a number of columns such as xyz, rgb and some scalar fields (conform numpy)
+        2.xyz (List[int], optional): Indices of the xyz coordinates in the dataframe. Defaults to [0,1,2].
+        3.rgb (List[int], optional): Indices of the color information in the dataframe e.g. [3,4,5]. Defaults to None.
+        4.dtypes (List[str], optional): types of the scalar fields that will be added e.g. ['float32','uint8']. Defaults to [float32] equal to the length of the scalar fields.
+
+    Returns:
+        laspy.lasdata: output las file 
+    """
+    #0.get xyz data
+    xyz=dataframe.iloc[:,:3].to_numpy()
+    # 1. Create a new header
+    header = laspy.LasHeader(point_format=3, version="1.2")
+    header.offsets = np.min(xyz, axis=0)
+    header.scales = np.array([0.1, 0.1, 0.1])
+
+    # 2. Create a Las from xyz
+    las = laspy.LasData(header)
+
+    las.x = xyz[:, 0]
+    las.y = xyz[:, 1]
+    las.z = xyz[:, 2]
+    
+    # 3. add rgb if present
+    if rgb:
+        rgb=dataframe.iloc[:,rgb].to_numpy()
+        las.red=rgb[:, 0]
+        las.green=rgb[:, 1]
+        las.blue=rgb[:, 2]
+        
+    # 4. Create extra dims for scalar fields
+    names=arr.columns[3:] if rgb is None else arr.columns[[t for t in np.arange(3,len(arr.columns)) if t not in rgb]] 
+    dtypes=dtypes if dtypes else ['float32' for n in names]
+    extraBytesParams=[laspy.ExtraBytesParams(name=name, type=dtype) for name,dtype in zip(names,dtypes)]
+    las.add_extra_dims(extraBytesParams)   
+    [setattr(las,name,dataframe[name].to_numpy()) for i,name in enumerate(names)]
+    
+    return las
+
 def las_add_extra_dimensions(las:laspy.LasData, recordData:np.array, names:List[str]=['newField'], dtypes:List[str]=["uint8"] )-> laspy.LasData:
     """Add one or more columns of data to an existing las point cloud file.\n
     View laspy dimension and type formatting at https://laspy.readthedocs.io/en/latest/lessbasic.html.\n
     
     **NOTE**: to be tested
     
     Args:
@@ -779,18 +936,18 @@
     """
     #validate inputs
     names=ut.item_to_list(names)
     dtypes=ut.item_to_list(dtypes)
     assert 'las' in str(type(las))
     assert len(names)==len(dtypes)    
     if 'array' in str(type(recordData)):
-        assert recordData.shape[0]==las.header.point_count ,f'one of the recordData contains entries != (len(las.xyz)).'
+        assert recordData.shape[0]==las.x.shape[0] ,f'one of the recordData contains entries != (len(las.xyz)).'
         assert recordData.shape[1]==len(names), f'recordData.shape[1] !=len(names).'
     elif 'dataframe' in str(type(recordData)):
-        assert len(recordData)==las.header.point_count,f'one of the recordData contains entries != (len(las.xyz)).'
+        assert len(recordData)==las.x.shape[0],f'one of the recordData contains entries != (len(las.xyz)).'
         assert len(recordData.columns)==len(names), f'recordData.shape[1] !=len(names).'
     elif 'Tuple' in str(type(recordData)):
         assert len(recordData)==len(names), f'len(recordData) !=len(names).'
         
     #create dimensions
     extraBytesParams=[laspy.ExtraBytesParams(name=name, type=dtype) for name,dtype in zip(names,dtypes)]
     las.add_extra_dims(extraBytesParams)   
@@ -1073,15 +1230,15 @@
     phi =  rawData.get('sphericalElevation')
     range_cos_phi = range * np.cos(phi)
     pointArray=np.reshape(np.vstack( range_cos_phi * np.cos(theta),
                                     range_cos_phi * np.sin(theta),
                                     range * np.sin(phi)).flatten('F'),(len(range),3))
     return pointArray
 
-def e57_get_xyz_from_raw_data(rawData: dict)->np.array:
+def e57_get_xyz_from_raw_data(rawData: dict)->np.ndarray:
     """Returns the xyz coordinates from e57 raw data.\n
 
     Args:
         rawData (e57 dict):  rawData = e57.read_scan_raw(e57Index).   
         
     Returns:
         np.array (nx3): XYZ cartesian coordinates np.array.
@@ -1575,15 +1732,15 @@
     geometries=ut.item_to_list(geometries)
     for idx,geometry in enumerate(geometries):
         render.scene.add_geometry(str(idx),geometry,mtl) 
     #render image
     img = render.render_to_image()
     return None
 
-def e57_get_normals(rawData:dict)->np.array:
+def e57_get_normals(rawData:dict)->np.ndarray:
     """Returns normal vectors from e57 rawData.\n
 
     Args:
         rawData (dict): e57 dictionary resulting from e57.read_scan_raw(e57Index).\n
 
     Returns:
          np.array(nx3): magnitude 1
@@ -1618,15 +1775,15 @@
         
     #map colors
     colorArray=np.empty((array.shape[0],3))
     for v,c in zip(values,colors):    
         colorArray[array==v]=c
     return colorArray
 
-def e57_get_colors(rawData: dict)->np.array:
+def e57_get_colors(rawData: dict)->np.ndarray:
     """Extract color of intensity information from e57 raw data (3D data) and output Open3D o3d.utility.Vector3dVector(colors).\n
 
     Args:
         rawData(dict): e57 dictionary resulting from e57.read_scan_raw(e57Index)\n
     
     Returns:
         np.array(nx3): RGB or intensity color information. RGB is prioritised.
@@ -1753,35 +1910,96 @@
     if croppedGeometry is not None:
         croppedGeometry=croppedGeometry.rotate(r,center=(0, 0, 0))
         croppedGeometry=croppedGeometry.translate(t)
         return croppedGeometry
     else:
         return None
 
-def expand_box(box: o3d.geometry.OrientedBoundingBox, u=5.0,v=5.0,w=5.0) -> o3d.geometry.OrientedBoundingBox:
-    """expand an o3d.geometry.OrientedBoundingBox in u(x), v(y) and w(z) direction with a certain offset.\n
+def divide_box_in_boxes(box: o3d.geometry.Geometry,size:List[float]=None, parts:List[int]=None)->Tuple[List[o3d.geometry.Geometry],List[str]]:
+    """Subdivide an open3d OrientedBoundingBox or AxisAlignedBoundingBox into a set of smaller boxes (either by size of number of parts).
+    
+    .. image:: ../../../docs/pics/subselection1.PNG
 
     Args:
-        1. box (o3d.geometry.OrientedBoundingBox)\n
-        2. u (float, optional): Offset in X. Defaults to 5.0.\n
-        3. v (float, optional): Offset in Y. Defaults to 5.0.\n
-        4. w (float, optional): Offset in Z. Defaults to 5.0.\n
+        box (o3d.geometry.OrientedBoundingBox or AxisAlignedBoundingBox): box to divide
+        size (list[float], optional): X, Y and Z size of the subdivided boxes in meter e.g. [10,10,5].
+        parts (list[int], optional): X, Y and Z number of parts to divide the box in e.g. [7,7,1].
+
+    Returns:
+        List[o3d.geometry.AxisAlignedBoundingBox]: list of boxes
+    """
+    #parse inputs
+    if 'OrientedBoundingBox' in str(type(box)):
+        # get bounds
+        extent=box.extent()        
+    elif 'AxisAlignedBoundingBox' in str(type(box)):
+        extent=box.get_extent()
+        
+    # get bounds
+    minBound=box.get_min_bound()
+    maxBound=box.get_max_bound()   
+    center=box.get_center() 
+    
+    # get xyz ranges within the box
+    size=size if size is not None and parts is None else extent / np.array(parts)
+    # if size > extent, take centerpoint
+    xRange=np.arange(minBound[0]+size[0]/2,maxBound[0],size[0]) if size[0]<=extent[0] else np.array([center[0]])
+    yRange=np.arange(minBound[1]+size[1]/2,maxBound[1],size[1]) if size[1]<=extent[1] else np.array([center[1]])
+    zRange=np.arange(minBound[2]+size[2]/2,maxBound[2],size[2]) if size[2]<=extent[2] else np.array([center[2]])
+
+    # create names
+    xNames=np.arange(0,len(xRange))
+    yNames=np.arange(0,len(yRange))
+    zNames=np.arange(0,len(zRange))
+    xn,yn,zn=np.meshgrid(xNames,yNames,zNames,indexing='xy')
+    names = np.stack((xn,yn,zn), axis = -1)
+    names=np.reshape(names,(-1,3))
+
+    #create relative center points
+    xx,yy,zz=np.meshgrid(xRange,yRange,zRange,indexing='xy')
+    grid = np.stack((xx,yy,zz), axis = -1)
+    grid_list=np.reshape(grid,(-1,3))
+    #create box
+    small_box=expand_box(box,u=-extent[0]+size[0],v=-extent[1]+size[1],w=-extent[2]+size[2])
+
+    boxes=[]
+    for p in grid_list:
+        box=copy.deepcopy(small_box)
+        box.translate(p,False)
+        boxes.append(box)
+    return boxes,names
+
+def expand_box(box: o3d.geometry, u=5.0,v=5.0,w=5.0) -> o3d.geometry:
+    """expand an o3d.geometry.BoundingBox in u(x), v(y) and w(z) direction with a certain offset.\n
+
+    Args:
+        1. box (o3d.geometry.OrientedBoundingBox or o3d.geometry.AxisAlignedBoundingBox)\n
+        2. u (float, optional): Offset in X. Defaults to 5.0m.\n
+        3. v (float, optional): Offset in Y. Defaults to 5.0m.\n
+        4. w (float, optional): Offset in Z. Defaults to 5.0m.\n
 
     Returns:
-        o3d.geometry.OrientedBoundingBox
+        o3d.geometry.OrientedBoundingBox or o3d.geometry.AxisAlignedBoundingBox
     """    
-    if 'OrientedBoundingBox' not in str(type(box)):
-        raise ValueError('Only OrientedBoundingBox allowed.' )
-    if (u<0 and abs(u)>= box.extent[0]) or (v<0 and abs(v)>=box.extent[1]) or (w<0 and abs(w)>=box.extent[2]):
-        raise ValueError("can't schrink more than the extent of the box")
-
-    center = box.get_center()
-    orientation = box.R 
-    extent = box.extent + [u,v,w] 
-    return o3d.geometry.OrientedBoundingBox(center,orientation,extent) 
+    # if 'OrientedBoundingBox' not in str(type(box)):
+    #     raise ValueError('Only OrientedBoundingBox allowed.' )
+    
+
+    if 'OrientedBoundingBox' in str(type(box)):
+        center = box.get_center()
+        orientation = box.R 
+        extent = box.extent + [u,v,w] 
+        return o3d.geometry.OrientedBoundingBox(center,orientation,extent) 
+    elif 'AxisAlignedBoundingBox' in str(type(box)):
+        # assert ((abs(u)<= box.get_extent()[0]) and (abs(v)<=box.get_extent()[1]) and (abs(w)<=box.get_extent()[2])), f'cannot schrink more than the extent of the box.'
+        minBound=box.get_min_bound()
+        maxBound=box.get_max_bound()
+        new_minBound=minBound-np.array([u,v,w])/2
+        new_maxBound=maxBound+np.array([u,v,w])/2        
+        return o3d.geometry.AxisAlignedBoundingBox(new_minBound,new_maxBound) 
 
 def join_geometries(geometries)->o3d.geometry:
     """Join a number of o3d.PointCloud or o3d.TriangleMesh instances.\n
 
     **NOTE**: Only members of the same geometryType can be merged.\n
 
     Args:
@@ -1824,14 +2042,57 @@
     _,indices=crop_point_cloud_from_meshes(pcd,meshes)
     newDataFrames=[None]*len(meshes)
     for i,list in enumerate(indices):
         if len(list) != 0:
             newDataFrames[i]=df.loc[list]
     return newDataFrames
 
+def las_get_data(las,indices:np.ndarray=None,excludedList:List[str]=None)->np.ndarray:
+    """Get all the relevant data from a las file i.e. the points, colors, intensity and user assigned values such as the classification or features.
+
+    Args:
+        las (laspy.Laspy): point cloud to extract the data from
+        indices (np.ndarray): array with indices to extract
+        excludedList (List[str], optional): List with point fields to exlude. []'X', 'Y', 'Z','red', 'green', 'blue'] should be removed as they are automatically assigned if present. Other values that are excluded are ['X', 'Y', 'Z','red', 'green', 'blue','return_number', 'number_of_returns', 'synthetic', 'key_point', 
+                'withheld', 'overlap', 'scanner_channel', 'scan_direction_flag', 
+                'edge_of_flight_line', 'user_data', 'scan_angle', 'point_source_id', 'gps_time'].
+
+    Returns:
+        np.array (points,colors, user_defined_values)
+    """
+    # get dimension names
+    dimension_names=list(las.point_format.dimension_names)
+
+    # remove unwanted dimension names
+    excludedList=None
+    excludedList=['X', 'Y', 'Z','red', 'green', 'blue','return_number', 'number_of_returns', 'synthetic', 'key_point', 
+                'withheld', 'overlap', 'scanner_channel', 'scan_direction_flag', 
+                'edge_of_flight_line', 'user_data', 'scan_angle', 'point_source_id', 'gps_time'] if excludedList is None else excludedList
+    dimension_names=[dim for dim in dimension_names if dim not in excludedList]
+
+    # gather points
+    data=las.xyz 
+    names=['X', 'Y', 'Z']
+
+    # gather color if present
+    if las['red'].T.shape[0]==data.shape[0]:
+        data=np.hstack((data,np.array([las['red']]).T,np.array([las['red']]).T,np.array([las['red']]).T)) 
+        names.extend(['red', 'green', 'blue'])
+
+    # gather other fields if present
+    for dim in dimension_names:
+        if las[dim].T.shape[0]==data.shape[0] :
+            data=np.hstack((data,np.array([las[dim]]).T)) 
+            names.append(dim)
+    
+    #get indices if present
+    data=data[indices] if indices is not None else data
+    
+    return data,names
+
 def crop_point_cloud_from_meshes(pcd: o3d.geometry.PointCloud,meshes:List[o3d.geometry.TriangleMesh]) -> List[o3d.geometry.PointCloud]:
     """Crop point cloud and divide the inliers per waterthight mesh. \n
 
     Args:
         1. pcd (o3d.geometry.PointCloud): point cloud to be cropped.\n
         2. meshes (o3d.geometry.TriangleMesh). cutter objects.\n 
 
@@ -1952,15 +2213,15 @@
         newnxyz=transform_points( nxyz.to_numpy(),transform) if transform is not None else nxyz.to_numpy()
         #replace column
         for i,n in enumerate(['Nx', 'Ny', 'Nz']):
             df.drop(n, axis = 1, inplace = True)
             df[n] = newnxyz[:,i].tolist()
     return df
 
-def transform_points(points:np.array,transform:np.array)->np.array:
+def transform_points(points:np.ndarray,transform:np.ndarray)->np.ndarray:
     """Transform points with transformation matrix.\n
 
     Args:
         1.points (np.array(:,3)): points to transform\n
         2.transform (np.array(4,4)): transformation Matrix\n
 
     Returns:
@@ -1970,30 +2231,30 @@
     assert(transform.shape[0] == 4)
     assert(transform.shape[1]== 4)
 
     hpoints=np.hstack((points,np.ones((points.shape[0],1))))
     hpoints=transform @ hpoints.transpose()
     return hpoints[0:3].transpose()
 
-def normalize_vectors(array:np.array, axis:int=-1, order:int=2) -> np.array:
+def normalize_vectors(array:np.ndarray, axis:int=-1, order:int=2) -> np.ndarray:
     """Normalize an set of vectors np.array(:,3) to unit vectors len(1).\n
 
     Args:
         array (np.array(:,3))
         axis (int, optional): Defaults to -1.
         order (int, optional): Defaults to 2.
 
     Returns:
         np.array(:,3)
     """
     l2 = np.atleast_1d(np.linalg.norm(array, order, axis))
     l2[l2==0] = 1
     return array / np.expand_dims(l2, axis)
 
-def create_xyz_grid(bounds:List[float], resolutions:List[float])->np.array:
+def create_xyz_grid(bounds:List[float], resolutions:List[float])->np.ndarray:
     """Generate a xyz grid. If only a single value is needed, set the boundaries equal e.g. xMin=xMax and the resolution to 1 e.g. dx=1.\n
 
     Args:
         1.bounds (List[float]): [xMin,xMax,yMin,yMax,zMin,zMax]\n
         2.resolutions (List[float]):[dx,dy,dz]\n
 
     Returns:
@@ -2174,15 +2435,15 @@
     triangles=np.asarray([triangle for idx,triangle in enumerate(mesh.triangles) if idx in triangleIndices])
     centers=np.empty((len(triangles),3))
     for idx,row in enumerate(triangles):
         points=np.array([mesh.vertices[row[0]],mesh.vertices[row[1]],mesh.vertices[row[2]]])
         centers[idx]=np.mean(points,axis=0)
     return centers
 
-def get_cartesian_bounds(geometry : o3d.geometry.Geometry) ->np.array:
+def get_cartesian_bounds(geometry : o3d.geometry.Geometry) ->np.ndarray:
     """Get cartesian bounds from Open3D geometry.\n
 
     Args:
         geometry (o3d.geometry): Open3D geometry supertype (PointCloud, TriangleMesh, OrientedBoundingBox, etc.)\n
 
     Returns:
         np.array: [xMin,xMax,yMin,yMax,zMin,zMax]
```

### Comparing `geomapi-0.3.0/geomapi/utils/geospatialutils.py` & `geomapi-0.3.1/geomapi/utils/geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi/utils/imageutils.py` & `geomapi-0.3.1/geomapi/utils/imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/geomapi.egg-info/PKG-INFO` & `geomapi-0.3.1/geomapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geomapi
-Version: 0.3.0
+Version: 0.3.1
 Summary: A standard library to manage geomatic data
 Home-page: https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 Author: Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 License: MIT
 Keywords: Geomatics,alignment,monitoring,validation,progress,point clouds,computer vision,deep learning
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `geomapi-0.3.0/geomapi.egg-info/SOURCES.txt` & `geomapi-0.3.1/geomapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/setup.cfg` & `geomapi-0.3.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geomapi
-version = 0.3.0
+version = 0.3.1
 author = Bassier M., De Geyter S., De Winter H., Vermandere J. @ Geomatics KU Leuven
 description = A standard library to manage geomatic data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://geomatics.pages.gitlab.kuleuven.be/research-projects/geomapi/
 keywords = Geomatics, alignment, monitoring, validation, progress, point clouds, computer vision, deep learning
 License = MIT
```

### Comparing `geomapi-0.3.0/test/test_alignmenttools.py` & `geomapi-0.3.1/test/test_alignmenttools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_bimnode.py` & `geomapi-0.3.1/test/test_bimnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_completiontools.py` & `geomapi-0.3.1/test/test_completiontools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_geometrynode.py` & `geomapi-0.3.1/test/test_geometrynode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_geometryutils.py` & `geomapi-0.3.1/test/test_geometryutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -448,17 +448,14 @@
         self.assertEqual(expandedbox1.extent[2],box.extent[2]+1)
         
         #negate expansion
         expandedbox2=gmu.expand_box(box,u=-1,v=-1,w=-1)
         self.assertEqual(expandedbox2.extent[0],box.extent[0]-1)
         self.assertEqual(expandedbox2.extent[1],box.extent[1]-1)
         self.assertEqual(expandedbox2.extent[2],box.extent[2]-1)
-
-        #impossible expansion
-        self.assertRaises(ValueError,gmu.expand_box,box=box,u=-55 )
             
     def test_join_geometries(self):
         #TriangleMesh
         mesh1=self.mesh
         mesh2=copy.deepcopy(mesh1)
         mesh2.translate([5,0,0])
         joinedMeshes= gmu.join_geometries([mesh1,mesh2])
```

### Comparing `geomapi-0.3.0/test/test_geospatialutils.py` & `geomapi-0.3.1/test/test_geospatialutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_imageutils.py` & `geomapi-0.3.1/test/test_imageutils.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_imgnode.py` & `geomapi-0.3.1/test/test_imgnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_meshnode.py` & `geomapi-0.3.1/test/test_meshnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_node.py` & `geomapi-0.3.1/test/test_node.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_pointcloudnode.py` & `geomapi-0.3.1/test/test_pointcloudnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_progresstools.py` & `geomapi-0.3.1/test/test_progresstools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_sessionnode.py` & `geomapi-0.3.1/test/test_sessionnode.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_tools.py` & `geomapi-0.3.1/test/test_tools.py`

 * *Files identical despite different names*

### Comparing `geomapi-0.3.0/test/test_utils.py` & `geomapi-0.3.1/test/test_utils.py`

 * *Files identical despite different names*

