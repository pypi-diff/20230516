# Comparing `tmp/vtmmpy-1.0.7.tar.gz` & `tmp/vtmmpy-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vtmmpy-1.0.7.tar", max compression
+gzip compressed data, was "vtmmpy-1.0.8.tar", max compression
```

## Comparing `vtmmpy-1.0.7.tar` & `vtmmpy-1.0.8.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.7/LICENSE
--rw-r--r--   0        0        0      346 2023-05-16 13:29:19.315875 vtmmpy-1.0.7/pyproject.toml
--rw-r--r--   0        0        0     8869 2023-05-16 13:09:25.853982 vtmmpy-1.0.7/src/vtmmpy/__init__.py
--rw-r--r--   0        0        0      625 1970-01-01 00:00:00.000000 vtmmpy-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-19 12:45:40.000000 vtmmpy-1.0.8/LICENSE
+-rw-r--r--   0        0        0     3640 2023-04-28 10:46:41.000000 vtmmpy-1.0.8/README.md
+-rw-r--r--   0        0        0      426 2023-05-16 13:36:49.342503 vtmmpy-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0     8869 2023-05-16 13:09:25.853982 vtmmpy-1.0.8/src/vtmmpy/__init__.py
+-rw-r--r--   0        0        0     4431 1970-01-01 00:00:00.000000 vtmmpy-1.0.8/PKG-INFO
```

### Comparing `vtmmpy-1.0.7/LICENSE` & `vtmmpy-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `vtmmpy-1.0.7/src/vtmmpy/__init__.py` & `vtmmpy-1.0.8/src/vtmmpy/__init__.py`

 * *Files identical despite different names*

