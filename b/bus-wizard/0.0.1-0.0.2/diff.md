# Comparing `tmp/bus_wizard-0.0.1.tar.gz` & `tmp/bus_wizard-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_wizard-0.0.1.tar", last modified: Tue May 16 13:18:09 2023, max compression
+gzip compressed data, was "bus_wizard-0.0.2.tar", last modified: Tue May 16 13:37:03 2023, max compression
```

## Comparing `bus_wizard-0.0.1.tar` & `bus_wizard-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 13:18:09.126141 bus_wizard-0.0.1/
--rw-rw-rw-   0        0        0      668 2023-05-16 13:18:09.126141 bus_wizard-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-05-16 13:02:16.000000 bus_wizard-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 13:18:09.118140 bus_wizard-0.0.1/app/
-drwxrwxrwx   0        0        0        0 2023-05-16 13:18:09.125141 bus_wizard-0.0.1/app/bus_wizard.egg-info/
--rw-rw-rw-   0        0        0      668 2023-05-16 13:18:09.000000 bus_wizard-0.0.1/app/bus_wizard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2023-05-16 13:18:09.000000 bus_wizard-0.0.1/app/bus_wizard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:18:09.000000 bus_wizard-0.0.1/app/bus_wizard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-16 13:18:09.000000 bus_wizard-0.0.1/app/bus_wizard.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 13:18:09.000000 bus_wizard-0.0.1/app/bus_wizard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 13:18:09.126141 bus_wizard-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      882 2023-05-16 13:09:11.000000 bus_wizard-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 13:37:03.316147 bus_wizard-0.0.2/
+-rw-rw-rw-   0        0        0      667 2023-05-16 13:37:03.315150 bus_wizard-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      163 2023-05-16 13:02:16.000000 bus_wizard-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 13:37:03.305148 bus_wizard-0.0.2/app/
+drwxrwxrwx   0        0        0        0 2023-05-16 13:37:03.314159 bus_wizard-0.0.2/app/bus_wizard.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-05-16 13:37:03.000000 bus_wizard-0.0.2/app/bus_wizard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2023-05-16 13:37:03.000000 bus_wizard-0.0.2/app/bus_wizard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:37:03.000000 bus_wizard-0.0.2/app/bus_wizard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-16 13:37:03.000000 bus_wizard-0.0.2/app/bus_wizard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 13:37:03.000000 bus_wizard-0.0.2/app/bus_wizard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 13:37:03.316147 bus_wizard-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-05-16 13:36:33.000000 bus_wizard-0.0.2/setup.py
```

### Comparing `bus_wizard-0.0.1/PKG-INFO` & `bus_wizard-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bus_wizard
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package containing a bus wizard
 Home-page: https://github.com/phanlehoang/bus_wizard
 Author: Hoang Phan Le & An Thu Le
 Author-email: anthule2000@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # A model for bus driver modeling
 
 Our model has some objects:
```

### Comparing `bus_wizard-0.0.1/app/bus_wizard.egg-info/PKG-INFO` & `bus_wizard-0.0.2/app/bus_wizard.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: bus-wizard
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package containing a bus wizard
 Home-page: https://github.com/phanlehoang/bus_wizard
 Author: Hoang Phan Le & An Thu Le
 Author-email: anthule2000@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # A model for bus driver modeling
 
 Our model has some objects:
```

### Comparing `bus_wizard-0.0.1/setup.py` & `bus_wizard-0.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="bus_wizard",
-    version="0.0.1",
+    version="0.0.2",
     description="A package containing a bus wizard",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/phanlehoang/bus_wizard",
     author="Hoang Phan Le & An Thu Le",
@@ -20,9 +20,9 @@
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent",
     ],
     install_requires=["bson >= 0.5.10"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
-    python_requires=">=3.10",
+    python_requires=">=3.9",
 )
```

