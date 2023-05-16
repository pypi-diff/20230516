# Comparing `tmp/macrometa-target-collection-0.0.59.tar.gz` & `tmp/macrometa-target-collection-0.0.60.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.59.tar", last modified: Mon May 15 08:20:06 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.60.tar", last modified: Tue May 16 09:31:43 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.59.tar` & `macrometa-target-collection-0.0.60.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:20:06.812740 macrometa-target-collection-0.0.59/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-15 08:19:41.000000 macrometa-target-collection-0.0.59/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-15 08:20:06.812740 macrometa-target-collection-0.0.59/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-15 08:19:41.000000 macrometa-target-collection-0.0.59/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:20:06.812740 macrometa-target-collection-0.0.59/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-15 08:19:41.000000 macrometa-target-collection-0.0.59/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14112 2023-05-15 08:19:41.000000 macrometa-target-collection-0.0.59/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 08:20:06.812740 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 08:20:06.000000 macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-15 08:19:41.000000 macrometa-target-collection-0.0.59/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-15 08:20:06.812740 macrometa-target-collection-0.0.59/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14181 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-16 09:31:23.000000 macrometa-target-collection-0.0.60/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.59/LICENSE` & `macrometa-target-collection-0.0.60/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.59/PKG-INFO` & `macrometa-target-collection-0.0.60/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.59
+Version: 0.0.60
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.59/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.60/macrometa_target_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.59/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.60/macrometa_target_collection/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,19 +299,20 @@
     input_messages = io.TextIOWrapper(sys.stdin.buffer, encoding='utf-8')
     state = persist_messages(collection, input_messages, record_batch)
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
     try_upsert(collection, record_batch, force=True)
 
-    # Wait for Prometheus to scrape the metrics
-    logger.info("Waiting for metrics scrape...")
-    while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total", f"workflow=\"{workflow_label}\""):
-        time.sleep(15)
-    logger.info("Metrics scrape complete. Exiting...")
+    if is_metrics_enabled.lower() == 'true':
+        # Wait for Prometheus to scrape the metrics
+        while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total", f"workflow=\"{workflow_label}\""):
+            logger.info("Waiting for metrics scrape...")
+            time.sleep(15)
+        logger.info("Metrics scrape complete. Exiting...")
 
     emit_state(state)
     event_loop.stop()
     logger.info("Completing normally...")
 
 
 def is_scrape_complete(prometheus_url, metric_name, filter):
```

### Comparing `macrometa-target-collection-0.0.59/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.59
+Version: 0.0.60
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.59/pyproject.toml` & `macrometa-target-collection-0.0.60/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.59"
+version = "0.0.60"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

