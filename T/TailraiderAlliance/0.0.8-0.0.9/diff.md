# Comparing `tmp/TailraiderAlliance-0.0.8.tar.gz` & `tmp/TailraiderAlliance-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TailraiderAlliance-0.0.8.tar", last modified: Tue May 16 11:44:15 2023, max compression
+gzip compressed data, was "TailraiderAlliance-0.0.9.tar", last modified: Tue May 16 12:19:27 2023, max compression
```

## Comparing `TailraiderAlliance-0.0.8.tar` & `TailraiderAlliance-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.572695 TailraiderAlliance-0.0.8/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      256 2023-05-16 11:44:15.571236 TailraiderAlliance-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.504423 TailraiderAlliance-0.0.8/TailraiderAlliance/
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.550850 TailraiderAlliance-0.0.8/TailraiderAlliance/Boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.552218 TailraiderAlliance-0.0.8/TailraiderAlliance/Bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.559933 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/
--rw-rw-rw-   0        0        0       48 2023-05-16 09:54:03.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/__init__.py
--rw-rw-rw-   0        0        0     1282 2023-05-16 10:27:58.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/catplot.py
--rw-rw-rw-   0        0        0     1302 2023-05-16 10:28:01.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/relplot.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.563304 TailraiderAlliance-0.0.8/TailraiderAlliance/Plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.566318 TailraiderAlliance-0.0.8/TailraiderAlliance/Protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.568958 TailraiderAlliance-0.0.8/TailraiderAlliance/Trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/Trouper/__init__.py
--rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 TailraiderAlliance-0.0.8/TailraiderAlliance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 11:44:15.547850 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-16 11:44:13.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-16 11:44:15.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 11:44:13.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-16 11:44:14.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-16 11:44:14.000000 TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 11:44:15.572695 TailraiderAlliance-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-05-16 11:43:45.000000 TailraiderAlliance-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.700422 TailraiderAlliance-0.0.9/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      298 2023-05-16 12:19:27.698412 TailraiderAlliance-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.639137 TailraiderAlliance-0.0.9/TailraiderAlliance/
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.672100 TailraiderAlliance-0.0.9/TailraiderAlliance/Boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.674515 TailraiderAlliance-0.0.9/TailraiderAlliance/Bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.689791 TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/
+-rw-rw-rw-   0        0        0       46 2023-05-16 12:15:36.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/__init__.py
+-rw-rw-rw-   0        0        0     1282 2023-05-16 10:27:58.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/catplot.py
+-rw-rw-rw-   0        0        0     1302 2023-05-16 10:28:01.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/relplot.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.692799 TailraiderAlliance-0.0.9/TailraiderAlliance/Plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.694804 TailraiderAlliance-0.0.9/TailraiderAlliance/Protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.696279 TailraiderAlliance-0.0.9/TailraiderAlliance/Trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/Trouper/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-16 11:43:39.000000 TailraiderAlliance-0.0.9/TailraiderAlliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:19:27.670650 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/
+-rw-rw-rw-   0        0        0      298 2023-05-16 12:19:26.000000 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-16 12:19:27.000000 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:19:26.000000 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 12:19:26.000000 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 12:19:26.000000 TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:19:27.701423 TailraiderAlliance-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      567 2023-05-16 12:16:19.000000 TailraiderAlliance-0.0.9/setup.py
```

### Comparing `TailraiderAlliance-0.0.8/LICENSE` & `TailraiderAlliance-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/catplot.py` & `TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/catplot.py`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.8/TailraiderAlliance/Gajalaka/relplot.py` & `TailraiderAlliance-0.0.9/TailraiderAlliance/Gajalaka/relplot.py`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.8/TailraiderAlliance.egg-info/SOURCES.txt` & `TailraiderAlliance-0.0.9/TailraiderAlliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.8/setup.py` & `TailraiderAlliance-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
-    description = 'A package for making Data Science easier',
+    description = 'A package for making Data Science easier, versions with 0.0.x are trials and tests',
     name = 'TailraiderAlliance',
-    version = '0.0.8',
+    version = '0.0.9',
     packages = find_packages(include = ['TailraiderAlliance', 'TailraiderAlliance.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

