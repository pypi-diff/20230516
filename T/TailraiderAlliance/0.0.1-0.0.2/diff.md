# Comparing `tmp/TailraiderAlliance-0.0.1.tar.gz` & `tmp/TailraiderAlliance-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TailraiderAlliance-0.0.1.tar", last modified: Mon May 15 11:34:09 2023, max compression
+gzip compressed data, was "TailraiderAlliance-0.0.2.tar", last modified: Tue May 16 09:07:31 2023, max compression
```

## Comparing `TailraiderAlliance-0.0.1.tar` & `TailraiderAlliance-0.0.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.311558 TailraiderAlliance-0.0.1/
--rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.1/LICENSE
--rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      256 2023-05-15 11:34:09.309478 TailraiderAlliance-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.236906 TailraiderAlliance-0.0.1/TailraiderAlliance/
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.288307 TailraiderAlliance-0.0.1/TailraiderAlliance/Boaboa/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Boaboa/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.290262 TailraiderAlliance-0.0.1/TailraiderAlliance/Bugtrapper/
--rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Bugtrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.299454 TailraiderAlliance-0.0.1/TailraiderAlliance/Gajalaka/
--rw-rw-rw-   0        0        0       48 2023-05-15 10:18:54.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Gajalaka/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-15 10:21:16.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Gajalaka/catplot.py
--rw-rw-rw-   0        0        0        0 2023-05-15 09:51:17.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Gajalaka/relplot.py
--rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Palico.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.301647 TailraiderAlliance-0.0.1/TailraiderAlliance/Plunderer/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Plunderer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.305218 TailraiderAlliance-0.0.1/TailraiderAlliance/Protector/
--rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Protector/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.308064 TailraiderAlliance-0.0.1/TailraiderAlliance/Trouper/
--rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/Trouper/__init__.py
--rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.1/TailraiderAlliance/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:34:09.284875 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/
--rw-rw-rw-   0        0        0      256 2023-05-15 11:34:07.000000 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      626 2023-05-15 11:34:08.000000 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:34:07.000000 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2023-05-15 11:34:08.000000 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-15 11:34:08.000000 TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:34:09.312569 TailraiderAlliance-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      525 2023-05-15 11:13:01.000000 TailraiderAlliance-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.114567 TailraiderAlliance-0.0.2/
+-rw-rw-rw-   0        0        0      696 2023-05-15 11:30:33.000000 TailraiderAlliance-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-05-15 11:31:16.000000 TailraiderAlliance-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      256 2023-05-16 09:07:31.114567 TailraiderAlliance-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      278 2023-05-15 11:20:40.000000 TailraiderAlliance-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.081115 TailraiderAlliance-0.0.2/TailraiderAlliance/
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.102478 TailraiderAlliance-0.0.2/TailraiderAlliance/Boaboa/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:32.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Boaboa/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.103483 TailraiderAlliance-0.0.2/TailraiderAlliance/Bugtrapper/
+-rw-rw-rw-   0        0        0       52 2023-05-15 09:41:49.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Bugtrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.109386 TailraiderAlliance-0.0.2/TailraiderAlliance/Gajalaka/
+-rw-rw-rw-   0        0        0      274 2023-05-16 09:04:21.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Gajalaka/__init__.py
+-rw-rw-rw-   0        0        0      957 2023-05-16 09:03:18.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Gajalaka/catplot.py
+-rw-rw-rw-   0        0        0      963 2023-05-16 09:03:16.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Gajalaka/relplot.py
+-rw-rw-rw-   0        0        0       25 2023-05-15 11:16:18.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Palico.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.110815 TailraiderAlliance-0.0.2/TailraiderAlliance/Plunderer/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:46:55.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Plunderer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.112298 TailraiderAlliance-0.0.2/TailraiderAlliance/Protector/
+-rw-rw-rw-   0        0        0        0 2023-05-15 09:47:06.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Protector/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.112298 TailraiderAlliance-0.0.2/TailraiderAlliance/Trouper/
+-rw-rw-rw-   0        0        0        0 2023-05-15 10:03:58.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/Trouper/__init__.py
+-rw-rw-rw-   0        0        0      159 2023-05-15 10:04:09.000000 TailraiderAlliance-0.0.2/TailraiderAlliance/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-16 09:07:31.100379 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-16 09:07:30.000000 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      626 2023-05-16 09:07:30.000000 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 09:07:30.000000 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2023-05-16 09:07:30.000000 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-16 09:07:30.000000 TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 09:07:31.115871 TailraiderAlliance-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      525 2023-05-16 09:07:17.000000 TailraiderAlliance-0.0.2/setup.py
```

### Comparing `TailraiderAlliance-0.0.1/LICENSE` & `TailraiderAlliance-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.1/TailraiderAlliance.egg-info/SOURCES.txt` & `TailraiderAlliance-0.0.2/TailraiderAlliance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TailraiderAlliance-0.0.1/setup.py` & `TailraiderAlliance-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     author = 'Busse Heemskerk',
     description = 'A package for making Data Science easier',
     name = 'TailraiderAlliance',
-    version = '0.0.1',
+    version = '0.0.2',
     packages = find_packages(include = ['TailraiderAlliance', 'TailraiderAlliance.*']),
     install_requires = ['pandas>=1.0',
                         'numpy>=1.0',
                         'matplotlib>=2.2.3',
                         'seaborn>=0.9.0'],
     python_requires = '>=2.7, !=3.0.*, !=3.1.*'
     )
```

