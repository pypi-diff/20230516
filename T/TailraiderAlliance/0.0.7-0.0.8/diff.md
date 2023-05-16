# Comparing `tmp/TailraiderAlliance-0.0.7.tar.gz` & `tmp/TailraiderAlliance-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TailraiderAlliance-0.0.7.tar", last modified: Tue May 16 10:34:47 2023, max compression
+gzip compressed data, was "TailraiderAlliance-0.0.8.tar", last modified: Tue May 16 11:44:15 2023, max compression
```

## Comparing `TailraiderAlliance-0.0.7.tar` & `TailraiderAlliance-0.0.8.tar`

### file list

```diff
@@ -1,31 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.354679 TailraiderAlliance-0.0.7/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0      256 2023-05-16 10:34:47.353634 TailraiderAlliance-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.319824 TailraiderAlliance-0.0.7/TailraiderAlliance/
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.341914 TailraiderAlliance-0.0.7/TailraiderAlliance/Boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.342933 TailraiderAlliance-0.0.7/TailraiderAlliance/Bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.348388 TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/
--rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-05-16 10:27:58.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/catplot.py
--rw-rw-rw-   0        0        0     1302 2023-05-16 10:28:01.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/relplot.py
--rw-rw-rw-   0        0        0     2602 2023-05-16 10:34:28.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Palamute.py
--rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Palico.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.350499 TailraiderAlliance-0.0.7/TailraiderAlliance/Plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.351501 TailraiderAlliance-0.0.7/TailraiderAlliance/Protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.352509 TailraiderAlliance-0.0.7/TailraiderAlliance/Trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/Trouper/__init__.py
--rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.7/TailraiderAlliance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 10:34:47.339522 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-16 10:34:46.000000 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      657 2023-05-16 10:34:47.000000 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 10:34:46.000000 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 10:34:46.000000 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 10:34:46.000000 TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 10:34:47.354679 TailraiderAlliance-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-05-16 10:34:22.000000 TailraiderAlliance-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.572695 TailraiderAlliance-0.0.8/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      256 2023-05-16 11:44:15.571236 TailraiderAlliance-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.504423 TailraiderAlliance-0.0.8/TailraiderAlliance/
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.550850 TailraiderAlliance-0.0.8/TailraiderAlliance/Boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.552218 TailraiderAlliance-0.0.8/TailraiderAlliance/Bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.559933 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/
+-rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-16 10:27:58.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/catplot.py
+-rw-rw-rw-   0        0        0     1302 2023-05-16 10:28:01.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/relplot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.563304 TailraiderAlliance-0.0.8/TailraiderAlliance/Plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.566318 TailraiderAlliance-0.0.8/TailraiderAlliance/Protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.568958 TailraiderAlliance-0.0.8/TailraiderAlliance/Trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Trouper/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.547850 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-16 11:44:13.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-16 11:44:15.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 11:44:13.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 11:44:14.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 11:44:14.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 11:44:15.572695 TailraiderAlliance-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-05-16 11:43:45.000000 TailraiderAlliance-0.0.8/setup.py
```

### Comparing `TailraiderAlliance-0.0.7/LICENSE` & `TailraiderAlliance-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/catplot.py` & `TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/catplot.py`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.7/TailraiderAlliance/Gajalaka/relplot.py` & `TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/relplot.py`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.7/TailraiderAlliance.egg-info/SOURCES.txt` & `TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
-TailraiderAlliance/Palamute.py
-TailraiderAlliance/Palico.py
 TailraiderAlliance/__init__.py
 TailraiderAlliance.egg-info/PKG-INFO
 TailraiderAlliance.egg-info/SOURCES.txt
 TailraiderAlliance.egg-info/dependency_links.txt
 TailraiderAlliance.egg-info/requires.txt
 TailraiderAlliance.egg-info/top_level.txt
 TailraiderAlliance/Boaboa/__init__.py
```

### Comparing `TailraiderAlliance-0.0.7/setup.py` & `TailraiderAlliance-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     name = 'TailraiderAlliance',
-    version = '0.0.7',
+    version = '0.0.8',
     packages = find_packages(include = ['TailraiderAlliance', 'TailraiderAlliance.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

