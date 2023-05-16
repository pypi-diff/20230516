# Comparing `tmp/arxivai-0.0.2.tar.gz` & `tmp/arxivai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxivai-0.0.2.tar", last modified: Tue May 16 12:28:45 2023, max compression
+gzip compressed data, was "arxivai-0.0.3.tar", last modified: Tue May 16 18:49:51 2023, max compression
```

## Comparing `arxivai-0.0.2.tar` & `arxivai-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:45.943718 arxivai-0.0.2/
--rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      655 2023-05-16 12:28:45.942717 arxivai-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.2/README.md
--rw-rw-rw-   0        0        0      615 2023-05-16 12:28:23.000000 arxivai-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 12:28:45.944718 arxivai-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:45.911720 arxivai-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:45.921717 arxivai-0.0.2/src/arxivai/
--rw-rw-rw-   0        0        0       40 2023-05-16 12:26:54.000000 arxivai-0.0.2/src/arxivai/__init__.py
--rw-rw-rw-   0        0        0       48 2023-05-16 11:58:39.000000 arxivai-0.0.2/src/arxivai/bye.py
--rw-rw-rw-   0        0        0       50 2023-05-16 11:58:09.000000 arxivai-0.0.2/src/arxivai/hello.py
-drwxrwxrwx   0        0        0        0 2023-05-16 12:28:45.940716 arxivai-0.0.2/src/arxivai.egg-info/
--rw-rw-rw-   0        0        0      655 2023-05-16 12:28:45.000000 arxivai-0.0.2/src/arxivai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2023-05-16 12:28:45.000000 arxivai-0.0.2/src/arxivai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 12:28:45.000000 arxivai-0.0.2/src/arxivai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 12:28:45.000000 arxivai-0.0.2/src/arxivai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.252609 arxivai-0.0.3/
+-rw-rw-rw-   0        0        0     1090 2023-05-16 12:09:57.000000 arxivai-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      655 2023-05-16 18:49:51.251607 arxivai-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      122 2023-05-16 12:09:49.000000 arxivai-0.0.3/README.md
+-rw-rw-rw-   0        0        0      652 2023-05-16 18:49:07.000000 arxivai-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-16 18:49:51.252609 arxivai-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.214605 arxivai-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.230609 arxivai-0.0.3/src/arxivai/
+-rw-rw-rw-   0        0        0       24 2023-05-16 18:44:42.000000 arxivai-0.0.3/src/arxivai/__init__.py
+-rw-rw-rw-   0        0        0     4365 2023-05-16 18:33:06.000000 arxivai-0.0.3/src/arxivai/arxiv_api.py
+drwxrwxrwx   0        0        0        0 2023-05-16 18:49:51.249607 arxivai-0.0.3/src/arxivai.egg-info/
+-rw-rw-rw-   0        0        0      655 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-16 18:49:51.000000 arxivai-0.0.3/src/arxivai.egg-info/top_level.txt
```

### Comparing `arxivai-0.0.2/LICENSE` & `arxivai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `arxivai-0.0.2/PKG-INFO` & `arxivai-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `arxivai-0.0.2/pyproject.toml` & `arxivai-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
-requires = ["setuptools>=61.0"]
+requires = [
+  "setuptools",
+  "requests",
+  "beautifulsoup4",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "arxivai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Bongsang Kim", email="happykbs@gmail.com" },
 ]
 description = "A complete arXiv API wrapper for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `arxivai-0.0.2/src/arxivai.egg-info/PKG-INFO` & `arxivai-0.0.3/src/arxivai.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arxivai
-Version: 0.0.2
+Version: 0.0.3
 Summary: A complete arXiv API wrapper for Python.
 Author-email: Bongsang Kim <happykbs@gmail.com>
 Project-URL: Homepage, https://github.com/bongsang/arxivai-pypi
 Project-URL: Bug Tracker, https://github.com/bongsang/arxivai-pypi/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

