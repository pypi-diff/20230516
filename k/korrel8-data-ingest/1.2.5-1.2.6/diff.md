# Comparing `tmp/korrel8-data-ingest-1.2.5.tar.gz` & `tmp/korrel8-data-ingest-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "korrel8-data-ingest-1.2.5.tar", last modified: Thu Dec 29 21:28:04 2022, max compression
+gzip compressed data, was "korrel8-data-ingest-1.2.6.tar", last modified: Tue May 16 01:22:50 2023, max compression
```

## Comparing `korrel8-data-ingest-1.2.5.tar` & `korrel8-data-ingest-1.2.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 hari       (501) staff       (20)        0 2022-12-29 21:28:04.542572 korrel8-data-ingest-1.2.5/
--rw-r--r--   0 hari       (501) staff       (20)      483 2022-12-29 21:28:04.542641 korrel8-data-ingest-1.2.5/PKG-INFO
--rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.5/README.txt
-drwxr-xr-x   0 hari       (501) staff       (20)        0 2022-12-29 21:28:04.527054 korrel8-data-ingest-1.2.5/korrel8/
--rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-17 20:32:51.000000 korrel8-data-ingest-1.2.5/korrel8/__init__.py
--rw-r--r--   0 hari       (501) staff       (20)      969 2022-12-17 20:32:55.000000 korrel8-data-ingest-1.2.5/korrel8/downloader.py
--rw-r--r--   0 hari       (501) staff       (20)     1088 2022-12-17 20:32:55.000000 korrel8-data-ingest-1.2.5/korrel8/uploader.py
-drwxr-xr-x   0 hari       (501) staff       (20)        0 2022-12-29 21:28:04.542397 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/
--rw-r--r--   0 hari       (501) staff       (20)      483 2022-12-29 21:28:04.000000 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/PKG-INFO
--rw-r--r--   0 hari       (501) staff       (20)      382 2022-12-29 21:28:04.000000 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/SOURCES.txt
--rw-r--r--   0 hari       (501) staff       (20)        1 2022-12-29 21:28:04.000000 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/dependency_links.txt
--rw-r--r--   0 hari       (501) staff       (20)       14 2022-12-29 21:28:04.000000 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/requires.txt
--rw-r--r--   0 hari       (501) staff       (20)       13 2022-12-29 21:28:04.000000 korrel8-data-ingest-1.2.5/korrel8_data_ingest.egg-info/top_level.txt
--rw-r--r--   0 hari       (501) staff       (20)       85 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.5/pyproject.toml
--rw-r--r--   0 hari       (501) staff       (20)      687 2022-12-29 21:28:04.542945 korrel8-data-ingest-1.2.5/setup.cfg
-drwxr-xr-x   0 hari       (501) staff       (20)        0 2022-12-29 21:28:04.527310 korrel8-data-ingest-1.2.5/test/
--rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.5/test/__init__.py
--rw-r--r--   0 hari       (501) staff       (20)      200 2022-12-17 01:35:27.000000 korrel8-data-ingest-1.2.5/test/test_uploader.py
+drwxr-xr-x   0 hari       (501) staff       (20)        0 2023-05-16 01:22:50.106240 korrel8-data-ingest-1.2.6/
+-rw-r--r--   0 hari       (501) staff       (20)      483 2023-05-16 01:22:50.106321 korrel8-data-ingest-1.2.6/PKG-INFO
+-rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.6/README.txt
+drwxr-xr-x   0 hari       (501) staff       (20)        0 2023-05-16 01:22:50.104794 korrel8-data-ingest-1.2.6/korrel8/
+-rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-17 20:32:51.000000 korrel8-data-ingest-1.2.6/korrel8/__init__.py
+-rw-r--r--   0 hari       (501) staff       (20)     1146 2023-05-16 01:20:11.000000 korrel8-data-ingest-1.2.6/korrel8/copier.py
+-rw-r--r--   0 hari       (501) staff       (20)      969 2022-12-17 20:32:55.000000 korrel8-data-ingest-1.2.6/korrel8/downloader.py
+-rw-r--r--   0 hari       (501) staff       (20)     1088 2022-12-17 20:32:55.000000 korrel8-data-ingest-1.2.6/korrel8/uploader.py
+drwxr-xr-x   0 hari       (501) staff       (20)        0 2023-05-16 01:22:50.106057 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/
+-rw-r--r--   0 hari       (501) staff       (20)      483 2023-05-16 01:22:50.000000 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/PKG-INFO
+-rw-r--r--   0 hari       (501) staff       (20)      402 2023-05-16 01:22:50.000000 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/SOURCES.txt
+-rw-r--r--   0 hari       (501) staff       (20)        1 2023-05-16 01:22:50.000000 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/dependency_links.txt
+-rw-r--r--   0 hari       (501) staff       (20)       14 2023-05-16 01:22:50.000000 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/requires.txt
+-rw-r--r--   0 hari       (501) staff       (20)       13 2023-05-16 01:22:50.000000 korrel8-data-ingest-1.2.6/korrel8_data_ingest.egg-info/top_level.txt
+-rw-r--r--   0 hari       (501) staff       (20)       85 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.6/pyproject.toml
+-rw-r--r--   0 hari       (501) staff       (20)      687 2023-05-16 01:22:50.106699 korrel8-data-ingest-1.2.6/setup.cfg
+drwxr-xr-x   0 hari       (501) staff       (20)        0 2023-05-16 01:22:50.105175 korrel8-data-ingest-1.2.6/test/
+-rw-r--r--   0 hari       (501) staff       (20)        0 2022-12-12 18:41:44.000000 korrel8-data-ingest-1.2.6/test/__init__.py
+-rw-r--r--   0 hari       (501) staff       (20)      200 2022-12-17 01:35:27.000000 korrel8-data-ingest-1.2.6/test/test_uploader.py
```

### Comparing `korrel8-data-ingest-1.2.5/korrel8/downloader.py` & `korrel8-data-ingest-1.2.6/korrel8/downloader.py`

 * *Files identical despite different names*

### Comparing `korrel8-data-ingest-1.2.5/korrel8/uploader.py` & `korrel8-data-ingest-1.2.6/korrel8/uploader.py`

 * *Files identical despite different names*

### Comparing `korrel8-data-ingest-1.2.5/setup.cfg` & `korrel8-data-ingest-1.2.6/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = korrel8-data-ingest
-version = 1.2.5
+version = 1.2.6
 author = Harichandan Pulagam
 author_email = hari@korrel8.ai
 description = Korrel8 Library
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/k8ai
 project_urls =
```

