# Comparing `tmp/unidata-blocks-0.0.1.tar.gz` & `tmp/unidata-blocks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unidata-blocks-0.0.1.tar", last modified: Tue May  9 10:56:51 2023, max compression
+gzip compressed data, was "unidata-blocks-0.0.2.tar", last modified: Tue May 16 07:57:49 2023, max compression
```

## Comparing `unidata-blocks-0.0.1.tar` & `unidata-blocks-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.742226 unidata-blocks-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.742226 unidata-blocks-0.0.1/src/unidata_blocks/
--rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/src/unidata_blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/src/unidata_blocks/unidata/
--rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/src/unidata_blocks/unidata/Blocks.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-09 10:56:51.000000 unidata-blocks-0.0.1/src/unidata_blocks.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 10:56:51.746225 unidata-blocks-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-09 10:56:40.000000 unidata-blocks-0.0.1/tests/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/unidata/
+-rw-r--r--   0 runner    (1001) docker     (123)    10951 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/unidata/Blocks.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks/unidata/i18n/
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/src/unidata_blocks/unidata/i18n/zh-cn.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 07:57:49.000000 unidata-blocks-0.0.2/src/unidata_blocks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 07:57:49.161783 unidata-blocks-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-16 07:57:32.000000 unidata-blocks-0.0.2/tests/test_query.py
```

### Comparing `unidata-blocks-0.0.1/LICENSE` & `unidata-blocks-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.1/PKG-INFO` & `unidata-blocks-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
```

### Comparing `unidata-blocks-0.0.1/README.md` & `unidata-blocks-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.1/pyproject.toml` & `unidata-blocks-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "unidata-blocks"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library that helps query unicode blocks by Blocks.txt."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
@@ -20,13 +20,13 @@
 
 [project.urls]
 homepage = "https://github.com/TakWolf/unidata-blocks"
 source = "https://github.com/TakWolf/unidata-blocks"
 issues = "https://github.com/TakWolf/unidata-blocks/issues"
 
 [tool.setuptools]
-package-data = { "unidata_blocks" = ["unidata/*.txt"] }
+package-data = { "unidata_blocks" = ["unidata/*.txt", "unidata/i18n/*.txt"] }
 
 [tool.pytest.ini_options]
 pythonpath = [
     "src",
 ]
```

### Comparing `unidata-blocks-0.0.1/src/unidata_blocks/__init__.py` & `unidata-blocks-0.0.2/src/unidata_blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.1/src/unidata_blocks/unidata/Blocks.txt` & `unidata-blocks-0.0.2/src/unidata_blocks/unidata/Blocks.txt`

 * *Files identical despite different names*

### Comparing `unidata-blocks-0.0.1/src/unidata_blocks.egg-info/PKG-INFO` & `unidata-blocks-0.0.2/src/unidata_blocks.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unidata-blocks
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library that helps query unicode blocks by Blocks.txt.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/unidata-blocks
 Project-URL: source, https://github.com/TakWolf/unidata-blocks
 Project-URL: issues, https://github.com/TakWolf/unidata-blocks/issues
```

### Comparing `unidata-blocks-0.0.1/tests/test_query.py` & `unidata-blocks-0.0.2/tests/test_query.py`

 * *Files identical despite different names*

