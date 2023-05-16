# Comparing `tmp/autumn8-1.0.5rc7.tar.gz` & `tmp/autumn8-1.0.5rc8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autumn8-1.0.5rc7.tar", last modified: Tue May 16 13:55:30 2023, max compression
+gzip compressed data, was "autumn8-1.0.5rc8.tar", last modified: Tue May 16 14:36:46 2023, max compression
```

## Comparing `autumn8-1.0.5rc7.tar` & `autumn8-1.0.5rc8.tar`

### file list

```diff
@@ -1,68 +1,70 @@
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc7/README.md
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.751744 autumn8-1.0.5rc7/autumn8/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/cli/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/__main__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/analyze.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/cli_environment.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/cli/commands/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13488 2023-05-16 13:55:08.000000 autumn8-1.0.5rc7/autumn8/cli/commands/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 13:13:29.000000 autumn8-1.0.5rc7/autumn8/cli/commands/models.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/cli/examples.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4850 2023-05-16 11:20:08.000000 autumn8-1.0.5rc7/autumn8/cli/interactive.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/main.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/options.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/pending_uploads.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/cli/validation.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/common/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 13:54:52.000000 autumn8-1.0.5rc7/autumn8/common/_version.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/common/config/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/cloud_info.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/common/config/settings.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/config/supported_instances.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/common/types.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.761744 autumn8-1.0.5rc7/autumn8/env/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc7/autumn8/env/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc7/autumn8/env/app.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc7/autumn8/env/cli.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc7/autumn8/env/predictor.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc7/autumn8/env/worker.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/examples/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/examples/convblock.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc7/autumn8/examples/loadMnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/mnist.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/model.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/sbert-alpha.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/examples/tensorflow_custom_layers.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/lib/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/__init__.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/autumn8/lib/api/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api/__init__.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3918 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api/cloud.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc7/autumn8/lib/api/lab.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc7/autumn8/lib/api/user.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/api_creds.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/asyncio.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/http.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/logging.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/logging.yaml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc7/autumn8/lib/package_resolver.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/autumn8/lib/service.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.751744 autumn8-1.0.5rc7/autumn8.egg-info/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/PKG-INFO
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1436 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/SOURCES.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/dependency_links.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/entry_points.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/requires.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 13:55:30.000000 autumn8-1.0.5rc7/autumn8.egg-info/top_level.txt
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/pyproject.toml
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/setup.cfg
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/setup.py
-drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 13:55:30.771744 autumn8-1.0.5rc7/tests/
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/tests/test_io_bottleneck_detection.py
--rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc7/tests/test_settings.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4612 2023-05-16 11:19:52.000000 autumn8-1.0.5rc8/README.md
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       26 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/cli/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        0 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       42 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/__main__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     7999 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/analyze.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1202 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/cli_environment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8/cli/commands/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    13527 2023-05-16 14:35:59.000000 autumn8-1.0.5rc8/autumn8/cli/commands/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    16114 2023-05-16 13:13:29.000000 autumn8-1.0.5rc8/autumn8/cli/commands/models.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    17034 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/cli/examples.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5170 2023-05-16 14:28:29.000000 autumn8-1.0.5rc8/autumn8/cli/interactive.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/main.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     5315 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/options.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3296 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/pending_uploads.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2487 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/cli/validation.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/common/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      102 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      106 2023-05-16 14:31:36.000000 autumn8-1.0.5rc8/autumn8/common/_version.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/common/config/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       50 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6861 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/cloud_info.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2954 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/common/config/settings.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    65887 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/config/supported_instances.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      565 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/common/types.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/env/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4876 2023-04-13 16:57:54.000000 autumn8-1.0.5rc8/autumn8/env/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      246 2023-04-13 17:40:25.000000 autumn8-1.0.5rc8/autumn8/env/app.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       65 2023-04-13 16:50:50.000000 autumn8-1.0.5rc8/autumn8/env/cli.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       10 2023-04-13 16:53:19.000000 autumn8-1.0.5rc8/autumn8/env/predictor.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       11 2023-04-13 16:54:28.000000 autumn8-1.0.5rc8/autumn8/env/worker.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/examples/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      380 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/examples/convblock.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       62 2023-03-10 14:58:37.000000 autumn8-1.0.5rc8/autumn8/examples/loadMnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1283 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/mnist.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      583 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/model.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     2514 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/sbert-alpha.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1955 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/examples/tensorflow_custom_layers.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/lib/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     6297 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/__init__.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/lib/api/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       31 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/api/__init__.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4067 2023-05-16 14:26:52.000000 autumn8-1.0.5rc8/autumn8/lib/api/cloud.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)    11953 2023-05-16 13:55:08.000000 autumn8-1.0.5rc8/autumn8/lib/api/lab.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1348 2023-05-16 11:19:37.000000 autumn8-1.0.5rc8/autumn8/lib/api/user.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1517 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/api_creds.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      614 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/asyncio.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1020 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/http.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1176 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/logging.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      580 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/logging.yaml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3548 2023-03-23 21:40:57.000000 autumn8-1.0.5rc8/autumn8/lib/package_resolver.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3582 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/autumn8/lib/service.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/autumn8/types/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1112 2023-05-16 14:30:08.000000 autumn8-1.0.5rc8/autumn8/types/deployment.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.029531 autumn8-1.0.5rc8/autumn8.egg-info/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     4832 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/PKG-INFO
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1464 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/SOURCES.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        1 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/dependency_links.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       54 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/entry_points.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      136 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/requires.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)        8 2023-05-16 14:36:46.000000 autumn8-1.0.5rc8/autumn8.egg-info/top_level.txt
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     1985 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/pyproject.toml
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)       38 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/setup.cfg
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      295 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/setup.py
+drwxr-xr-x   0 mbalc     (1000) mbalc     (1001)        0 2023-05-16 14:36:46.039531 autumn8-1.0.5rc8/tests/
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)      969 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/tests/test_io_bottleneck_detection.py
+-rw-r--r--   0 mbalc     (1000) mbalc     (1001)     3749 2023-05-14 21:36:00.000000 autumn8-1.0.5rc8/tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc7/PKG-INFO` & `autumn8-1.0.5rc8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc7
+Version: 1.0.5rc8
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc7/README.md` & `autumn8-1.0.5rc8/README.md`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/analyze.py` & `autumn8-1.0.5rc8/autumn8/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/cli_environment.py` & `autumn8-1.0.5rc8/autumn8/cli/cli_environment.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/commands/cloud.py` & `autumn8-1.0.5rc8/autumn8/cli/commands/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     deployments = cloud_api.get_running_deployments(
         organization_id,
         environment,
         model_id=model_id,
         service_provider=cloud_provider,
     )
 
-    click.echo(json.dumps(deployments, indent=4))
+    click.echo(json.dumps([depl.dict() for depl in deployments], indent=4))
     return
 
 
 @cloud_commands_group.command()
 @click.option(
     "-hw",
     "-t",
@@ -268,15 +268,15 @@
     "--custom_headers",
     type=str,
     multiple=True,
     default=[],
     help="Custom HTTP headers to pass",
 )
 @click.option(
-    "-i",
+    "-I",
     "--input",
     type=str,
     help="JSON / Raw Text HTTP Body input to pass within the HTTP request",
 )
 async def run_docker(
     organization_id: int,
     machine_type_param: Optional[str],
@@ -371,16 +371,17 @@
 @options.use_environment
 @options.use_quiet_mode
 @click.option(
     "--deployment_url", type=str, help="Public dns of your deployment"
 )
 @click.option("--model_id", type=int, help="Model id of model")
 @click.option(
-    "-i",
-    "--model_input",
+    "-I",
+    "model_input",
+    "--input",
     type=str,
     help="JSON / Raw Text HTTP Body input to pass within the HTTP request",
 )
 @click.option(
     "-f",
     "--input_file",
     type=str,
@@ -390,15 +391,15 @@
     "-d",
     "--decode64",
     type=bool,
     is_flag=True,
     help="Decode model output from base64 string",
 )
 @click.option(
-    "-o",
+    "-O",
     "--output_file",
     type=str,
     help="Output file",
 )
 def run_inference(
     organization_id: int,
     environment: CliEnvironment,
```

### Comparing `autumn8-1.0.5rc7/autumn8/cli/commands/models.py` & `autumn8-1.0.5rc8/autumn8/cli/commands/models.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/examples.py` & `autumn8-1.0.5rc8/autumn8/cli/examples.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/interactive.py` & `autumn8-1.0.5rc8/autumn8/cli/interactive.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import asyncio
 import datetime
 import json
 import re
 from functools import wraps
-from typing import Optional, Tuple
+from typing import Optional, Tuple, TypedDict, Union
 
 import click
 import questionary
 from questionary import Choice
 
 import autumn8.lib.api.cloud as cloud_api
 from autumn8.cli.validation import IsoDatetimeValidator
 from autumn8.lib import logging
 from autumn8.lib.api.user import fetch_user_data
+from autumn8.types.deployment import DeploymentView
 
 logger = logging.getLogger(__name__)
 
 
 def normalize_args(name: str):
     """
     Use this with a click.group to allow both underscores and dashes
@@ -55,28 +56,36 @@
     ]
     if organization_id not in user_organization_ids:
         raise Exception(
             f"The user {user_data['email']} does not belong to the organization of id={organization_id}"
         )
 
 
+def render_deployment(deployment: DeploymentView):
+    return (
+        f"{deployment.status} model {deployment.model_id} "
+        + f"on {deployment.service_provider} {deployment.instance_type} "
+        + f"(id={deployment.deployment_id})"
+    )
+
+
 def get_deployment(organization_id, environment, model_id=None):
     deployments = cloud_api.get_running_deployments(
         organization_id,
         environment,
         model_id=model_id,
     )
 
     if len(deployments) == 1:
-        return deployments[0]["public_dns"]
+        return deployments[0].public_dns
     else:
         choices = [
             Choice(
-                title=deployment["public_dns"],
-                value=deployment["public_dns"],
+                title=render_deployment(deployment),
+                value=deployment.public_dns,
             )
             for deployment in deployments
         ]
         question = questionary.select(
             "Choose deployment",
             choices=choices,
             use_shortcuts=(len(choices) < 36),
```

### Comparing `autumn8-1.0.5rc7/autumn8/cli/main.py` & `autumn8-1.0.5rc8/autumn8/cli/main.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/options.py` & `autumn8-1.0.5rc8/autumn8/cli/options.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/pending_uploads.py` & `autumn8-1.0.5rc8/autumn8/cli/pending_uploads.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/cli/validation.py` & `autumn8-1.0.5rc8/autumn8/cli/validation.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/common/config/cloud_info.py` & `autumn8-1.0.5rc8/autumn8/common/config/cloud_info.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/common/config/settings.py` & `autumn8-1.0.5rc8/autumn8/common/config/settings.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/common/config/supported_instances.py` & `autumn8-1.0.5rc8/autumn8/common/config/supported_instances.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/common/types.py` & `autumn8-1.0.5rc8/autumn8/common/types.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/env/__init__.py` & `autumn8-1.0.5rc8/autumn8/env/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/examples/mnist.py` & `autumn8-1.0.5rc8/autumn8/examples/mnist.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/examples/model.py` & `autumn8-1.0.5rc8/autumn8/examples/model.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/examples/sbert-alpha.py` & `autumn8-1.0.5rc8/autumn8/examples/sbert-alpha.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/examples/tensorflow_custom_layers.py` & `autumn8-1.0.5rc8/autumn8/examples/tensorflow_custom_layers.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/__init__.py` & `autumn8-1.0.5rc8/autumn8/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/api/cloud.py` & `autumn8-1.0.5rc8/autumn8/lib/api/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import requests
 from requests.auth import HTTPBasicAuth
 
 from autumn8.cli.cli_environment import CliEnvironment
 from autumn8.common.config.settings import CloudServiceProvider
 from autumn8.common.types import Sla
 from autumn8.lib.api_creds import retrieve_api_creds
 from autumn8.lib.http import require_ok_response, url_with_params
+from autumn8.types.deployment import DeploymentView
 
 DEFAULT_API_TIMEOUT = 60
 
 
 def get_running_deployments(
     organization_id: int,
     environment: CliEnvironment,
     model_id: Optional[int] = None,
     service_provider: Optional[CloudServiceProvider] = None,
-):
+) -> List[DeploymentView]:
     autodl_host = environment.value.app_host
 
     params: Dict[str, Any] = {"organization_id": organization_id}
     if model_id is not None:
         params["model_id"] = model_id
     if service_provider is not None:
         params["service_provider"] = service_provider
@@ -32,15 +33,18 @@
         url_with_params(deployments_api_route, params),
         headers={"Content-Type": "application/json"},
         auth=HTTPBasicAuth(*retrieve_api_creds()),
         timeout=DEFAULT_API_TIMEOUT,
     )
 
     require_ok_response(response)
-    return response.json()["deployments"]
+    return [
+        DeploymentView.parse_obj(item)
+        for item in response.json()["deployments"]
+    ]
 
 
 def deploy_by_best_sla(
     organization_id: int,
     environment: CliEnvironment,
     model_id: int,
     best_sla: Sla,
```

### Comparing `autumn8-1.0.5rc7/autumn8/lib/api/lab.py` & `autumn8-1.0.5rc8/autumn8/lib/api/lab.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/api/user.py` & `autumn8-1.0.5rc8/autumn8/lib/api/user.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/api_creds.py` & `autumn8-1.0.5rc8/autumn8/lib/api_creds.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/asyncio.py` & `autumn8-1.0.5rc8/autumn8/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/http.py` & `autumn8-1.0.5rc8/autumn8/lib/http.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/logging.py` & `autumn8-1.0.5rc8/autumn8/lib/logging.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/logging.yaml` & `autumn8-1.0.5rc8/autumn8/lib/logging.yaml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/package_resolver.py` & `autumn8-1.0.5rc8/autumn8/lib/package_resolver.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8/lib/service.py` & `autumn8-1.0.5rc8/autumn8/lib/service.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/autumn8.egg-info/PKG-INFO` & `autumn8-1.0.5rc8/autumn8.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autumn8
-Version: 1.0.5rc7
+Version: 1.0.5rc8
 Summary: Utilities to export models to the autumn8.ai service
 Author-email: Autumn8 <team@autumn8.ai>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Autumn8 CLI
```

### Comparing `autumn8-1.0.5rc7/autumn8.egg-info/SOURCES.txt` & `autumn8-1.0.5rc8/autumn8.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -46,9 +46,10 @@
 autumn8/lib/logging.yaml
 autumn8/lib/package_resolver.py
 autumn8/lib/service.py
 autumn8/lib/api/__init__.py
 autumn8/lib/api/cloud.py
 autumn8/lib/api/lab.py
 autumn8/lib/api/user.py
+autumn8/types/deployment.py
 tests/test_io_bottleneck_detection.py
 tests/test_settings.py
```

### Comparing `autumn8-1.0.5rc7/pyproject.toml` & `autumn8-1.0.5rc8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/tests/test_io_bottleneck_detection.py` & `autumn8-1.0.5rc8/tests/test_io_bottleneck_detection.py`

 * *Files identical despite different names*

### Comparing `autumn8-1.0.5rc7/tests/test_settings.py` & `autumn8-1.0.5rc8/tests/test_settings.py`

 * *Files identical despite different names*

