# Comparing `tmp/prometheus_http_sd-1.2.2.tar.gz` & `tmp/prometheus_http_sd-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_http_sd-1.2.2.tar", max compression
+gzip compressed data, was "prometheus_http_sd-1.2.3.tar", max compression
```

## Comparing `prometheus_http_sd-1.2.2.tar` & `prometheus_http_sd-1.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-05-11 03:51:33.194050 prometheus_http_sd-1.2.2/LICENSE
--rw-r--r--   0        0        0    11097 2023-05-11 03:51:33.194050 prometheus_http_sd-1.2.2/README.md
--rw-r--r--   0        0        0        0 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/__init__.py
--rw-r--r--   0        0        0     3400 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/app.py
--rw-r--r--   0        0        0     2398 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/cli.py
--rw-r--r--   0        0        0      110 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/config.py
--rw-r--r--   0        0        0       45 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/const.py
--rw-r--r--   0        0        0     6443 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/decorator.py
--rw-r--r--   0        0        0        0 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/exceptions.py
--rw-r--r--   0        0        0     1165 2023-05-11 03:51:33.198050 prometheus_http_sd-1.2.2/prometheus_http_sd/mem_perf.py
--rw-r--r--   0        0        0     4964 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/sd.py
--rw-r--r--   0        0        0      147 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/targets.py
--rw-r--r--   0        0        0     1148 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/templates/admin.html
--rw-r--r--   0        0        0     2118 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/validate.py
--rw-r--r--   0        0        0       18 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/prometheus_http_sd/version.py
--rw-r--r--   0        0        0      648 2023-05-11 03:51:33.202050 prometheus_http_sd-1.2.2/pyproject.toml
--rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-16 09:36:36.282711 prometheus_http_sd-1.2.3/LICENSE
+-rw-r--r--   0        0        0    11097 2023-05-16 09:36:36.282711 prometheus_http_sd-1.2.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/__init__.py
+-rw-r--r--   0        0        0     3774 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/app.py
+-rw-r--r--   0        0        0     2398 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/cli.py
+-rw-r--r--   0        0        0      110 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/config.py
+-rw-r--r--   0        0        0       45 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/const.py
+-rw-r--r--   0        0        0     6443 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/decorator.py
+-rw-r--r--   0        0        0        0 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/exceptions.py
+-rw-r--r--   0        0        0     1165 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/mem_perf.py
+-rw-r--r--   0        0        0     5019 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/sd.py
+-rw-r--r--   0        0        0      147 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/targets.py
+-rw-r--r--   0        0        0     1148 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/templates/admin.html
+-rw-r--r--   0        0        0     2118 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/validate.py
+-rw-r--r--   0        0        0       18 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/prometheus_http_sd/version.py
+-rw-r--r--   0        0        0      648 2023-05-16 09:36:36.286711 prometheus_http_sd-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11866 1970-01-01 00:00:00.000000 prometheus_http_sd-1.2.3/PKG-INFO
```

### Comparing `prometheus_http_sd-1.2.2/LICENSE` & `prometheus_http_sd-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/README.md` & `prometheus_http_sd-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/app.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 version_info = Info(
     "httpsd_version",
     "prometheus_http_sd version info",
 )
 version_info.info({"version": VERSION})
 target_path_requests_total = Counter(
     "httpsd_path_requests_total",
-    "The total count of a path being requested, status label can be"
-    " success/fail",
-    ["path", "status"],
+    (
+        "The total count of a path being requested, status label can be"
+        " success/fail"
+    ),
+    ["path", "status", "l1_dir", "l2_dir"],
 )
 target_path_request_duration_seconds = Histogram(
     "httpsd_target_path_request_duration_seconds",
     "The bucket of request duration in seconds",
     ["path"],
 )
 
@@ -56,35 +58,46 @@
 
     @app.route(f"{prefix}/targets", defaults={"rest_path": ""})
     @app.route(f"{prefix}/targets/", defaults={"rest_path": ""})
     # match the rest of the path
     @app.route(f"{prefix}/targets/<path:rest_path>")
     def get_targets(rest_path):
         logger.info(
-            "request target path: {} with parameters: {}".format(
+            "request target path: {}, with parameters: {}".format(
                 rest_path,
                 request.args,
             )
         )
+
+        l1_dir = l2_dir = ""
+        path_splits = rest_path.split("/")
+        if len(path_splits) > 0:
+            l1_dir = path_splits[0]
+        if len(path_splits) > 1:
+            l2_dir = path_splits[1]
+
         with target_path_request_duration_seconds.labels(
             path=rest_path
         ).time():
             try:
                 targets = generate(config.root_dir, rest_path, **request.args)
             except FileNotFoundError:
                 logger.error(f"Didn't found {config.root_dir}/{rest_path}!")
                 abort(404)
             except:  # noqa: E722
                 target_path_requests_total.labels(
-                    path=rest_path, status="fail"
+                    path=rest_path, status="fail", l1_dir=l1_dir, l2_dir=l2_dir
                 ).inc()
                 raise
             else:
                 target_path_requests_total.labels(
-                    path=rest_path, status="success"
+                    path=rest_path,
+                    status="success",
+                    l1_dir=l1_dir,
+                    l2_dir=l2_dir,
                 ).inc()
                 path_last_generated_targets.labels(path=rest_path).set(
                     sum(len(t.get("targets", [])) for t in targets)
                 )
 
                 return jsonify(targets)
```

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/cli.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/decorator.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/decorator.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/mem_perf.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/mem_perf.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/sd.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/sd.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,31 +38,32 @@
     "httpsd_generator_run_duration_seconds",
     "The time cost that this generator run",
     ["generator"],
 )
 
 
 def should_ignore(file, full_path, ignore_dirs):
-    logger.info(f"{file=}")
     if ignore_dirs:
         for ignore in ignore_dirs:
             if full_path.startswith(ignore):
                 logger.warning(
                     f"{full_path} is ignored due to match ignore"
                     f" pattern {ignore}"
                 )
                 return True
 
     should_ignore_underscore = any(
         p.startswith("_") for p in os.path.normpath(full_path).split(os.sep)
     )
+
     if should_ignore_underscore:
         return True
 
     should_ignore_hidden = file.startswith(".")
+
     if should_ignore_hidden:
         return True
     return False
 
 
 def get_generator_list(
     root: str, path: str = "", ignore_dirs=None
@@ -81,15 +82,17 @@
     if not Path(root).exists():
         raise FileNotFoundError(f"{root} not exist!")
 
     for root, _, files in os.walk(root):
         for file in files:
             full_path = os.path.join(root, file)
 
-            if should_ignore(file, full_path, ignore_dirs):
+            ignore = should_ignore(file, full_path, ignore_dirs)
+            logger.info(f"{file=}, ignore={ignore}")
+            if ignore:
                 continue
 
             generators.append(full_path)
 
     logger.debug(f"{generators=}")
     return generators
```

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/templates/admin.html` & `prometheus_http_sd-1.2.3/prometheus_http_sd/templates/admin.html`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/prometheus_http_sd/validate.py` & `prometheus_http_sd-1.2.3/prometheus_http_sd/validate.py`

 * *Files identical despite different names*

### Comparing `prometheus_http_sd-1.2.2/pyproject.toml` & `prometheus_http_sd-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-http-sd"
-version = "1.2.2"
+version = "1.2.3"
 description = "Prometheus HTTP SD framework."
 authors = ["laixintao <laixintaoo@gmail.com>"]
 readme = 'README.md'
 homepage = "https://python-poetry.org://github.com/laixintao/prometheus-http-sd"
 
 
 [tool.poetry.dependencies]
@@ -15,15 +15,15 @@
 PyYAML = "^6.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 
 [build-system]
-requires = ["poetry-core>=1.2.2"]
+requires = ["poetry-core>=1.2.3"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 79
 
 [tool.poetry.scripts]
 prometheus-http-sd = 'prometheus_http_sd.cli:main'
```

### Comparing `prometheus_http_sd-1.2.2/PKG-INFO` & `prometheus_http_sd-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-http-sd
-Version: 1.2.2
+Version: 1.2.3
 Summary: Prometheus HTTP SD framework.
 Home-page: https://python-poetry.org://github.com/laixintao/prometheus-http-sd
 Author: laixintao
 Author-email: laixintaoo@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

