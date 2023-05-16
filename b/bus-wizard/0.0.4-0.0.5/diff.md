# Comparing `tmp/bus_wizard-0.0.4.tar.gz` & `tmp/bus_wizard-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_wizard-0.0.4.tar", last modified: Tue May 16 14:00:28 2023, max compression
+gzip compressed data, was "bus_wizard-0.0.5.tar", last modified: Tue May 16 14:04:35 2023, max compression
```

## Comparing `bus_wizard-0.0.4.tar` & `bus_wizard-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 14:00:28.350664 bus_wizard-0.0.4/
--rw-rw-rw-   0        0        0      667 2023-05-16 14:00:28.349673 bus_wizard-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-16 13:02:16.000000 bus_wizard-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 14:00:28.329666 bus_wizard-0.0.4/app/
-drwxrwxrwx   0        0        0        0 2023-05-16 14:00:28.342664 bus_wizard-0.0.4/app/bus_wizard/
--rw-rw-rw-   0        0        0        0 2023-05-16 13:56:50.000000 bus_wizard-0.0.4/app/bus_wizard/__init__.py
--rw-rw-rw-   0        0        0     5664 2023-05-16 12:58:15.000000 bus_wizard-0.0.4/app/bus_wizard/bus_driver_scheduling.py
--rw-rw-rw-   0        0        0      204 2023-05-16 13:01:52.000000 bus_wizard-0.0.4/app/bus_wizard/driver.py
--rw-rw-rw-   0        0        0      344 2023-05-12 09:45:38.000000 bus_wizard-0.0.4/app/bus_wizard/task.py
--rw-rw-rw-   0        0        0     1466 2023-05-16 13:02:10.000000 bus_wizard-0.0.4/app/bus_wizard/task_chain_finder.py
-drwxrwxrwx   0        0        0        0 2023-05-16 14:00:28.348673 bus_wizard-0.0.4/app/bus_wizard.egg-info/
--rw-rw-rw-   0        0        0      667 2023-05-16 14:00:28.000000 bus_wizard-0.0.4/app/bus_wizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-05-16 14:00:28.000000 bus_wizard-0.0.4/app/bus_wizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 14:00:28.000000 bus_wizard-0.0.4/app/bus_wizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-16 14:00:28.000000 bus_wizard-0.0.4/app/bus_wizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-16 14:00:28.000000 bus_wizard-0.0.4/app/bus_wizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 14:00:28.350664 bus_wizard-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-05-16 13:58:39.000000 bus_wizard-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:04:35.871340 bus_wizard-0.0.5/
+-rw-rw-rw-   0        0        0      667 2023-05-16 14:04:35.870340 bus_wizard-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-16 13:02:16.000000 bus_wizard-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 14:04:35.854352 bus_wizard-0.0.5/app/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:04:35.864361 bus_wizard-0.0.5/app/bus_wizard/
+-rw-rw-rw-   0        0        0        0 2023-05-16 13:56:50.000000 bus_wizard-0.0.5/app/bus_wizard/__init__.py
+-rw-rw-rw-   0        0        0     5664 2023-05-16 12:58:15.000000 bus_wizard-0.0.5/app/bus_wizard/bus_driver_scheduling.py
+-rw-rw-rw-   0        0        0      204 2023-05-16 13:01:52.000000 bus_wizard-0.0.5/app/bus_wizard/driver.py
+-rw-rw-rw-   0        0        0      344 2023-05-12 09:45:38.000000 bus_wizard-0.0.5/app/bus_wizard/task.py
+-rw-rw-rw-   0        0        0     1466 2023-05-16 13:02:10.000000 bus_wizard-0.0.5/app/bus_wizard/task_chain_finder.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:04:35.869340 bus_wizard-0.0.5/app/bus_wizard.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-05-16 14:04:35.000000 bus_wizard-0.0.5/app/bus_wizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-05-16 14:04:35.000000 bus_wizard-0.0.5/app/bus_wizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:04:35.000000 bus_wizard-0.0.5/app/bus_wizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-16 14:04:35.000000 bus_wizard-0.0.5/app/bus_wizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 14:04:35.000000 bus_wizard-0.0.5/app/bus_wizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 14:04:35.871340 bus_wizard-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-05-16 14:04:09.000000 bus_wizard-0.0.5/setup.py
```

### Comparing `bus_wizard-0.0.4/PKG-INFO` & `bus_wizard-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus_wizard
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package containing a bus wizard
 Home-page: https://github.com/phanlehoang/bus_wizard
 Author: Hoang Phan Le & An Thu Le
 Author-email: anthule2000@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bus_wizard-0.0.4/app/bus_wizard/bus_driver_scheduling.py` & `bus_wizard-0.0.5/app/bus_wizard/bus_driver_scheduling.py`

 * *Files identical despite different names*

### Comparing `bus_wizard-0.0.4/app/bus_wizard/task_chain_finder.py` & `bus_wizard-0.0.5/app/bus_wizard/task_chain_finder.py`

 * *Files identical despite different names*

### Comparing `bus_wizard-0.0.4/app/bus_wizard.egg-info/PKG-INFO` & `bus_wizard-0.0.5/app/bus_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus-wizard
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package containing a bus wizard
 Home-page: https://github.com/phanlehoang/bus_wizard
 Author: Hoang Phan Le & An Thu Le
 Author-email: anthule2000@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bus_wizard-0.0.4/setup.py` & `bus_wizard-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="bus_wizard",
-    version="0.0.4",
+    version="0.0.5",
     description="A package containing a bus wizard",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phanlehoang/bus_wizard",
     author="Hoang Phan Le & An Thu Le",
```

