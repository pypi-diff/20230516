# Comparing `tmp/vecdb-0.0.4.tar.gz` & `tmp/vecdb-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vecdb-0.0.4.tar", last modified: Thu May  4 00:02:49 2023, max compression
+gzip compressed data, was "vecdb-0.0.5.tar", last modified: Mon May 15 23:58:46 2023, max compression
```

## Comparing `vecdb-0.0.4.tar` & `vecdb-0.0.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-04 00:02:28.000000 vecdb-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 00:02:49.968280 vecdb-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 00:02:28.000000 vecdb-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 00:02:28.000000 vecdb-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:02:49.968280 vecdb-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 00:02:28.000000 vecdb-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_api/test_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-04 00:02:28.000000 vecdb-0.0.4/tests/test_connection_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/api/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/collections/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/collections/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-04 00:02:28.000000 vecdb-0.0.4/vecdb/utils/json_encoder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:02:49.968280 vecdb-0.0.4/vecdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 00:02:49.000000 vecdb-0.0.4/vecdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.238985 vecdb-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-15 23:58:26.000000 vecdb-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 23:58:46.238985 vecdb-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-15 23:58:26.000000 vecdb-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 23:58:26.000000 vecdb-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 23:58:46.238985 vecdb-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-15 23:58:26.000000 vecdb-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_api/test_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-15 23:58:26.000000 vecdb-0.0.5/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16922 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/api/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb/collections/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/collections/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.238985 vecdb-0.0.5/vecdb/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14246 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3499 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-15 23:58:26.000000 vecdb-0.0.5/vecdb/utils/json_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 23:58:46.234985 vecdb-0.0.5/vecdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 23:58:46.000000 vecdb-0.0.5/vecdb.egg-info/top_level.txt
```

### Comparing `vecdb-0.0.4/LICENSE` & `vecdb-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/setup.py` & `vecdb-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/tests/conftest.py` & `vecdb-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/tests/core/test_api/test_client.py` & `vecdb-0.0.5/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/tests/core/test_dataset/test_dataset.py` & `vecdb-0.0.5/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/tests/core/test_dataset/test_field.py` & `vecdb-0.0.5/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/api/api.py` & `vecdb-0.0.5/vecdb/api/api.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/api/local.py` & `vecdb-0.0.5/vecdb/api/local.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/collections/dataset.py` & `vecdb-0.0.5/vecdb/collections/dataset.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/collections/field.py` & `vecdb-0.0.5/vecdb/collections/field.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/types.py` & `vecdb-0.0.5/vecdb/types.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/utils/document.py` & `vecdb-0.0.5/vecdb/utils/document.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/utils/example_documents.py` & `vecdb-0.0.5/vecdb/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb/utils/json_encoder.py` & `vecdb-0.0.5/vecdb/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `vecdb-0.0.4/vecdb.egg-info/SOURCES.txt` & `vecdb-0.0.5/vecdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

