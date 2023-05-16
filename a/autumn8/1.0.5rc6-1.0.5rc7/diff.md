# Comparing `tmp/autumn8-1.0.5rc6.tar.gz` & `tmp/autumn8-1.0.5rc7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc6.tar", last modified: Tue May 16 11:21:44 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc7.tar", last modified: Tue May 16 13:55:30 2023, max compression
```

## Comparing `autumn8-1.0.5rc6.tar` & `autumn8-1.0.5rc7.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc6/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.625373 autumn8-1.0.5rc6/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12672 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4850 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 11:20:36.000000 autumn8-1.0.5rc6/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc6/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc6/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc6/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc6/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc6/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11875 2023-05-16 11:19:37.000000 autumn8-1.0.5rc6/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc6/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc6/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.625373 autumn8-1.0.5rc6/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc7/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.751744 autumn8-1.0.5rc7/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13488 2023-05-16 13:55:08.000000 autumn8-1.0.5rc7/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 13:13:29.000000 autumn8-1.0.5rc7/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4850 2023-05-16 11:20:08.000000 autumn8-1.0.5rc7/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 13:54:52.000000 autumn8-1.0.5rc7/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc7/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc7/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc7/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc7/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc7/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc7/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc7/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc7/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.751744 autumn8-1.0.5rc7/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc6/PKG-INFO` & `autumn8-1.0.5rc7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc6
+Version: 1.0.5rc7
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc6/README.md` & `autumn8-1.0.5rc7/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/analyze.py` & `autumn8-1.0.5rc7/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc7/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc7/autumn8/cli/commands/cloud.py`

 * *Files 5% similar despite different names*

```diff
@@ -260,14 +260,22 @@
     "--container_http_request_path",
     type=str,
     default="",
     prompt=True,
     help="HTTP path on the Docker container to query against",
 )
 @click.option(
+    "-H",
+    "--custom_headers",
+    type=str,
+    multiple=True,
+    default=[],
+    help="Custom HTTP headers to pass",
+)
+@click.option(
     "-i",
     "--input",
     type=str,
     help="JSON / Raw Text HTTP Body input to pass within the HTTP request",
 )
 async def run_docker(
     organization_id: int,
@@ -276,14 +284,15 @@
     quiet: bool,
     docker_image_name: str = "",
     docker_port: Optional[int] = None,
     docker_container_registry: Optional[
         str
     ] = DEFAULT_DOCKER_CONTAINER_REGISTRY,
     container_http_request_path: str = "",
+    custom_headers: List[str] = [],
     # disabled, cause these are not working properly right now on a8f
     # docker_environment: Optional[Dict[str, str]] = None,
     # docker_entrypoint: Optional[str] = None,
     input: Union[Dict[str, str], List[str], str, None] = None,
 ):
     """
     Run an inference on a given Docker image by creating
@@ -307,14 +316,23 @@
 
     if container_http_request_path.startswith("/"):
         container_http_request_path = container_http_request_path[1:]
 
     api_keys = api.user.fetch_org_api_keys(environment, organization_id)
     inference_api_key = api_keys[0]["api_key"]
 
+    custom_headers_parsed = {}
+    for entry in custom_headers:
+        split = entry.split(":")
+        if len(split) != 2:
+            print(f'"{entry}" is not a valid header entry, skipping...')
+
+        [header, value] = split
+        custom_headers_parsed[header.strip()] = value.strip()
+
     async with httpx.AsyncClient(
         auth=(str(organization_id), inference_api_key)
     ) as httpClient:
         query: str = build_docker_processing_query_string(
             organization_id, machine_type
         )
         url = posixpath.join(
@@ -328,14 +346,15 @@
             json={
                 "container_image_name": docker_image_name,
                 "container_registry": docker_container_registry,
                 "container_port": docker_port,
                 "http_request_input": input,
                 "http_request_path": container_http_request_path,
             },
+            headers=custom_headers_parsed,
             timeout=None,
         )
 
         logger.info("Container responded with:")
         click.echo(response.text)
         response.raise_for_status()
 
@@ -395,16 +414,18 @@
     Run an inference on a given deployment
     """
 
     api_keys = api.user.fetch_org_api_keys(environment, organization_id)
     inference_api_key = api_keys[0]["api_key"]
 
     if decode64 and output_file is None:
-        click.echo("Please specify output file to decode base64 to")
-        return
+        output_file = questionary.text(
+            "Please specify output file to decode base64 to",
+            default="",
+        ).unsafe_ask()
 
     if deployment_url is None:
         deployment_url = get_deployment(
             organization_id, environment, model_id=model_id
         )
 
     if input_file is not None:
@@ -414,41 +435,50 @@
 
     if deployment_url is None:
         click.echo(
             "You need to specify either deployment_url or choose existing deployment"
         )
         return
 
-    if model_input is None:
-        click.echo("You need to either specify model_input or input_file")
-        return
+    final_input: str = (
+        model_input
+        if model_input is not None
+        else questionary.text("JSON model input").unsafe_ask()
+    )
+
+    json_input = None
+    try:
+        json_input = json.loads(final_input)
+    except json.JSONDecodeError:
+        pass
 
     with httpx.Client(
         auth=(str(organization_id), inference_api_key)
     ) as httpClient:
         response: httpx.Response = httpClient.post(
             url=deployment_url,
-            json=json.loads(model_input),
+            json=json_input if json_input is not None else None,
+            content=final_input if json_input is None else None,
             timeout=None,
         )
-        if not decode64:
-            logger.info("Deployment responded with:")
-            click.echo(response.text)
-            response.raise_for_status()
-            if output_file is not None:
-                with open(output_file, "w") as f:
-                    f.write(response.text)
-        else:
+        if decode64:
             data = json.loads(response.text)
             if "message" in data and "output" in data["message"]:
                 model_output_base64 = data["message"]["output"]
                 model_output = decode_base64_model_output(model_output_base64)
                 if (
                     output_file is None
                 ):  # check for this is above, additional check for pylint
                     return
                 with open(output_file, "wb") as f:
                     f.write(model_output)
             else:
                 logger.info("Deployment responded with:")
                 click.echo(response.text)
                 response.raise_for_status()
+        else:
+            logger.info("Deployment responded with:")
+            click.echo(response.text)
+            response.raise_for_status()
+            if output_file is not None:
+                with open(output_file, "w") as f:
+                    f.write(response.text)
```

### Comparing `autumn8-1.0.5rc6/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc7/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/examples.py` & `autumn8-1.0.5rc7/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/interactive.py` & `autumn8-1.0.5rc7/autumn8/cli/interactive.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/main.py` & `autumn8-1.0.5rc7/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/options.py` & `autumn8-1.0.5rc7/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc7/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/cli/validation.py` & `autumn8-1.0.5rc7/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc7/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/common/config/settings.py` & `autumn8-1.0.5rc7/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc7/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/common/types.py` & `autumn8-1.0.5rc7/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/env/__init__.py` & `autumn8-1.0.5rc7/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/examples/mnist.py` & `autumn8-1.0.5rc7/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/examples/model.py` & `autumn8-1.0.5rc7/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc7/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc7/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/__init__.py` & `autumn8-1.0.5rc7/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc7/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc7/autumn8/lib/api/lab.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from threading import Lock
 from typing import Any, Dict, List, Literal, Optional, TypedDict, Union
 
 import appdirs
 import boto3
 import httpx
 import requests
-from mypy_boto3_s3 import S3Client
+from mypy_boto3_s3 import S3Client, S3ServiceResource
 from mypy_boto3_s3.type_defs import PartTypeDef
 from mypy_boto3_sts.type_defs import CredentialsTypeDef
 from requests.auth import HTTPBasicAuth
 from tqdm.contrib.concurrent import thread_map
 
 from autumn8.cli import pending_uploads
 from autumn8.cli.analyze import is_model_file_link_external, s3path_join
@@ -176,15 +176,15 @@
 
     require_ok_response(response)
     return FileUploadPermissionsResponse(response.json())
 
 
 def get_s3_resource_from_temporary_permissions(
     environment: CliEnvironment, permissions: FileUploadPermissionsResponse
-):
+) -> S3ServiceResource:
     credentials = permissions["credentials"]
 
     session = boto3.Session(
         aws_access_key_id=credentials["AccessKeyId"],
         aws_secret_access_key=credentials["SecretAccessKey"],
         aws_session_token=credentials["SessionToken"],
     )
@@ -341,14 +341,16 @@
                     "ETag": part.get("ETag"),
                 }
                 for part in all_parts
             ]
         },
     )
 
+    return permissions["object_key"]
+
 
 # TODO: fix s3 file structure so that this is not needed
 def get_hacked_legacy_backwards_compatible_s3_file_url(
     s3_root_folder_name: Optional[str],
     s3_file_url: str,
 ):
     return s3path_join(s3_root_folder_name or "", s3_file_url)
```

### Comparing `autumn8-1.0.5rc6/autumn8/lib/api/user.py` & `autumn8-1.0.5rc7/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc7/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc7/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/http.py` & `autumn8-1.0.5rc7/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/logging.py` & `autumn8-1.0.5rc7/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc7/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc7/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8/lib/service.py` & `autumn8-1.0.5rc7/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc7/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc6
+Version: 1.0.5rc7
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc6/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc7/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/pyproject.toml` & `autumn8-1.0.5rc7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc7/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc6/tests/test_settings.py` & `autumn8-1.0.5rc7/tests/test_settings.py`

 * *Files identical despite different names*

