# Comparing `tmp/pytmac-3.0.0.tar.gz` & `tmp/pytmac-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytmac-3.0.0.tar", last modified: Sun May 14 19:21:20 2023, max compression
+gzip compressed data, was "pytmac-3.1.0.tar", last modified: Tue May 16 20:08:22 2023, max compression
```

## Comparing `pytmac-3.0.0.tar` & `pytmac-3.1.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:21:20.883408 pytmac-3.0.0/
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-14 19:21:20.883408 pytmac-3.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6580 2023-05-14 19:21:17.000000 pytmac-3.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-14 19:21:18.000000 pytmac-3.0.0/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:21:20.883408 pytmac-3.0.0/bin/
--rw-r--r--   0 root         (0) root         (0)    21127 2023-05-14 19:21:17.000000 pytmac-3.0.0/bin/get_config.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-05-14 19:21:17.000000 pytmac-3.0.0/bin/input_validator.py
--rw-r--r--   0 root         (0) root         (0)     2766 2023-05-14 19:21:17.000000 pytmac-3.0.0/bin/resource_validator.py
--rw-r--r--   0 root         (0) root         (0)      242 2023-05-14 19:21:17.000000 pytmac-3.0.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)    18877 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-14 19:21:20.883408 pytmac-3.0.0/pytmac.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6671 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-14 19:21:20.000000 pytmac-3.0.0/pytmac.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-14 19:21:20.883408 pytmac-3.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-14 19:21:17.000000 pytmac-3.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:08:22.696899 pytmac-3.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-16 20:08:19.000000 pytmac-3.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5028 2023-05-16 20:08:22.696899 pytmac-3.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4915 2023-05-16 20:08:19.000000 pytmac-3.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-16 20:08:20.000000 pytmac-3.1.0/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:08:22.692899 pytmac-3.1.0/bin/
+-rw-r--r--   0 root         (0) root         (0)     2719 2023-05-16 20:08:19.000000 pytmac-3.1.0/bin/get_config.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-05-16 20:08:19.000000 pytmac-3.1.0/bin/input_validator.py
+-rw-r--r--   0 root         (0) root         (0)     2766 2023-05-16 20:08:19.000000 pytmac-3.1.0/bin/resource_validator.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:08:22.692899 pytmac-3.1.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-05-16 20:08:19.000000 pytmac-3.1.0/docs/config.yaml
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-05-16 20:08:19.000000 pytmac-3.1.0/docs/defaults.yaml
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-05-16 20:08:19.000000 pytmac-3.1.0/docs/resources.yaml
+-rw-r--r--   0 root         (0) root         (0)     7555 2023-05-16 20:08:19.000000 pytmac-3.1.0/docs/security_checks.yaml
+-rw-r--r--   0 root         (0) root         (0)     1474 2023-05-16 20:08:19.000000 pytmac-3.1.0/docs/swagger.json
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-16 20:08:19.000000 pytmac-3.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)    18878 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-16 20:08:22.696899 pytmac-3.1.0/pytmac.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5028 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       90 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-16 20:08:22.000000 pytmac-3.1.0/pytmac.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-16 20:08:22.696899 pytmac-3.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      868 2023-05-16 20:08:19.000000 pytmac-3.1.0/setup.py
```

### Comparing `pytmac-3.0.0/bin/input_validator.py` & `pytmac-3.1.0/bin/input_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.0.0/bin/resource_validator.py` & `pytmac-3.1.0/bin/resource_validator.py`

 * *Files identical despite different names*

### Comparing `pytmac-3.0.0/pytmac` & `pytmac-3.1.0/pytmac`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     ),
     level=logging.INFO,
     datefmt="%Y-%m-%d %H:%M:%S",
 )
 
 # Use argparse to add arguments
 parser = argparse.ArgumentParser(
-    prog="tmacs",
+    prog="pytmac",
     description="Python based programmatic threat modelling tool",
 )
 parser.add_argument(
     "--version", action="store_true", help="Option to print the current version only"
 )
 parser.add_argument(
     "--demo",
```

### Comparing `pytmac-3.0.0/setup.py` & `pytmac-3.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,10 +21,11 @@
 setup(
     name="pytmac",
     version=__version__,
     long_description=readme_contents,
     long_description_content_type="text/markdown",
     install_requires=required,
     scripts=["pytmac", "_version.py"],
-    packages=["bin"],
+    packages=["bin", "docs"],
     package_data={"docs": ["*"]},
+    exclude_package_data={"docs": ["*bak*"]},
 )
```

