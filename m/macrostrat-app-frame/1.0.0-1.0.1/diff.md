# Comparing `tmp/macrostrat_app_frame-1.0.0.tar.gz` & `tmp/macrostrat_app_frame-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrostrat_app_frame-1.0.0.tar", max compression
+gzip compressed data, was "macrostrat_app_frame-1.0.1.tar", max compression
```

## Comparing `macrostrat_app_frame-1.0.0.tar` & `macrostrat_app_frame-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       30 2023-05-15 21:32:14.319041 macrostrat_app_frame-1.0.0/macrostrat/app_frame/__init__.py
--rw-r--r--   0        0        0     1010 2023-05-15 21:33:32.603627 macrostrat_app_frame-1.0.0/macrostrat/app_frame/compose.py
--rw-r--r--   0        0        0     5361 2023-05-15 21:32:54.008625 macrostrat_app_frame-1.0.0/macrostrat/app_frame/control_command.py
--rw-r--r--   0        0        0     3780 2023-05-15 21:31:33.953594 macrostrat_app_frame-1.0.0/macrostrat/app_frame/core.py
--rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.0/macrostrat/app_frame/follow_logs.py
--rw-r--r--   0        0        0      426 2023-05-15 21:39:54.281118 macrostrat_app_frame-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      434 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-15 21:52:48.046507 macrostrat_app_frame-1.0.1/macrostrat/app_frame/__init__.py
+-rw-r--r--   0        0        0     1010 2023-05-15 21:33:32.603627 macrostrat_app_frame-1.0.1/macrostrat/app_frame/compose.py
+-rw-r--r--   0        0        0     5361 2023-05-15 21:32:54.008625 macrostrat_app_frame-1.0.1/macrostrat/app_frame/control_command.py
+-rw-r--r--   0        0        0     3780 2023-05-15 21:31:33.953594 macrostrat_app_frame-1.0.1/macrostrat/app_frame/core.py
+-rw-r--r--   0        0        0     2372 2023-05-15 21:32:32.147486 macrostrat_app_frame-1.0.1/macrostrat/app_frame/follow_logs.py
+-rw-r--r--   0        0        0      481 2023-05-15 21:58:59.945254 macrostrat_app_frame-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      529 1970-01-01 00:00:00.000000 macrostrat_app_frame-1.0.1/PKG-INFO
```

### Comparing `macrostrat_app_frame-1.0.0/macrostrat/app_frame/compose.py` & `macrostrat_app_frame-1.0.1/macrostrat/app_frame/compose.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.0/macrostrat/app_frame/control_command.py` & `macrostrat_app_frame-1.0.1/macrostrat/app_frame/control_command.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.0/macrostrat/app_frame/core.py` & `macrostrat_app_frame-1.0.1/macrostrat/app_frame/core.py`

 * *Files identical despite different names*

### Comparing `macrostrat_app_frame-1.0.0/macrostrat/app_frame/follow_logs.py` & `macrostrat_app_frame-1.0.1/macrostrat/app_frame/follow_logs.py`

 * *Files identical despite different names*

