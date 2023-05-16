# Comparing `tmp/autumn8-1.0.5rc5.tar.gz` & `tmp/autumn8-1.0.5rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc5.tar", last modified: Mon May 15 15:00:54 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc6.tar", last modified: Tue May 16 11:21:44 2023, max compression
```

## Comparing `autumn8-1.0.5rc5.tar` & `autumn8-1.0.5rc6.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-15 13:51:44.000000 autumn8-1.0.5rc5/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13237 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16089 2023-05-15 12:34:48.000000 autumn8-1.0.5rc5/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4094 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-15 15:00:22.000000 autumn8-1.0.5rc5/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc5/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc5/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc5/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc5/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc5/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc5/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11875 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-15 15:00:03.000000 autumn8-1.0.5rc5/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc5/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.502499 autumn8-1.0.5rc5/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-15 15:00:54.000000 autumn8-1.0.5rc5/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-15 15:00:54.512499 autumn8-1.0.5rc5/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc5/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc6/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.625373 autumn8-1.0.5rc6/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    12672 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4850 2023-05-16 11:20:08.000000 autumn8-1.0.5rc6/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 11:20:36.000000 autumn8-1.0.5rc6/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc6/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc6/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc6/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc6/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc6/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.635373 autumn8-1.0.5rc6/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc6/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11875 2023-05-16 11:19:37.000000 autumn8-1.0.5rc6/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc6/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc6/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.625373 autumn8-1.0.5rc6/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 11:21:44.000000 autumn8-1.0.5rc6/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 11:21:44.645374 autumn8-1.0.5rc6/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc6/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc5/PKG-INFO` & `autumn8-1.0.5rc6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc5
+Version: 1.0.5rc6
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc5/README.md` & `autumn8-1.0.5rc6/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/analyze.py` & `autumn8-1.0.5rc6/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc6/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc6/autumn8/cli/commands/cloud.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import asyncio
+import base64
 import json
+import os
 import posixpath
 import uuid
 from typing import Dict, List, Optional, Union
-import os
-import base64
 
 import click
 import httpx
 import questionary
-
 from questionary import Choice
 
 import autumn8.lib.api.cloud as cloud_api
 from autumn8.cli import options
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.cli.interactive import (
     coro_click_command,
+    get_deployment,
     normalize_args,
     validate_and_ask_about_docker_image_name,
     validate_and_ask_about_schedule,
 )
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import Sla
 from autumn8.lib import api, logging
@@ -195,17 +195,20 @@
     click.echo(json.dumps(response, indent=4))
 
 
 DEFAULT_DOCKER_CONTAINER_REGISTRY = "docker.io"
 
 
 def build_docker_processing_query_string(
-    organization_id: int, container_image_name: str, machine_type: str
+    organization_id: int, machine_type: str
 ) -> str:
+    # TODO: drop obsolete, unused query string?
     container_id = str(uuid.uuid4())
+
+    container_image_name = ""
     deployment_id = 0
     memory = 0
 
     return "+".join(
         [
             container_id,
             str(organization_id),
@@ -308,15 +311,15 @@
     api_keys = api.user.fetch_org_api_keys(environment, organization_id)
     inference_api_key = api_keys[0]["api_key"]
 
     async with httpx.AsyncClient(
         auth=(str(organization_id), inference_api_key)
     ) as httpClient:
         query: str = build_docker_processing_query_string(
-            organization_id, docker_image_name, machine_type
+            organization_id, machine_type
         )
         url = posixpath.join(
             environment.value.a8f_host,
             "docker-processing",
             query,
             container_http_request_path,
         )
@@ -341,15 +344,14 @@
     model_output_base64_bytes = bytes(model_output_base64, encoding="utf-8")
 
     model_output = base64.decodebytes(model_output_base64_bytes)
     return model_output
 
 
 @cloud_commands_group.command()
-@coro_click_command
 @options.use_organization_id
 @options.use_environment
 @options.use_quiet_mode
 @click.option(
     "--deployment_url", type=str, help="Public dns of your deployment"
 )
 @click.option("--model_id", type=int, help="Model id of model")
@@ -365,23 +367,24 @@
     type=str,
     help="filepath to file with JSON / Raw Text HTTP Body input to pass within the HTTP request",
 )
 @click.option(
     "-d",
     "--decode64",
     type=bool,
+    is_flag=True,
     help="Decode model output from base64 string",
 )
 @click.option(
     "-o",
     "--output_file",
     type=str,
     help="Output file",
 )
-async def run_inference(
+def run_inference(
     organization_id: int,
     environment: CliEnvironment,
     quiet: bool,
     deployment_url: Optional[str],
     model_id: Optional[int],
     model_input: Optional[str],
     input_file: Optional[str],
@@ -396,37 +399,18 @@
     inference_api_key = api_keys[0]["api_key"]
 
     if decode64 and output_file is None:
         click.echo("Please specify output file to decode base64 to")
         return
 
     if deployment_url is None:
-        deployments = cloud_api.get_running_deployments(
-            organization_id,
-            environment,
-            model_id=model_id,
+        deployment_url = get_deployment(
+            organization_id, environment, model_id=model_id
         )
 
-        if len(deployments) == 1:
-            deployment_url = deployments[0]["public_dns"]
-        else:
-            choices = [
-                Choice(
-                    title=deployment["public_dns"],
-                    value=deployment["public_dns"],
-                )
-                for deployment in deployments
-            ]
-            question = questionary.select(
-                "Choose deployment",
-                choices=choices,
-                use_shortcuts=True,
-            )
-            deployment_url = question.unsafe_ask()
-
     if input_file is not None:
         if os.path.exists(input_file):
             with open(input_file, "r", encoding="utf-8") as file:
                 model_input = file.read()
 
     if deployment_url is None:
         click.echo(
@@ -434,18 +418,18 @@
         )
         return
 
     if model_input is None:
         click.echo("You need to either specify model_input or input_file")
         return
 
-    async with httpx.AsyncClient(
+    with httpx.Client(
         auth=(str(organization_id), inference_api_key)
     ) as httpClient:
-        response: httpx.Response = await httpClient.post(
+        response: httpx.Response = httpClient.post(
             url=deployment_url,
             json=json.loads(model_input),
             timeout=None,
         )
         if not decode64:
             logger.info("Deployment responded with:")
             click.echo(response.text)
```

### Comparing `autumn8-1.0.5rc5/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc6/autumn8/cli/commands/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 import click
 import questionary
 
 from autumn8.cli import options
 from autumn8.cli.analyze import analyze_model_file, suggest_model_name
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.cli.examples import example_model_names
-from autumn8.cli.interactive import announce_model_upload_response, normalize_args
+from autumn8.cli.interactive import (
+    announce_model_upload_response,
+    normalize_args,
+)
 from autumn8.cli.validation import validate_input_dims_json, validate_input_file
 from autumn8.common.config.settings import supported_quants
 from autumn8.lib import api, api_creds, logging
 from autumn8.lib import service as autodl
 
 USER_ID_LENGTH = len(str(uuid.uuid4()))
 API_KEY_LENGTH = 32
@@ -443,16 +446,16 @@
 @options.use_environment
 @options.use_organization_id
 @options.use_quiet_mode
 @click.option(
     "-i",
     "--model_id",
     type=int,
-    help=f"Model ID to delete",
-    prompt="Model ID to delete",
+    help=f"Model ID to get info for",
+    prompt="Model ID to get info for",
 )
 def get_model(
     organization_id: int,
     model_id: int,
     quiet: bool,
     **kwargs,
 ):
```

### Comparing `autumn8-1.0.5rc5/autumn8/cli/examples.py` & `autumn8-1.0.5rc6/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/interactive.py` & `autumn8-1.0.5rc6/autumn8/cli/interactive.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from functools import wraps
 from typing import Optional, Tuple
 
 import click
 import questionary
 from questionary import Choice
 
+import autumn8.lib.api.cloud as cloud_api
 from autumn8.cli.validation import IsoDatetimeValidator
 from autumn8.lib import logging
 from autumn8.lib.api.user import fetch_user_data
 
 logger = logging.getLogger(__name__)
 
 
@@ -54,14 +55,40 @@
     ]
     if organization_id not in user_organization_ids:
         raise Exception(
             f"The user {user_data['email']} does not belong to the organization of id={organization_id}"
         )
 
 
+def get_deployment(organization_id, environment, model_id=None):
+    deployments = cloud_api.get_running_deployments(
+        organization_id,
+        environment,
+        model_id=model_id,
+    )
+
+    if len(deployments) == 1:
+        return deployments[0]["public_dns"]
+    else:
+        choices = [
+            Choice(
+                title=deployment["public_dns"],
+                value=deployment["public_dns"],
+            )
+            for deployment in deployments
+        ]
+        question = questionary.select(
+            "Choose deployment",
+            choices=choices,
+            use_shortcuts=(len(choices) < 36),
+            use_arrow_keys=True,
+        )
+        return question.unsafe_ask()
+
+
 def announce_model_upload_response(model_upload_response):
     return announce_json_response({"model_details": model_upload_response})
 
 
 def announce_json_response(model_upload_response):
     logger.info("")  # newline
     logger.info("Done!")
```

### Comparing `autumn8-1.0.5rc5/autumn8/cli/main.py` & `autumn8-1.0.5rc6/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/options.py` & `autumn8-1.0.5rc6/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc6/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/cli/validation.py` & `autumn8-1.0.5rc6/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc6/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/common/config/settings.py` & `autumn8-1.0.5rc6/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc6/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/common/types.py` & `autumn8-1.0.5rc6/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/env/__init__.py` & `autumn8-1.0.5rc6/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/examples/mnist.py` & `autumn8-1.0.5rc6/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/examples/model.py` & `autumn8-1.0.5rc6/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc6/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc6/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/__init__.py` & `autumn8-1.0.5rc6/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc6/autumn8/lib/api/cloud.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc6/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/api/user.py` & `autumn8-1.0.5rc6/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc6/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc6/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/http.py` & `autumn8-1.0.5rc6/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/logging.py` & `autumn8-1.0.5rc6/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc6/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc6/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8/lib/service.py` & `autumn8-1.0.5rc6/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc6/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc5
+Version: 1.0.5rc6
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc5/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc6/autumn8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/pyproject.toml` & `autumn8-1.0.5rc6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc6/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc5/tests/test_settings.py` & `autumn8-1.0.5rc6/tests/test_settings.py`

 * *Files identical despite different names*

