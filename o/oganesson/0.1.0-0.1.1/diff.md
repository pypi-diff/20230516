# Comparing `tmp/oganesson-0.1.0.tar.gz` & `tmp/oganesson-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oganesson-0.1.0.tar", last modified: Tue May  9 01:01:43 2023, max compression
+gzip compressed data, was "oganesson-0.1.1.tar", last modified: Tue May 16 06:40:57 2023, max compression
```

## Comparing `oganesson-0.1.0.tar` & `oganesson-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-09 01:01:43.611136 oganesson-0.1.0/
--rw-rw-rw-   0        0        0       59 2023-05-09 00:53:03.000000 oganesson-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.0/CONTRIBUTING.rst
--rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      412 2023-05-09 01:01:43.609878 oganesson-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-05-09 00:45:17.000000 oganesson-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-09 01:01:43.571153 oganesson-0.1.0/oganesson/
--rw-rw-rw-   0        0        0        5 2023-05-09 00:59:25.000000 oganesson-0.1.0/oganesson/VERSION
--rw-rw-rw-   0        0        0       74 2023-05-09 00:52:11.000000 oganesson-0.1.0/oganesson/__init__.py
--rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.0/oganesson/__main__.py
--rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.0/oganesson/cli.py
--rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.0/oganesson/ogai.py
--rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.0/oganesson/version.py
-drwxrwxrwx   0        0        0        0 2023-05-09 01:01:43.606115 oganesson-0.1.0/oganesson.egg-info/
--rw-rw-rw-   0        0        0      412 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-09 01:01:43.000000 oganesson-0.1.0/oganesson.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-09 01:01:43.611642 oganesson-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1046 2023-05-09 00:58:18.000000 oganesson-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.316781 oganesson-0.1.1/
+-rw-rw-rw-   0        0        0       66 2023-05-09 00:45:17.000000 oganesson-0.1.1/.gitattributes
+-rw-rw-rw-   0        0        0      191 2023-05-16 04:21:08.000000 oganesson-0.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1574 2023-04-18 13:14:12.000000 oganesson-0.1.1/CONTRIBUTING.rst
+-rw-rw-rw-   0        0        0     1107 2023-05-09 00:45:17.000000 oganesson-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      128 2023-05-09 01:01:12.000000 oganesson-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2688 2023-05-16 06:40:57.315784 oganesson-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2235 2023-05-16 06:38:06.000000 oganesson-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.294468 oganesson-0.1.1/oganesson/
+-rw-rw-rw-   0        0        0        5 2023-05-16 03:18:39.000000 oganesson-0.1.1/oganesson/VERSION
+-rw-rw-rw-   0        0        0       74 2023-05-09 00:52:11.000000 oganesson-0.1.1/oganesson/__init__.py
+-rw-rw-rw-   0        0        0       72 2023-05-03 06:26:05.000000 oganesson-0.1.1/oganesson/__main__.py
+-rw-rw-rw-   0        0        0     1234 2023-05-09 00:53:11.000000 oganesson-0.1.1/oganesson/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.310782 oganesson-0.1.1/oganesson/descriptors/
+-rw-rw-rw-   0        0        0     1226 2023-05-16 04:44:12.000000 oganesson-0.1.1/oganesson/descriptors/__init__.py
+-rw-rw-rw-   0        0        0     7896 2023-05-11 01:10:06.000000 oganesson-0.1.1/oganesson/descriptors/bacd.py
+-rw-rw-rw-   0        0        0     3646 2023-05-16 03:55:37.000000 oganesson-0.1.1/oganesson/descriptors/rosa.py
+-rw-rw-rw-   0        0        0     2801 2023-05-16 03:55:40.000000 oganesson-0.1.1/oganesson/descriptors/symmetry_functions.py
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.311785 oganesson-0.1.1/oganesson/genetic_algorithms/
+-rw-rw-rw-   0        0        0     7642 2023-05-16 06:10:22.000000 oganesson-0.1.1/oganesson/genetic_algorithms/__init__.py
+-rw-rw-rw-   0        0        0       21 2023-05-09 00:51:37.000000 oganesson-0.1.1/oganesson/ogai.py
+-rw-rw-rw-   0        0        0     6700 2023-05-16 04:38:44.000000 oganesson-0.1.1/oganesson/ogstructure.py
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.314799 oganesson-0.1.1/oganesson/utilities/
+-rw-rw-rw-   0        0        0      633 2023-05-16 01:59:56.000000 oganesson-0.1.1/oganesson/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1524 2023-05-16 06:10:06.000000 oganesson-0.1.1/oganesson/utilities/atomic_data.py
+-rw-rw-rw-   0        0        0   405452 2023-05-16 02:56:53.000000 oganesson-0.1.1/oganesson/utilities/bonds_dictionary.py
+-rw-rw-rw-   0        0        0      136 2023-05-03 11:28:20.000000 oganesson-0.1.1/oganesson/version.py
+drwxrwxrwx   0        0        0        0 2023-05-16 06:40:57.307351 oganesson-0.1.1/oganesson.egg-info/
+-rw-rw-rw-   0        0        0     2688 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-16 06:40:57.000000 oganesson-0.1.1/oganesson.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 06:40:57.316781 oganesson-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1046 2023-05-09 00:58:18.000000 oganesson-0.1.1/setup.py
```

### Comparing `oganesson-0.1.0/CONTRIBUTING.rst` & `oganesson-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.0/LICENSE` & `oganesson-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.0/oganesson/cli.py` & `oganesson-0.1.1/oganesson/cli.py`

 * *Files identical despite different names*

### Comparing `oganesson-0.1.0/setup.py` & `oganesson-0.1.1/setup.py`

 * *Files identical despite different names*

